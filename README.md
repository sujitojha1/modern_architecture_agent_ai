# modern_architecture_agent_ai
modern_architecture_agent_ai

## Highlevel Plan

### 1) Stabilize Context & Memory Handling
- Implement `_ensure_parsed_value(value)` using `ast.literal_eval` to convert stringified lists/dicts into real Python objects
- Apply recursive parsing across:
  - inputs (ex: `inputs['urls']`)
  - tool outputs
  - agent outputs / extracted values
- Save **rich clarification memory**:
  - store: “Agent asked: <Q>. User answered: <A>” (not only “Yes”)

### 2) Fix Core Loop Logic & Reporting
- Fix **Blind Formatter**:
  - explicitly inject `all_globals_schema` into `FormatterAgent` so it receives `research_summary`, `code_analysis`, etc.
- Fix **Infinite Loop ending**:
  - inject warning prompt on `turn == max_turns - 1`:
    - “FINAL TURN: stop browsing and summarize now”

### 3) Improve UX Bootstrapping
- Implement **Bootstrap Graph**:
  - create a minimal graph immediately with a `Query` node + “Planning…” node
  - update node status while `PlannerAgent` runs (avoids blank UI / infinite spinner perception)

### 4) Add Robust Extraction Fallbacks
- Implement 3-strategy extraction in `memory/context.py`:
  - strategy 1: check runtime/code-execution variables
  - strategy 2: read from JSON output keys
  - strategy 3: fallback parse from `final_answer` when agents misplace outputs

### 5) Upgrade MCP Servers Layer (S20 Parity)
- `mcp_servers/multi_mcp.py`
  - switch from hardcoded dict → dynamic `mxp_config.json`
  - add git clone + install support for MCP servers
  - add caching via `mcp_cache.json`
  - increase default timeout to 20s
- `mcp_servers/server_rag.py`
  - parallel ingestion (`ThreadPoolExecutor`, max_workers=2)
  - thread safety (`pdf_lock` to prevent crashes)
  - optimized semantic chunking (`semantic_merge`)
  - caption-first image ingestion (embed image captions in FAISS)
- `mcp_servers/server_browser.py`
  - restore bulk tool `search_web_with_text_content` for efficient research

### 6) Harden Prompts for Headless Execution
- Update `coder.md` with strict headless constraints (no GUI actions like `plt.show()`, `cv2.imshow`)
- Update `planner.md` with MCP-browser-only rules (no desktop browser assumptions)
- Add missing App Builder prompts required for frontend workflow

### 7) Final Demo + Submission
- Run & record demo query:
  - “What’s the latest revenue of Dhurandhar Movie”
- Run & record a separate RAG query
- Confirm:
  - no crashes on stringified lists
  - formatter outputs filled (no `[None]`)
  - UI shows planning instantly
  - agent summarizes before turn limit
- Submit GitHub repo link + YouTube full-flow video

