Okay, recordings are on. All right, so today's session is
finally on something that you're going to be carrying forward and this is something that will allow you to build
something that you actually see outside or other application in other applications or uh
you can productize it actually you will be able to take it back to your companies and implement something right.
So that's a modern architecture we've been going to and uh I can show you where it's going to lead you to into. So
this is where I was last week uh where we have the runs and other things
running but I have a fully upgraded version of this also. Uh this is what you're going to be building as the part
of the remaining course. I'm going to explain the concepts behind and you're going to go back and implement uh things
that uh allow all of this to happen. But we're going to see from the theoretical point of view what is required to take
it to this level and what to do about it. I've changed the UI a lot. So I'm going to show you my modern one uh which
I call actress. This is working but uh I'll show you the
actual one.
This is the old one. Changed the UI and added lot more features to it.
This is my new platform.
So, a bit of UI changes and a lot other things. So, here's how I initiate my new
run. Um what should we ask anyone? Any question?
Okay. Yeah. What's the uh what's happening with the current uh uh silver reserves
uh in the world and where is the money flowing?
Where's the money flowing? Yeah.
Okay. So now when I click run, what you'll see is going to happen is you're going to see a flow coming in front of you. You're also going to see the
planner agent actually uh the UI actually telling you what the planner agent is thinking. Uh the flow will come
in front and as each note starts working on it, it will also have it trajectory
defined for you. So the task here is formulate execution plan. That's what planner agent is doing. It decides to go
for retrieval agent. One is working on research current status of global silver. The other is artifact track
major money flows related to silver including investments and as it is going in the back end it is
right now searching a lot of internet uh databases which are going to be visible in this section later on
it's doing this at the back end. By the way, we full screen
calling a lot of requests going on a lot of different places. It's done mostly send it to thinker agent. Thinker agent
is sort of thinking on how to respond.
And finally format agent which is creating a detailed comprehensive report. The report will come on the preview.
Okay. So here's the report. The solar market in 2026 is
characterized by persistent structural supply deficit driven by decreased mine production and increased industrial demand particularly from clean techch
industries such as solar electric vehicles and emerging technologies like AI etc. table of content of where things
are, how things are structured, potential risk, opportunity, supply, demand, price volatility, investment,
regulation, and all of the stuff. Okay. Now, that's not all. What I've also done
is I can go back here and actually change the prompt. Maybe I had something wrong. I didn't
want to do that, right? So, that I can do and I can go and click again. I can go to retriever agent, go to its
overview. And this was a agent goal. Maybe my planner did not give it enough information to search or maybe I want to
trigger something else. So I can go here and edit this and I can go here and change this guy also. And by the way, we
can see what all uh websites it went into and what it
scrolled into. So I tried and added as much detail possible. Some websites open, some website don't open for us because this is not a full web browser.
Uh we also have preview of things where they matter. uh the stats of how much tokens they spent in input and output uh
overall overview thinker agent what was the input goal it read this particular stuff you you see the silver money flow
t02 none that is guaranteed to be read because we are using network x right that that guarantees there and that's
the important part and for matter agent always is always going to get uh this goal and uh we can ask it to convert
this into HTML also right now right it's right now giving us a markdown format it
has input of again something on D3 and it is giving us kind of an output again
some idea on the cost and the cost the call self was false code is not here but
if I were to look at code here I will see the code code A and code B and we'll see which code was executed so that is
also shown for each agent so it's fully basically baked in all the features are essentially in to understand from here
what is happening and again start for that but most importantly I can go to formatter agent and click this button
This button says build app from the node. Now because I have the main flow
ready, right? This is the main flow. And I can show you some other runs also. For example, this was the F1 run. Donald
Trump, how much movie durand made. Now it has actually made some 1200 cr. That's interesting,
right? So let me play with this guy. Okay. And I think I have this guy. So I
can go here and click this button. Remember that app. Okay. But what are the other icons? These are the other assignments that you're going to be
building soon. Then next one is going to be on the rag. Let's click rag.
Now here's a normal filter. I can write unmole sing and mol sing is going to be
found on this particular site. It's probably somewhere I need to search here. But I also have chunk search.
Right. First of all, let's look at this document. Because this document is here, I can click this chunk and I can visually see what are the chunks that
were made by my algorithm. This is our semantic chunker that we discussed earlier fully integrated seeing exactly
what is happening on each chunk and possibly referring to it. Most importantly, I can go back here because
everything is already done. I can select this guy add to context
and click insights and this is the chat that I have. Now that documents context is taken this chat and I can talk talk
about it. If we send this particular uh text to Gemini, it will get some ideas and can have our own chat here. But
that's not that's something that you're going to be doing in the next session. So slowly you're going to see uh how we
improve. But I can do a full rag searcher also, right? So for example, unmold sing
uh paid df. This is again all running on my system.
No, no gemini. Here we are using gamma model and nomic uh fires index. And if I
click it's going to on uh markdown there's no page number but if the page
number was there it is supposed to take me to that particular page and scroll which is not happening
right now. Sometimes it works sometimes it doesn't
work. I give it some time. Yes. So it took me to page number 23.
So something should be here where un was mentioned or this is a section I should be looking at this
un is mentioned. Yeah in remarks it is mentioned
there in the remarks. Yeah right there there also next page also in the
remarks it is mentioned I've added a feature of uh highlighting that but I'm not sure why it's not
coming the third chunk p it says p number 12 is supposed to take us there.
So some debugging problem. I think it will scroll to 12. Yes. Yeah. Right. So that's there now. So basically
this is the search rag. Now what also happens is as we discussed this as I
just added this if I go to rag I have mapped that here. So today's 10th that
JSON is here. What is happening to the current silver reserves and at the back end I'm hoping the chunks are already
made or being made. Chunks are not made yet.
Yes, chunks are not made yet. On bottom you can see indexing, right? I click index
and hopefully it should index in some time. My uh you can see temperature is going up because this uh llama small
llama is actually taking up some GPU.
It should be done in a moment. say start anyway. So it's showing here
whenever uh our rag is not up to date on the bottom it basically comes there I
can click escape I can see that one of the one of the 51 files need indexing so
some of the files are still pending which I have trans which I moved here so that's rack that's how I wanted to build it and uh implement things end to end
now rag doesn't work on keywords you remember
Yeah, semantic search, right? It's a semantic search.
But it works for us. So, how does uh keyword search work with rag is something we are going to touch
upon in next session. I have some content on this in today's session also because I want you to uh get this end to
end. Okay. Then we have MCP. These are some of the MCP. So, this is something that we have built. Uh there are three
MCP servers for us. One of them is browser. Then we have rag sandbox. Then
alpha alpha vantage. This is a third party. So if I click it, it opens up the website in the in the between. And here
I can select which functions I want to send to my uh agent. And you can see
there lot of them. I don't want to send any basically. Then I can select Yahoo Finance which is something I'm using.
Get stock price. So if you actually ask uh my agent right now what is the stock price of Apple? It uses this. it doesn't
go online search and then gets back right this is something that we have uh we can use for some free then we have
remy remy is something I'm going to spend a lot of time in future but remy is essentially how are we extracting the
content from the discussions we have with our agent and storing that as remember me that's remy and I can
manually add stuff also I can manually add that I am a non okay I'm a pure
veget I'm raw vegetarian uh hate
science I don't and love what should I
use I don't like basically I can do that and I can save that as a fact in fact I have saved some facts about myself
for example to revenues load I need to fix some of this AQI and these are some
of things are old so it's not capturing proper but the new memories user teacher school of AI and users located in
Bangalore those are something I have added myself otherwise it just extracts information from the runs and saves in
re so it understands again all of this goes back to the prompt so what is it that you want to store about the user
and every once in a week uh it takes the whole data goes to Gemini and builds a profile for me this you can do locally
also so this is a comprehensive psychological and professional profile of myself this is what the agent thinks
about Okay. Okay. Then we have explorer. Explorer is for code. You can add any uh GitHub repo
or in fact download or upload any code and it will tell you how the code is structured on the right side. You can
read more about it. Then we have apps. This is the interesting one and I was saying durand
right oh it's already mentioned 112 here okay so let me select this and change
the number okay and net revenue collection also let
me change to only 128 code all right let me save it I'll show you how this is
made but then I can refetch now what I'm doing is I can add my preferences also uh get the
latest data uh today is what today is 10th Jan. Now what it is doing
I'll show you the full workflow the final summarizer that we had uh in our agent flow we can create an app using
that you can see what happened here right you can create an app using that that app has some components so I'll
show you manually how we can create an app so let's say we create a manual app and design both we can do let's do a
design here's a build canvas and I can go in components and I can drag and drop some components here so this is my
header Then I need a text block. Let's drag everything as of now. And then we'll
make something interesting. I have a chart. Let's say we have revenue box. Then I need some other charts. Let's say
we have a Santi chart. I love Santi chart. Then in the finance we have
no let's say quiz. Yeah, we have a quiz also by the way. quiz block.
Then we have this big blocks. Uh let's say we go for this block. Okay.
So we can arrange it and design it in a way that looks better to you.
The auto designer I've not designed yet.
And let's pull this to top because both the colors are there to Make it look
better.
Q&A won't make sense. Let's remove that. Okay. So, let us imagine that this is a
basic dashboard that we have made. Okay. Now, let me save it.
Now, let me click refetch. Okay. Make this
dashboard specific to what do we do?
Uh CSK team in IPL
in India. I did all fields
and data with latest
We can show the wins, losses,
revenue, generation, etc. Make sure each
component has real updated data.
I'm doing this for the first time by the way this extreme because early at least I had some uh Thank you. So zero IPL
titles I'm not okay five IPL titles $4.4 4 million fan following $17 million
sponsorship revenue and 10th rank in 202 I'm not sure if this is correct or not but the dashboard wise comprehensive CSK
1875 cr is the revenue uh scorecard is 44.6 six then media rightites and
sponsorship and mercandize and ticket sales and price money all this data is coming from there right so my idea is that this is how we want the apps to be
and right now I do not have to build any API any server or anything u the preview looks better u and if you keep I keep on
adding more then you can actually build more interesting stuff right now there is u uh this ID crash course also this
whole quiz was built by again AI you just add a question and it picks the right component places it there So
something that we can do for other things as well. AI purify market. I can again click it refresh and it goes out
and figures out the auto awesome
right so that's my idea of dashboards like we will have we can have multiple different kind of dashboards and I will continue to expand this then I have a
news section what happens in news section is I go to hacker news uh because I love it I can click this it
opens this sometimes it will fail if it fails then I have this reader view which is definitely better than the nor normal
So this is the latest news in the on the hacker news. I can select this and again as I said I can add to my context. Now
the context also remembers the three other contextes I added from the older document. So with respect to multiple documents we can build context and have
a discussion with whatever we want. So this is my browser and uh whatever we
want to discuss with it and then there are the interesting links for example and uh it says twitter.com but uh it has
API I've not indicated that. So simplest thing is go online and figure out some search results for that's what I've been
doing here. Simon Wilson again really good um documents that he mentions. So I
get to read all of them here. Most importantly archive right it takes a bit
of time to review or come here
and add a bit of refresh.
Hopefully it will come. Okay. So I think something so they will keep on changing things. I will have to continue.
It shouldn't fail. Let me see what's happening on the back end.
Truthless removal did not work. Okay. Some request is
okay. Better.
If it doesn't work now, then I'll try and show you next time. Yes, perfect. Worked this time. So this
is the latest paper on archive related to AI. So G GDPO good reward decoupling
blah blah blah. Uh then again PDF uh we have a reader view also for that it's
going to not take the PDF convert that into markdown format for us and store it uh so you can view it or whatever you
want to do. And of course I can select any of this and add to context and talk to my guy.
Right. So this is how I want yeah this is a markdown conversion from the library that we've been using traffic
later sometimes it will fail sometimes it will win but this is one way for you to keep on
uh learning things and implementing things and learn is the last thing that is pending from my side now I saw this
guy called deep tutor not sure how many of you saw it it's getting very uh
popular I think two two million something downloads or something was talking uh
but I tried install it. It failed a lot of times. I didn't like the overall structure. So uh I was already building
learn and I saw this. So there's a lot of learnings from here. Most of the inbuilt things are already built for us.
For example, the document knowledge uh really good rack search and all the
component that we need. So things are already there. I just need to literally put things in structure. So learn
imagine we have a add topic. When you add a topic add document inside rag is done. uh create assignments or create uh
uh lessons and it starts populating on the right side and of course like some cool things also. So this is there then
you can click play because why not it looks cool. So it will show you what happened first, what happened second, so
on and so on. But the good part is basically you can stop everything and use it. All of this is possible because
we just did one thing and that was move to network X. All right. Now let's start start talking
about network X. what is it and why it is important for us. Now till session 14
we had we did mention that we have dynamic stuff and other things but it was not really dynamic. It was not pure
a synchronous. We had a fixed pipeline because we had a perception, decision and execution. All of those things will
go in the sequence. Right? In session 15 and NX to uh keep reminding you that all
of this is possible because of the NX library. Now we have planner who can go to retriever coder browser and thinker
at the same time. All of them will be executed because network X takes care of the node finished or not. So if a node
is finished the data is actually passed on and kept ready for the next processing. So if there is branched as
multiple agents inside or sub aents inside it will continue to work with it and continue to finish it. Right? So our
planner now decides multiple different agents at the same time and we have 10 of them. Uh by the way I forgot to show
you one more thing which is if you go in settings and go to prompts you'll see all the prompts. We have app generation
prompt. This is the guy that generates app for us. So for example app uh create
a new one uh aski uh let's call this what do we call this
uh uh who was the director of corona or DD current
board think of problems
is facing new talent,
missed movies, missed events. He could take part in
uh other characters.
Current revenue
spending in current movie productions
foreign locations not available
and then make this amazing dashboard.
Use as many
different as possible expecting
minimum of let's say 15
All right, let's see what Karan is interested in. Uh let's go back. Current
Joe's personalized dashboard. Company name K Alphabet Inc. Uh movies are rated eight. Movies produced 50 plus. Award
went 100. Social media following 25. Box office collection is increasing. That's
good. Uh movie rating then Bloomberg. Okay, this is not updated. Uh project a
pre-p production some upcoming projects. K is a highly influential figure. Add my notes. influential highly influential
contact current so on and so on right it's there like I I need to improve the prompt to get this correct now if I
change the prompt how do I now improve it that problem is something that I think is the best is best solved by this
guy which is basically app generation prompt right so app generation prompt essentially tells gemini that here are
our uh components uh these this is how we define our components and uh this is what I want you to do and it generates
an app and we can render it then we Hydration prompt. Hydration prompt is that button. Uh if you go in app the
refetch is at hydration prompt. Right. So all the prompts are managed here. Report to app prompt. Uh this
converts uh this basically sends the summary from the summarizer to the app
uh generation prompt and uh that's how we generate app there. Then we have browser prompt, right? Uh how do we go
online? What do we search? We have a clarification. Clarification working really well by the way. It stops midway. Uh let's do something like this. Uh,
let's start.
And yeah, what is the
current AQI of my city? Ask me
questions if any. So, planet agent, what is the current
API of my city? Ask me questions if any. I'm hoping it's going to ask the
clarification agent. No clarification because it knows
It's picking the retrieval
from there. If it does then perfect. If it doesn't then ah this is wrong. This should have been the clarification
agent.
We lost that. Okay, I need to fix it.
It's not available. Okay, missed it. One bug caught.
Okay, but I hope you get what I'm trying to say, right? Clarification agent was working very well. I may have broken it.
That's why there's no uh us
Go one question is that so is this UI look
and feel are we using any framework or libraries kind of thing or it is custom made everything custom made no basically this is
tailwind and react that's all react okay okay uh what is the current AP asking uh
okay let me hack let me CL
is for
now it's basically running the old one and the new one. This was the old This was the new one. Let's save the session.
And you can see that now has called clarification. Now if we run this
Oh, I forgot how.
Okay, let me do this.
I'm yet to implement run all button. Basically, if it run all, then it's going to stop, hold and ask.
Okay, it is asking Kolkata.
Uh the for kolkata as of current date is unavailable. Would you like to search for nearby city or something else? Okay,
so it's not picking back. Maybe it's not there. Let me check. Let me
back. It is not picked for some reason. Okay, let me debug this. But this is where I also want things to go working
sometime not working sometime injection as a problem. But the main point is that it it can pick the complex graphs. One
of the graph was extremely complex. Something like this for example or this for example
multiple retrievers multiple thinkers multiple retrievers based on the last inputs and thinkers and final good
report
and of course this can be converted into app app as well. All right so this is
possible now. Oh but I was showing you something else. I'm sorry I was showing you the prompts. So we have these
prompts to be tested further. These are clarification. Then we have coder. Then we have decision, distiller, formatter,
planner, QA, retriever, summarizer and thinker. Right? So
I can modify my prompt here and save it and uh enable the whole system to work again. So the core logic is different
now. Earlier we were using main.py. Now we have app.py. We had agent loop v3.
Now we have v4. We had a fixed loop of perception, decision, action hardcoded. But now we have planner agent that
creates a graph and based on what node is on the graph that execution happens. Earlier we were managing managing a
state using context manager and agent session. Now we have execution context manager but that's literally just
network X. We don't have to manage a state. Network X manages state for us.
Agent composition also we have way more number of agents and smallest multi-purpose agents as well to make
sure that uh the task is very well contained. In fact, if you're notic I'm not sure how many of you are using
anti-gravity or cursor and noticing that cursor and anti-gravity both have
started sending sub aents. For example, whenever the browser automation happens, it's through the sub agent. It opens a
sub agent, gives a task to sub agent and ask it to revert back, right? They're managing the context with as few um key
information as possible. So, how does a new architecture look? It's a
very different architecture code-wise also. Uh it's a but it's a very simple architecture also very limited lines of
code. The problem that we are trying to solve is a context confusion. Uh which context should go to what is now very
well defined by our network. Now the one thing that so uh as I am also extending
this application I'm going to be adding my own cursor inside. And the reason to do that is not because uh I want to use
my own cursor. I wish I could but the reason is that if you see cursor uh recent blog also
cursor context discovery that three days old
yeah three days old dynamic context discovery right everyone is struggling with the same thing everyone is trying
to solve this particular problem so coding agents are quick changing quickly changing how software is built okay
files for dynamic context discovery dynamic context discovery is far more token efficient as only the necessary
data is pulled into a context window right I think we already have the right infrastructure to implement something like is because uh what we don't have
right now in our architecture is a context agent and I think we can build it very well which the context agent can
look at different nodes and build the context and pass that on. Is that a additional run? Yes, it is but even GMA
can do it very well. Uh I want to show you how good GMA is.
open on my left tab. Uh on full screen these they don't come.
This is GMA. So let me ask uh it can't go online. I don't think
I don't think tools are inbuilt. So I'll ask the question.
Yeah, tools are not there but it's coherent. Uh what do you know about uh
fast attention using elements?
Look at the speed and it's qu like app uh it's not going to not understand what is not a good
context. And you can see like the GPU usage is controlled not bad
right so the the small context manager can actually be just gamma that is running in the background so everyone is
fighting for this files for context discovery what they are trying to say is that u and I I think I like the approach
also why don't we convert a particular uh flow into a file okay so here's how
we have used dynamic context discover covering cursor turning long tool responses into file right so if required
you can actually read a file I found a startup uh which was just doing this as a service and I've unfortunately lost a
link of that because that was a they were claiming that you can just give us all your tools and we will tell you
which tool your MCP is which tool is required by our LM at runtime and that was a beautiful because they were dro
they were claiming that they're dropping context by around 80%. Because you saw when I showed you our MCP also, right?
Just just look at that hell. Uh just look at how many tools are there. If we enable just this MCP, we are going to be
drowning in context. So basically turning long tool responses into files and using those files, right? And the
files can be summarized as well. So their claim is that this is what is happening. The system instructions and
the tools that were there and uh the tool definition that were there, they can collapse it and reduce a overall
context. This is one reason I want to build something like a coding agent to
uh and uh someone shared on this link
a simple I can't search. So
let me see if I have it on my history.
No, it's not or maybe my
Yes, I found the link. So, there's this guy who has written a really good blog called Mil
not mill. Okay, let me
M I L A I L I C
Mi H. Sorry. M I H.
Yes, this one. The emperor has no clothes. How to code plot code in 200
lines of code, right? Very interesting blog and you can literally use the four
code setup that he has shared. What he's saying is that uh coding agent is basically you the LLM, your program, the
results of the LLM. The tools you need are read files, list files, and edit files. and the basic capability that you
have to provide. Greb, bash and web search and uh you can literally build a very very simple code coding agent. I
want you to start using these for your practices to make sure that you know how end to end flow can be built right I'll
share this link in the chat just in case you're interested and you can literally build this today of course with no UI
and other stuff but then once you build this talk to charge GPD or Gemini and ask it that hey do you think I'm done
and it's going to tell you no you have something like 100 years away from the actual coding agent but it's a really
good start so the context confusion is something that we have to solve and we think network X is something that can
help us a a lot in that particular part. Secondly, greedy logic uh the smaller models or uh without a proper
availability of a network for the for the Gemini or even u smaller model. It
will come up with a very short thing because it doesn't know what are the options it has available. It doesn't know the pieces of the chess uh board.
But because you have a graph and you can say that here are 10 things and you can arrange them in an order. Each sub aent can do its own work and we don't have a
serial bottleneck. We're not doing one by one. we can do multiple at the same time and then make make overall search
faster. Now uh there are two videos that I shared on the uh chat earlier. So
Banlu CTO of AMP code who shared basically four of their own coding agent he also mentioned the same thing. At its
core an agent is just a for loop with tool calls and model in the middle. The key levers for building the model are
the tools and how they iterated. Right? That's what we want to make sure that our tools are something that can be
decided by each agent and they can run and u have the context limited to what they want. Now in the shallow passes all
the agents we had till now we were essentially running it as long as we were getting a
feedback. It was a chain of command step A step B step C and if it stops then it stops. What we want is the network
discovery. If it stops for example you saw my uh graph stopping somewhere or failing somewhere. Now we have a clear
idea where it failed and now we can add a backend logic to see why it failed open up a clarification and then run
again right so by I hope by the next week I can show you that part also so the core more the four main pillars of
deep agents are explicit planning that is something we are solving right now there are a few uh things that we need
to uh make sure first is that fail problems fall tolerance you also had
some of you had this question how do we handle uh uh basically tolerance to failure Here here you have a clear idea
what has failed and what action you should take is something that you can either ask another agent to work on or
you can add a human in the loop. We have a hierarchal delegation task are divided into subtask and each one does its own
very similar to how anti-gravity or cursor first makes a to-do list and then
gets a confirmation from you and actually does it is very similar to what we're doing. Literally if you change the UI of what I showed you into a to-do
list then it looks very similar to what anti-gravity is doing. We have persistent memory. Everything that happens actually gets stored in JSON and
I can trigger uh the full backend integration on the MCP side for example
not MCP rack side that okay some files are missing why don't you index everything right and then I can do auto
index I have not enabled autoindex because I want to control where it actually starts indexing otherwise I'm
doing something uh training a model and opens up uh indexing at the back end don't want that then we have context
engineering right again because of the network we have the context a bit of context handling already handled for us
because a node is connected to A to B and we can explicitly connect any other node the context is limited to the
information coming from them if you want on top of them we can add uh some sort of a summarizer which distills it in
cell we also already have a distiller agent and it job is to just do that so
the pillar one we are doing explicit planning that's where the architecture comes from each node knows where the
information is going to come from and where it is going going to go. So for example, plan graph is connected to retriever agent. That's the first
connection. Then it's connected to another retriever agent. So here it's searching quantum supremacy uh uh search
error correction and then thinker agent and it's connected to synthesize t1 and t2. Right? So t1 and t2 are connected.
So reads data from t01 and t2 becomes very easy because that's how a network is actually decided or defined. So even
if our uh LLM is not good enough in defining the network network we can just see what uh it wanted basically I'm
saying instead of read it mentioned something else we can read these JSONs and actually link them together right so
edges are clear t1 goes to t3 t2 goes to t3 to graph becomes very very easy to
handle now in terms of hierarchal delegation sub aents we already have a sub routine because we have the finder
we have the oracle library and kaken these are the four ones that claude was talking about right our names are
different the finder for us is retriever agent the oracle for us is a thinker agent the librarian is a browser agent
and the kaken is a coder agent so we already have those four so we can verify the prompt of these guys pick a much
better LLM and convert this into a strong financial agent or a strong financial um evaluator or a coder or
anything that you actually want now we have persistent memory and graph state some bug in the remy side so I'm
not able to link it I'll see why that happened so deep agent decouple memory from the
context window both are different right the context injection is happening from remy I want to that's why I built it
separately the the rag is the whole thing that gets called remy is something
that is extracting contents okay it came now 16 minutes ago yeah uh remy is
something that extracts this context and before u we send a question to uh
planner agent it we do a quick search and attach those things to planner agent also so that becomes a context possibly
for my own debugging what I should do is when the planner agent is being called I should actually see what is the context that were attached here that will be a
very very clear debugging tool for me also we have some questions
come u so unlike like earlier where we had uh
the components within the loop predefined uh it is the dynamic uh
defining of the components uh that we are looking at in in this architecture right that's correct from the
that's correct earlier we okay so earlier the chain of command was that we have the
the sequencing was fixed right the sequencing always was for us
Is it?
Yes, this was the sequencing perception decision summarizer. Perception coder summarizer.
Correct. But now just look at this one. Uh this one we just searched it, right?
Planner and two separate retrievers. Now in the old case we never had this kind
of freedom. We were forcing the model to do it but it was not able to do this two different searches and then link it
back. Right now before uh we had we just have summarizer everything is thrown on a summarizer and that can be a block of
full information from all the websites ads and everything that we have scrolled. But now we have a thinker agent between similarly if I look at
other runs uh how much movie this may distiller we have a distiller also right. So review the search results. So
here we get lot of results from 1 2 3 4 5 and distiller takes all of that and
then compresses that into simpler output. This is the raw input that it's getting
and it gives out information which not available here but gives information to formatter in such a way that it can
actually summarize properly. Right? So we have this bottlenecks in between whose job is controlled and the planner
can decide to add these bottlenecks. Earlier we never had such bottlenecks because it was always perception decision or maybe a coder and then
summarizer. Uh command. Yeah. So a planner is different than
planner agent is it which is having a holistic overview of all the components
that yeah that's planner agent only planner agent can call other agents. Okay. And planner agent knows about
itself also like in the graph. Okay. Yes. So if you go and look at the
planner the prompt under K consulting style uh role
strategic planner output plan graph next step ID you are a planner agent your job is to convert a user's complex into
multi- aent execution plan u environment consent headless server no browser do not plan task that require
opening chrome basically ragable sandbox philosophy think like consulting firm simulate a 5 to 10% consulting
And you are going to get this you have this mid session if it is there then
this is the output agents are retriever thinker distiller coder for matter QA clarification schedule planner and so on
and definition of what these agents can do
here I can select agents uh I can change some settings and uh how many max
attempts are there rack pipeline what is my chunk size what is it I'm using model
uh what model I'm using from llama I can directly pull from here I'm using nomic for this gamma for this gamma for image
captioning gamma for extraction right I'm I'm depending on gamma a lot and I'm hoping that by the time I have uh e av4
uh all local agents are there we don't need gemini also
Okay. Then hierarchal delegation. We discussed that persistent memory. Uh the seeds are already there. I have to
debug, you have to debug. Then we have extreme context engineering. Essentially we have safety protocols for
clarification. We have a formatting rigor. We have a failure recovery. Failure recovery right now is not is something that as I said I'm going to be
pushing you to do it in session 18. and by the time I I will also be done. So the philosophy is that we have a one
year in the future lab. So idea is that we're not building loops anymore. We do not have a for loop a while loop that is
there. We have a graph and graph fundamentally is way more capable of executing a workflow. We are decoupling
the planning from execution. That is also very important. Uh we have to we are factoring our own context. We have
our own librarian who's basically u looking at our memories and getting that
uh data for that particular job and we're treating memory as infrastructure. That's why we have a fully functional
rack that is separate can be used for different applications. We have a remy also running separately that Remy is
like me0ero but we are building our own because if you just install mem zero then you have no idea what is happening
your data is also going out. So network X is the mathematical backbone for us. And why network X is there is some also
something you need to understand. There are three main things that network X provides us. Parallelization. So
everything has a syn a sync execution. Moment a module has uh the data
available it will process. You can't stop it. If you're stopping it, you're actually
disabling the flow. Right? So that's the beautiful part. So moment a particular node has all the data, it will just
process itself. Then you have a state management. uh network remembers what was the last state. So that's why I can
go and edit at particular state and other nodes can also be processed based on that and has resilience. It has a
subgraph recovery. So if a part of the graph failed the other part might still continue it. It's not that the whole
thing will actually fail and you can write an override also that if I fail then possibly read the other node and
then continue right so that also bu gets built in. For example, um you're building a whole user validation um
agent. All documents uploaded Aadhaar document failed. So should the agent stop, you can add a recursion there
where the the fault tolerance says no. If this fails then ask or maybe just continue.
So the key benefits are the data flow and that's why we are picking this. So first as we said paralization is free.
Then we have the state management. The graph is the state that's a beautiful part and the nodes are the context. what
all you uh push through that particular line is the context. So when you're looking at this, you're seeing two
things. You know, you're seeing the agent, but you're also seeing the context. This is the context.
Are we clear? The context is visible. Now
here you can see the thinker agent has one
is coming getting context from one, two, three, four different things, right? All
the context get together
synthesize research data from the current demand data one project demand data 2 and the computer data t3 and
identify the key tense group driver challenge that are possible in the Indian purify market. This was something difficult because earlier we had running
one retriever one then we do retriever two search then we do a search three and somehow we hope that we can connect all
we maintaining everything global schema if the global schema fails then we fail but here because the connections are
there the node names are also very clear and becomes easier to handle.
Okay, now industry comparison. Uh we have a lang chain and lang graph. Uh students always in fact most often ask
why not just use lang graph. The answer is lang graph is a graph engine heavily inspired from network expensible but it
is opinionated framework. They have decided how to use it what gets connected. It wraps the graph concepts
in specific agent abstractions like there's a state graph, there's a node, there's a edge. is great for standard use cases but you can't ex expand it and
that's why we we're building something which is raw right it gives you education clarity how it's done you have
full control over the execution context manager what you want to flow through it what you want for example I've
overridden even though the graph looks like this my formatter agent is been overridden overridden by the full global
schema right because I'm I'm sure that sometimes these fail that's why for the
formatted agent even the query everything is overwritten. So you can go back and override something. That's something you can't do in uh blank
graph. You can't override a default. But because you're writing your own, you can write a override now.
So the high uh high level life cycle is something like this. We have a injection. User sends a query. It goes
to app. py and that's where we're discovering the code.
We have this app. py. This is where the code comes in.
Okay. So the query goes to the app. py which is this.
Okay. Then architecture. Uh this essentially triggers the planner agent.
Planner agent creates the graph which is directed graph dags for us. Then we have
a state in initialization. Basically now the execution context manager kicks up.
It looks at a graph and starts execution. We have a steprunner agent runner multcpn tool. So execution goes
like this. We have a steprunner. Steprunner looks at the node. It runs it. What is it running? It's running the agent inside it. Basically pulling that
prompt and running it. If the tool is required, it fetches the multcp tool and runs it and then provides the result
back as the agent's output to the next node. The context is essentially the
node or the link that we are seeing and we have a summarizer agent which looks at all the nodes and then gives us
output. That's the override that we have written in our code. Stepbystep flow is going to be something like this. We have
the app py and loop. py query analyze these files. Agent loop 4 is going to
check the uploaded files if there are any. Then we have a display agent is going to look at the profile and it's
going to summarize them if the files were loaded and it's going to create a files profile in the JSON. Then we have
AR the planner agent coming up with the original query files profile and global schema. Right? Generally step step one
we have never seen but I think in the next session I can show you this. So right now you're starting from there. But when we're talking about chat here,
for example, if I go to let's say rag
open document. By the way, this is a pure image, right? I can't select this.
But if I go to that and search,
right? So we have a full image captioning also done. But let's say we had this. Maybe this. Okay. I'm not sure
why would that document ever come in. But let's say if you're selecting this and adding to context, right?
So this context uh being sent in initially is what we're talking about
here. So the context could could be the full file and the file first goes to a
distiller. We extract the distal information from the file and then send that. We don't send the whole file in
our context. Gemini can handle it but we designing it for low context window. Then we have a planner agent which comes
back uh with the original query looking at original query the files which are there in the global schema and then
creates the graph. Once the graph is there we go to the context manager and the graph is held by the uh the graph
storage essentially whole graph is held by the graph network x graph and then we go through step by step. Whatever data
is passed or whatever data is given out from a particular node is stored in the context getinput reads t001. Right? So
the graph name essentially itself becomes the name of the data that we have and if a tool is required then the
tool uh the node requests for a tool the tool executes the result of that becomes
the output of that node. So that also becomes simpler the loop sometimes our agent decide uh
self call self equal to true. So now in fact I can show you that
and I hope should be in one of these only.
uh hey know uh so uh so from uh uh session
12's code so uh there was actually use of uh network x so what I understood
from there was like uh from perception the plan graph was created and it was
stored in uh the network x uh um data structure and we were replanning and we
are modifying and changing it so here I'm just a little bit confused like uh what extra is happening here uh at the
state of distiller or uh the planner in session 12 we discuss about the
network x we had that mentioned also in the code but we never used it actually and session 12 a browser agent I'm not
sure why right uh in session 12 and in 15 there was no network it's like uh we did the
plan graph thing manually correct and uh but here extra it brings up like
I'm a little bit confused what it is bringing We have never used network X till now. Okay.
We were so last session specifically was a manual graph. So if attended last session we were
managing the graph manually right and if you have done the last assignment
then you'll know that when you're handling the graph manually then you need to manage the context you need to connect them you need to manage the
state. Yeah. Moment you look at the current code you're going to see that all that code is not there because NetworkX handles
that for us. So that's the difference. Okay, we in case of replanning or
anything, we do not have any code as such. It uh it uh like it does everything itself, right?
No. So, no. So, let us say this is not network X. Okay. Mhm. You can still create the graph.
Mhm. But now manually you have to somehow link the data manually. Somehow you have to trigger
them. This is done. You'll you'll write okay if I'm done then move to the next one. If I'm done then move to the next
one. Something like that. Okay. Right. So you have to write the all of this manually and then
uh basically fall tolerance and everything has to kick in. Yeah.
Okay. Okay. Thank you.
I have a question. Go ahead. Uh, how do you rate Neo 4G as a
framework for creating graph versus uh network access? Neo 4j is
okay one second
database. So the back end basically can create it's storing the graph
uh storing the execution output of our node as a graph.
It's not it's not a executor. So it's a knowledge graph basically it's
a knowledge graph. It's not a execution graph.
Okay. You know have you heard of pyarch? Yes.
So pytor creates this kind of graph okay backation. Okay. So we have
multiple variables here. We do back propagation and because it's a graph the information can flow and then we can
process it. So it is it is a storage and the execution at the same time. Network x
your neo 4G can store this information. Okay not exe.
Okay. Okay. So if I build a graph near using Neo by calling Neo4j and then use
network uh X will that be giving me a superior output versus you know building
the graph manually? Uh no no no you're confusing two things. Okay.
Network
network X creates a execution graph or that's why we call it DAG. Okay. Execution graph. So do this then do this
then do this then when these are done do this and then do this. You clear? Okay, that's clear.
Yeah, it's storing it's storing the execution and it's storing the uh result also or data as well. Results and data
result and data are stored. So query and output both are saved here.
When you say neoforj you're just saying once the graph is done I can store the
data. So data data it's not execution it's just a data neoforj
virtual knowledge graph basically. Yeah it's just a knowledge graph basically. Okay, thank you.
So not required redundant here. But if you have some other use case where you want to train a model on top then
probably you can extract all information from here and move there. Got it. Okay.
Okay. So multencp we already know the new uh the only code that you have to probably look at is execution code
context manager which is literally uh uh a wrapper around network X. That's the
only custom code that we've written. Right. So the input is a raw string goes to app. py planning comes back in JSON
from Gemini and goes comes from the planner agent. Orchestration happens to
network X automatically. That's a graph object. That graph object is the execution uh code as well as the data
stored for us. Then the output if a tool was involved is a JSON schema where do a
std out. The agent output is also structured JSON and the final result is markdown in case of us. final result we
can convert into an app or send it to someone else also. Now a very simple example how the browser flow will work.
Now in case the browser flow was there or we were doing a browser based query then we would have called web search in
between but everything else would will remain the same. The logic remains the same as we had last time. We are using
duckco. We are using uh same playright for our search. Uh we have five engines
black duckco bing yahoo eosia moji. So if one fails we go to second one with a code to third one and fourth and fifth
and if you're using uh the code that I shared in session 11 then we already
have fast scrape headless browser and triple extract we trying to use traffic liter if that fails we have readability
if that fails we have beautiful soup so we are trying thrice to extract the content that's why uh if even if a
website doesn't
I broke it. Okay. Sometimes the websites fail archive.
Yeah, you can see all JavaScript and everything is broken. But fortunately
No, it's not letting me. You can see that, right? Even after three attempts, I failed here. That's that is what we're
talking about here. Even trad all three failed. So, we're trying as
best as possible uh to extract this. The reason uh your Gemini or OpenAI don't
face this problem is because they have scanned every single website and stored the data. They have the whole copy of internet. They keep crawling. So, we
can't we can't manage that best. Okay. Okay, so the end to end data flow is
going to be you have a retrieval agent for the browser case uh where it may do a web search. It may call web extract
text directly. So web search is get the links. Web extract text is go to the link and extract text and then marks the
T01 as complete. Right now important question on the rag and this is where I want you to improve it and this is where
I showed you this feature also. So if you go on rag and click on rag and let's say search dhi it should not work but it
works for us right? It's there inside.
Okay. Oh, I removed a document. It won't come
down for example. Yes.
Now you can see if you see I'm making this up
then we
right again. So the reason that is working is because user expect it to work. People may ask a very sim so look
at this query for example uh find all
documents where reve is mentioned. Now if this kind of query is there what will
it do? rag will fail because we may not have a document that has that kind of query right but here in this case I'm
expecting it to give me something and here you can see we also fail so this is
where your rag is what do we mean right now we are on a classic vector search phase plant basically means that we are
we can only do vector search so when you just search for a query like unmole it
is not going to give you anything and if I don't implement what I just showed you it will just find HR documents ments
because the name looks like uh Indian name and HR document what I had in my
rack had few Indian names so it looks like okay I need to pull that up that's not what you want your rack to do that's
not what user is also expected especially in the professional case so this is what people do you need to
implement a hybrid retrieval top k and then implement a top uh key preserving
filtering for the quick win you need to do a quick heristic or lightweight NE
which is named entity recognition or you want to do BM25 and embedding and fusion RF. This is what I've likely implemented
and I'm I'm going to continue proving this. This is what we will discuss more in next session by the way. Right. And finally this is a production build by
the way. And finally you need to get an LM which validates whether the search result is what the user wanted or not.
Remember today agents are very cheap very very low cost. So you can actually use a small even a gamma to make sure
that the query was this this is the chunk I'm about to send. Do you agree or not? So what I will recommend
you should right now be uncomfortable with something like what just happened here right no document container we
exactly so but it search for okay because
document mentioned unve is not there
why did this came okay I search why that didn't
capital interesting very interesting I'll search I'll check why this is there right
because I know I fix it but what's the issue I'll check this very interesting by the way yeah so that's a
uncomfortable you you will not be able to even do the small or bigger one in your case so the blunt truth is the
keyword must appear in the uh data when what you're sending. So that's there, right? Otherwise, it's not going to just
work. You need to think of it like a bouncer or a DJ that is going to be finding the right detail, but like a DJ
can mix things and detect and provide back. You need to detect when the query has a lexical intent. Not every query
needs a literal match, but some absolutely do. For example, if the query is asking for a name, for a email, for a
phone number, for ID, for a quoted phrase, find document mentioned, where is written, etc., etc. In those cases
you are going to be finding the rag is going to fail but you are going to push for rag. User is going to ask LM might
ask such questions. So we don't want to fail there. So you need to classify a query into a lexical which is like
required must match lexical preferred bonus signal or semantic no lexical
constraint. Now how do we do this? Anyone
entity search? No llm again. Llm
remember it's cheap now so use it. Let me show you. I hope
that classify queries in lexical
query.
It will give me a long answer. I need to Yeah. See
you get what what I mean and to stop thinking of the whole
agentic system as something that we do a rag we get result in one step no look at what cursor is doing or what anti-gravity is doing moment you ask
something it goes into a long thinking in fact charge GP right now if I ask am I married it's going to like think like
15 minutes before it come back and say yeah I think you're married you have never told me but your questions are like that So you'll need to make sure
that you're spending enough uh of the smaller models to get such a result. Now
moment I have a lexical required I know that I'm looking for BM25 kind of search right apply a smart gating filter for
lexical you can retrieve the top key using vectors high recall we can add a gate at chunk level not the whole
document we can allow the extract normalize and tokenize for soft magic right require all tokens for names like
unmold sing otherwise sing alone won't match because sing there are like half
the people in the country have sing in the name right so we don't want that also If the gate removal removes
everything, return no extract found. Very important to go on the front and tell the user that I have a very low
confidence in document. I'm sending it to you. Now, this is very important. Add PM25 sooner or later. We'll talk about
it more in the next session. But this is something that is uh sort of I'll say industry standard. Everyone uses it
including your OpenAI and Gemini and cursor at the back end. This is going to solve your problem cleanly without
brittle rules. uh the code I'm show showed you that has PM24 already not the
one I'm sharing with you that's the assignment uh lightweight entity detection uh coded strings emails and
phone numbers use LM validation only as the last mile right if you use LM then
make sure that it's the last thing to check on the final result filter that you have so strategy I will pick phase
one lexical intent detection plus skating plus onyx UX phase two BM25 plus
dense plus RF phase 3 entity aware indexing and optional verification. This
is where you should be by the end of today's assignment. In the next assignment, I'm expecting you to build a BM25 tense because we are going to talk
about Remy and rack there more again. And the non-negotiable UX rule is that
you need to mention at the front no document mentions unmolding exactly that's why my document came in and said Ranir Singh, but I need to make sure the
spellings are not capitalized or other things. Okay. Now, here's a long assignment section. So the code I'm
sharing with you of course is not the full code. This is the code I'm sharing with you. No front end.
Okay, you don't see any front end. But if I show my code to you,
it looks like this. It has the platform front end and all my
code lives inside the platform front end. Right? Rest everything I've shared with you here. That's the back end
that's there. So you need to start working on your front end because you need to come up with uh what is it that you want to build in your capstone and
what kind of UI you want, what kind of features you want. I'll showing you what I'm building but you need to come up with your own application because the
next five sessions is your capstone extending to uh two or three more weeks from there. You need to come up with a
cool implementation of how you want things to be done. Okay. So there are some bugs and some fixes that are
required. the critical bug red is there right now and I'm leaving the bug as is
because it's going to cause a particular kind of failure. So you know how to fix them and you work with anti-glavity or
cursor to solve them. So the stringified list right now in the memory in the context of py you need to add a fix
called ensure past value method. Why? Because a lot of times lms and APIs are
going to often look like this. Now again this is not a problem with Gemini 2.5 or
3. This is a problem with Gemini 2 or GMA for example the smaller models that
will may not be able to completely understand this. So when your LLM or API is going to uh return a result you are
going to read the URL like this. This is a URL then this is a URL then this is a
URL then this is a URL and so on. We don't want that right? We want to read the whole www.artressplatform.com/theblog
of 20 20th century. So that's one bug that you have to solve to make sure that you're pass your LLM is passing giving
you the results and you're passing it properly. Second, you have a critical blind formatter bug in the loop. py
you need to explicitly in uh inject all global schema to the formatter agent. I told you I've done it in the code I'm
sharing with you. I have not. You need to explicitly enter it. Now why? when
you're going to run your uh flows in the code I've shared, it works by the way directly without the UI. You just need
to call it manually on the
Okay, I need to
There's no okay I think removed everything and then given that
you
okay because that is shared code I anyways can't run it because my in key is also not going to be
Uh browser is not there. That's fine.
Yes, this is
to tools. Yeah, right. So, this one is anyway is not there, but we can fix this one.
This should be in the config file.
Yes, you need to change the path for for these two, right? So the all global schema is not
explicitly added. You need to add that. The third one, the infinite spinner. So
right now when you uh if you were to ever connect the back end with your own created front end, you're going to see
that your state is always going to be saying running or infinite spin up, right? because
the planner agent takes some around 10 to 30 seconds worst case and your screen is going to just show blank at that
time. So you'll have a infinite spin up and uh the front end is going to crash thinking that I'm not receiving any
data. Are we clear? Back end is going to be slightly slower compared to what your front end might think. That's why you
need to make sure that uh you have some sort of connection from back end to front end telling the front end hey wait
don't worry otherwise it's just going to show infinite or show a failure. That is not a failure. It's something that the
front end has to wait. Now you need to start thinking on the front end back end.
Okay. Now we we have an infinite loop warning. For example, inject a warning prompt on turn equal to max turns minus
one. Whenever you have uh just one more thing left, you need to make sure that
you're informing uh that you're hitting the limit. Right now my limit is 15. Basically I have 15 turns uh for my
agent. Mostly it's done in one now because my internet search has become much better. But if your network is
showing or sorry if your uh log is showing that no output produced
then make sure that you are telling to the summarizer or you're telling someone that we have reached the end otherwise it will just exhaust all the runs that
are there. Now in the memory right now you need to save rich context which is a
question plus answer because agent should know should I deploy? answer is yes. Then in case of uh the data that
you're going to be storing, you need to mention the user response for yes, right? So the next agent can see yes.
Yes to what? Not just like the a the user said yes. We we are describing
clarification agent. By the way, the logic right now is you clarification
agent is going to come up. It's going to ask you a question. Hey, do you want this or not? You're going to say yes. Clarification agent is going to say yes
to the next agent. that is contextless right clarification agent should what I
ask a question and this is the response to that so that's what we're talking about making the context rich then some
sort of robustness you need to have a three strategy execution why now I'm calling this S20
because this was S20 code in the last session uh in the last course but right now it's S15 so we have pulled up the
overall u schedule to explain what how things are happening otherwise this
would be five six session So right now did a code execution produce a variable? Uh is a JSON output
correct? Is it hidden in the final answer? These are the final things that are there. Right? A common fallback.
Basically this prevents a pipeline from baking just because an agent put the answer in the wrong JSON field. That's why you need to make sure that all of
this data is being sent to your final uh formatter agent. Right? So that's why
we're calling a three strategy extraction. So did a code execution provided result is the output JSON or is
it hidden somewhere? All of this is something that uh may not be programmatically
extractable. So provide all of these three to your formatter agent. There are some critical logic fixes which you must
implement in the context list as a string crash happen a lot. Your LM is going to provide you uh basically the
four things we discussed above I mentioned here. L is going to provide you urls which may come as this and you
might end up extracting like that. We don't want that. Then we have a blind formatter global variable research
summary are not passed to the formatter agent. So we'll fail. So pass everything formatter agent. Then we have a zombie
hang UI might freeze for 30 seconds because planner is thinking UI UI might think I'm expecting something from the
back end nothing has come it will fail. We don't want that. We have infinite loop where agent will continue till it
actually reaches the token limit. We don't want that also. So halt your agent faster and inform someone.
MCB server upgrades. Uh this is something I've already done and shared with you. So the three files I've shared with you, they have a lot of upgrades
already done. So but some stages are still required in MCP. The configuration is hardcoded
dictionary. You need to convert that into MXP config or MCP config JSON. Uh
Git support there's none. But I've added a git support and uh you have seen that for example in the MCP I can add a new
git. There used to be a new button here. Yes, I can add a new MCP directly from
here. That's upgrade you need, right? Required caching. I'm not c uh currently
we're not caching but I can't keep on adding for example Yahoo Finance every time, right? So once I add I need to
cach it and it actually gets cached into my local uh
Let me see if you're caching in your code also.
No, you need to add that. Yes. So that's a assignment, right? So what's the assignment?
Assignment is that make sure that you have a five basis caching of the new MCP agent that you're adding and of course
time out. I've increased to 20, but you need to make sure that it's implemented right now. Default is I think five or 10
seconds. Okay. So we have a server rack. This is the heavy lifter. Pallet processing is there already. And uh this
is the basic code shared with you. This is where you want to go. So pallet processing thread pooler is there. Maximum two workers to ingest files. Add
smart semantic chunking. We have already added that. Uh I've updated the code to make sure semantic merge is three to
four times faster. Okay. Uh one key comment. This is our next session. So
this is a todo if you want to do. So in the next one we are doing parallel processing. um improve the chunking by a
lot. Then we have threat safety and then we have image captioning that is much better compared to what we had earlier
and we'll see why. Okay.
Okay. Uh to the coder agent you need to add strict environment constraints. to the planner agent you need to make sure
you're adding a data directory where is the data actually saved and in the apps.m MD new files not related to you
unless you are going to be making a new app file matrix is simple yes and please
remember this is the last time I'm sharing any code with you are you clear
this is the base of all the code that we're going to be building this is the base where whole network X and
everything is structured together. I've shared already a code with you where you have something like nine or 10 bugs. You
need to fix that to get to a state where the current assignment can be done. And the fixing the bug is the current
assignment. In the next one, we're going to be as I said taking next step and fixing this up and the next one is going
to be further taking us to u the remy part and context engineering. So each
new session from here onwards is going to be a delta upgrade on what we have earlier. And finally you need to end
somewhere where you can actually pull off a big capstone project. Any questions?
Uh Nita. Uh hi Rohan. Um so I have a few
questions here. Uh you mentioned S20 prompts right? uh like in prompt
engineering uh can you uh uh explain the ninth step a little bit more
below below nine uh whenever you mentioned S20 is it
meaning like it's it'll be done in session 20 or what is the expectation here I didn't expect
your session your session 20 is a capstone okay so and this is the last code I'm sharing
with you so to be able to attempt the session 20 capstone this needs Huh? Fixed.
Okay. Okay. Okay. So, uh now this uh um
for this assignment after we fix the back end uh is it necessary to have a front end built or can we uh run this
project headless also? You can run the project headless but that means your S20 capstone is also
going to be headless which probably is the wrong idea. Okay.
Okay. Thanks. Because ultimately we like to show some show something to people unless for example you're working on uh
we had a team from RBI last time they worked on security threats and they never needed a front end so the problem
was completely back end okay one more thing uh one more team which were working on the network uh attacks
they also never needed a front end your problem needs to be such that it
doesn't need a front end okay so uh do you have any samples of
other front end or uh or is this the first time you're doing this?
I showed two of them today. Oh, yes. The last uh
and also which uh front uh um are you using cursor or uh anti or how are you
building the front end? Uh your program looked really smooth. So just asking uh
I'm using uh anti-gravity. Antig Gemini is really good in uh this one.
This is the one I built in the uh EG V1.
Yes, you were saying we would be working with this. So we will not be working with this any longer. This is what you are working on. I
changed the UI. Earlier we had this. Now I've changed the graph layout.
Okay. Right. Here I'm adding a human in the loop. Basically editing the same uh
apps. Okay. Same session but here I'm only showing
the uh output result. Now I'm showing the whole graph and output result.
Okay. So this was old style. Now I'm making it
way more modern. Okay. There's a coder agent also. So slowly we
going to add the code but whole back end still works without inter. Okay.
Can we get this URL for this video so that we'll get some idea on the front end?
This URL this is the old one. Mhm.
I'm pasting it. Um, if you want I can uh So I' I've taken you through the whole new UI new UI today, right?
Okay. So you have that in the video already. Okay. Sure. This is my new UI.
Got it. Okay. And what I did, by the way, my old UI looked like uh I need to kill it
again.
Uh Rohan, Mr. Um so the front end that you have done
is very smooth right? So um is it possible to share any skeletal of this because adding more features to uh such
uh framework would be easier rather than starting from scratch. So I wanted to
know your thoughts on that. Not possible. Okay. Not because I don't want to. It's like
it's not possible.
So this is the one I started with. This is the one I shared the video also for. Right. This was the old UI.
So UI is basically a CSS file. I can share the CSS file if you want.
So I took this UI. So design anything. For example, I took this UI. Then I went to Midjourney. I have an account on
Midjourney, but you can also do it free dashboard.
Then I'm telling you literally what I did.
Then I pic literally picked this image, copied it, gave it to anti-gravity and said I want my UI to be inspired from
this. And it came up with that UI. So design anything you want. Make sure
whenever you're designing you're telling uh
you can see same UI sort of stuff everywhere, right? It's just a simple change from
where this was and where the current code is.
This UI became this UI.
and and yeah so you need to define it properly you need
to say that I have these many tabs I have these many things. Uh one important
thing uh whenever you're talking to any agent or any uh system to make a UI for
you, you need to mention
for all CSS. Moment you do it, it's going to make sure that you have a single index. CSS
file from which it is actually pulling things up. And everyone is using Tailwind. My my UI is also based on
table.
Okay, we have a question. We have SH.
Hi Ron. Sorry, a simple admin question. Actually, I seem to have lost access to the course in the canvas. Log from all
of your Gmail accounts on your system and then go to Canvas and then log in from Google there first and then log
back in Google then nothing nothing I can do. Okay. If you fail
seem to sudden Yeah, I'll try. I'll try. Yeah, I emailed I emailed admin but okay
if that's the trick I'll try. Yeah. Yeah. It's the if you fail in everything what you need to do is to tell us that
you have failed we are going to send you a reinvite. Then you have to relog in and recreate the whole system. Sure.
Sure. Okay. I'll write it. Okay. Sachin. Yeah. Rohan. Uh in this u um workflow uh
does it run a dynamic UI or you just have a static template and you only change the payload and then just
changing the payload apart from this apps. This is dynamic. This is dynamic.
So in this case in the app's case I think this all these components are uh are designed on the fly by the Gemini or
is this? No. Uh I picked a uh strategy. So you have you heard of I
forgot what is it called? Uh
I'm forgetting the term. Uh there is a you can just import a component. You are
from front and back background. No, I'm mostly on back end but I know a
little bit of front end. Yeah. Anyone uh you know you know do you guys know there's a single line of importing a component what is it called?
CDN what CDN sh CN what I've done is basically I found
really cool shard CN components and ask Gemini I want them. So every new component import for me is just a shard
CN component. So if you like any component anywhere just take a shard CN and give it to your uh and it brings those components to me
basically. So you have so you have copied the shad CN library. Exact not copied the shad CN library.
Shain components the component I like from different different guys. So I p pull pull those up.
Okay. And what is what is a shad scene component? Just a JSON file, right?
So if I show you actually each component Yeah, just I think just a JSX file or something like that. Yeah,
correct. So component for me for example a graph. Uh not this.
Yes, these are just simple simple components. Oh, okay. And it just selects one of
them based on the parts. Okay. Also, uh how do you get the ticker in your in your graph? Uh sorry, in the rendered
workflow. Uh I mean when the node is actually running, it shows a ticker, right? Something of the sort.
Which ticker? Uh I mean the sliding Yeah,
again a component this thing. Okay.
and it state is enabled only when it's executing something on this one. Yeah. Okay. Okay.
Uh one basic question. So what do you mean by like it is not possible to
share? Uh I didn't get is it um like it's a JS application or is it
uh built on some other framework? Uh repeat again. Uh you mentioned like it is not possible to
share this uh UI, right? Uh is it like uh built on some other framework or it is IP of Rohan right? I mean you
can't share no no not because of IP. The problem is that how do I share the UI with you? UI
is a index.t CSS file. I can share that with you. After that then you have the layout. After that the layout is
integrated with the back end. So I have to share the whole application to share the UI with you. You understand this? For example, this planner agent
everything nothing will come because that depends on what node we are selecting. For example, each node selects different inputs and different
outputs. For example, here it selects overview. For retriever, it shows web. When I go here and select this, this
layout is different. When I select this and go here, that layout is different. So all all are dynamic. So unless I
share the code with you, full end to end code with you. For example, this opens this box again very different from what
we had here. So I can share the CSS with you. CSS is going to tell you that if you were to open a node, if you were to
open a side box, how will it look? Okay, but this is literally very easy. You
have uh take a screenshot of this from the video, give it to your Gemini and ask it to create it. It will create it. That's better because it will be at your
end and you can link to the back end. Okay. Okay. Thank you.
Let me show you one more thing. Uh how do I crash it? I don't know.
Rohan, are you planning to make this open source our ar our tourist platform?
I'm planning to actually extend this way more where it is currently and uh hoping
that um and these are thoughts. I'm hoping that I can invite some of you for
the capstone to implement features in in Arress itself and then launch it. launch
it as in make it open source and make it available for people. Okay.
Yeah, I don't know how to catch the back end right now. But if I crash the back end, you will not see anything here.
All right. If you don't have anything else, then I'll see you next Saturday. If you have something then I'll still be
here. Hi Ron Srther here again. Uh I did try that sign out thing. Didn't work. So
I'll email again admin uh to send the link. Again going to send you the same canvas
link. Uh you need to sign out from all Gmail clear a cache and then try.
Yes. Yes. Did you sign in using uh Gmail and password or directly Gmail?
Uh sign in using direct Gmail. Yeah. Yes. Then there is no way we can set the password also, right?
Yeah. What is basically basically it is saying I mean
I don't have any courses. So that's the issue. So cash is wrong. You have somehow logged into something else.
Okay. Okay. Yeah. I'll What is your email ID again? Uh S uh uh S for Sridar and my surname B
Y R E K A. S B Y S S B Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y
Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y Y R R E E K Agmail. S
again. Sorry. B D. B for boy. S
Y B for boy. Y R E E K A.
Uh it's not coming up. What is the name? Yes. Last you logged in on 25th of October.
So it's a cache that is wrong and your cash is not letting the uh Gmail login. Okay. Okay. Cool.
Again resending the invitation which the admin would have done. So it's checking email. You should get a link there. When you click it, login through Gmail. If
the same thing happens, that means we need to get rid of the cache. Sure. Sure. Okay.
Uh, I want to build a local
uh uh app using this thing wherein I want to pull the data from the power this uh fabric uh you know uh data lakes
and uh and expose that to the agent. It give me a risk. Basically there is some concept which I want to build is that to
you know expose to find out the risk and uh you know of uh lot changes. So I want
to figure out is there any you know writer available as to how do I get that data from fabric
and