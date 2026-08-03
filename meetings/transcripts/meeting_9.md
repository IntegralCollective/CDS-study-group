# Weekly Meeting 9 Transcript

**Lukas Orsvärn**<br>
All right. Hello, everyone. Welcome to, is it the ninth meeting? I guess so. Welcome to the ninth meeting. In this one, we don't really have a very strict agenda because we're just going to keep working on the... study group that we've been having going on so it's mostly going to be down to what people want to talk to and if people have problems if there's stuff they want to talk about and so on so yeah i don't have much more to add than than that actually so I'll just right away ask, does someone have something they want to talk about that they feel is important right now for the study group? Otherwise, I have some stuff we can go through.

**samw**<br>
We could talk about the module 3 that Markus put on the GitHub.

**Alberto**<br>
Yeah, I would be up for it.

**Gary Kent**<br>
Did you update something there? I missed that.

**Lukas Orsvärn**<br>
Yeah, I'm not seeing anything.

**Marcus Barrick**<br>
Yeah, just... I did a couple folder requests this morning. I, like, accepted them now, so that's why maybe you're not seeing them.

**Lukas Orsvärn**<br>
Oh, you merged it? Yeah. Oh, okay. All right, I'm going to stream my screen so we can all look at the same thing.

**Marcus Barrick**<br>
It was still largely just a simplification, a rehash of the white paper. But I did have some questions, if that's maybe relevant to look through.

**Lukas Orsvärn**<br>
All right. Yeah, I didn't know this was in because I guess it slipped past me if it was merged pretty quickly. Yeah, we'll do that next time. So does someone have any comments on it immediately or who have had looked at it?

**Gary Kent**<br>
It seems to me that we're working directly on the main now. So if we have to make any changes or we want to suggest changes, it's going to happen there. We don't seem to have a developed consensus process for changes that we're making.

**Lukas Orsvärn**<br>
Yeah, we don't have a consensus process, but we're also not really making decisions about stuff in that sense. Like anyone is free to go in and make a new pull request that makes whatever changes to this one, for instance. And Marcus said that, yeah, he's not going to just merge it to main immediately next time. So that would be easier than to... have a discussion about it if there was a pull request for it. But we can just open one for it and talk about it there and make changes.

**Marcus Barrick**<br>
Mostly just pull this one in because, like I said, it is largely just what the white paper says. And just zooming out, I'm curious. I know it's just Markdown file. I don't know if there's a different way we can do some object-oriented coding so we can at least point to the same object instead of just using the Markdown notation.

**Lukas Orsvärn**<br>
You mean in terms of linking to different things and stuff?

**Marcus Barrick**<br>
Yeah, module 2, it says outputs, structure, issue view, and then module 3 inputs that. But if I could actually refer and point to that object, it would be helpful as we expand this more and more.

**Lukas Orsvärn**<br>
Yes, you can definitely do that. I can show you. So you want to link, for instance, module two to something. You can just do square brackets around it. And then you can link to stuff that's in the same folder. So show it just to module two underscore two dot md. And I think this should work. If I preview it, it looks like that. And if I click it, I middle clicked it. I get to module two. So it's just a.

**Marcus Barrick**<br>
But if we were to actually create a structured issue view as an object, which would have more information, it would almost be like a function or a subclass within module 2.

**Lukas Orsvärn**<br>
A structured issue view. Can you expand on that?

**Marcus Barrick**<br>
Right above your cursor that says a structured issue view. That's the object, basically. And so you can do maybe that same link there. But I'm just thinking if we actually make that an object, which would have properties and stuff, It'd be easier to structure issue view dot whatever function or property.

**Lukas Orsvärn**<br>
So you're saying this is treated more like a programming thing, where this is the name of a struct or an object, and then you list what are the things in the object. Is that kind of what you mean?

**Marcus Barrick**<br>
Yeah, I don't know if that's feasible for us to do as a skeleton code instead of just Markdown.

**Lukas Orsvärn**<br>
Yeah, we haven't done that in the other ones because it's a little bit more high level what we're doing here now. But maybe that would be desirable. The thing that I don't like about doing that is then we get really into the weeds and need to be very specific and have a lot of information that don't really help necessarily give a better idea of how everything works together, which is kind of a big point of what we're doing. But maybe someone else has some thoughts as well.

**samw**<br>
About that specifically or about module 3?

**Lukas Orsvärn**<br>
About that specifically, yeah.

**Gary Kent**<br>
I've been thinking about it or trying to think about this from a data perspective. And I have a question about whether or not this whole program, the integral itself, the integral system, at least some of the specifics and some of the modules and the subsystems that I've been looking at, whether they're actually programmable at all in terms of coding.

**Ben**<br>
There are. And it's not easy, but they will be.

**Gary Kent**<br>
Well, I haven't become convinced of that, especially looking at the FRS module. But even in the CDS we've been working on, there are a lot of things like scenarios. How is that generated?

**Alberto**<br>
You mean the bridge step, right? 3.5?

**Gary Kent**<br>
Yes.

**Alberto**<br>
It's not specified in the paper, so it's kind of like a black box.

**samw**<br>
But I think. No, I think scenarios are also proposals in module one too. And then there's more scenarios, more proposals generated in that bridge step automatically. But you don't even need that bridge step really because you have manual proposals in module one.

**Alberto**<br>
But I think this automatically, that's the thing that needs to be addressed. Yeah. Yeah.

**samw**<br>
They're alongside the manuals. It's not like they replace them. You could completely take out that bridge step and IntraBowl would function just fine. It's just not a necessary component. You probably do need to figure out how they're automatically generated if you're going to have that. But the whole project doesn't hinge on figuring that out. You could delete that step and IntraBowl would function as normal, I think.

**Alberto**<br>
I would agree with that, actually. Although, I mean, that's what three, it's a context model, right? So it's kind of like just logical to expand the scenarios that are already there or to create new ones. I understand the step, right? But yeah, I would be, because I'm not that versed in IT and stuff like that, I just don't know if something like that is feasible at all. So that's, I'm on Gary's side, although I must say that I have no idea

**Marcus Barrick**<br>
no expertise in this yeah me too yeah i think the challenge is like the a contextuality of it like it could be for like water sheds or nitrogen or any other thing so i think like at least having your mind set into a certain context would be helpful but i think like yeah so how do you make an object that's like Domain, like, general, and then how do you actually automate that? So that say, you're tracking water flows or nitrogen or anything like that. How does that actually, like, feed into the signals or, like, the capacities to actually, like, lower the capacity? I think that's where it gets challenging for, like, if it's actually automated.

**Gary Kent**<br>
See, that's why I think that one of the things that's specifically stated in the white paper is that for the test, for this minimum MVS structure test that is one of the primary goals of the first stage, that we need to have a complete data structure set up, a complete architecture, a complete schema of all data that's going to be used even when we use the full model, even when we do it just fractionally in the MVS. So that means you have to understand all those variables in not just the example context that they were given, but in all other contexts that might occur. So a schema or possible outcomes that are affecting any particular decision have to relate to every decision that the CDS might be required to to decide about. And that means not just the nodes, but the proto nodes and all the other aspects of this model that are going to exist as we move towards having full nodes and a federated system that's more inclusive of all the nodes. So it's a huge challenge. I mean, it's so abstract. I don't know how we would define it.

**Alberto**<br>
Yeah, I know what you mean. But I think also Peter mentions that it has to grow organically, like it gets to a complexity level that is manageable. And at some point when it's not manageable anymore, then we have to invent it. Like we have to do this extra step to... But you're right with the thing that we have to keep um, the whole structure in mind, like the, the, the whole base structure, like this, this, we have to, um, we have to assure the, um, how do you say the, um, the architecture. Yeah. Yeah. But, but, but I mean that it is kind of like that, that it can be, can be scaled out that it's a recursive thing. Yeah. Yeah. We have to keep that in mind. Yeah. It has to be similar. It doesn't have to be equal, right? With every new complexity level, but it has to be similar and it has to be kind of like, yeah, related to the level above, to the sub-node, yeah. But yeah, that's super theoretical, right? So for me, I just think we have to get an MVS ready, a minimal viable system, and grow from there, right? But I think it's still very important what we are doing right now, going through every module, yes.

**Marcus Barrick**<br>
yeah I think like high level like not having all decision making processes like narrow down to just the the number of money um I feel like it's a little bit what module three was talking about because it has like a a score vector if it was called scroll down a little bit there's like a context score vector so like i'm thinking as the very first like level instead of just like being money as your only metric for like decision making it has like it's still just like a score vector so like a very reduced thing that just shows you almost like a uh snowflake graph if you've ever seen one of those that's how i'm envisioning it but it has like a in ecological resource labor and social fairness. So like I feel like an NDS is kind of just seeing that. But then if you really want to dive into it more than you're actually looking into the different real world values and units of what the ecological resource is.

**samw**<br>
Module 3 is about constraints, right? That's the main takeaway, that it's about establishing constraints. There's a few other functions of it. But when I read Module 3, my takeaway was that it's establishing constraints for Module 4 to test against, very broadly speaking.

**Marcus Barrick**<br>
I thought 4 was constraints.

**samw**<br>
Well, 4 tests.

**Alberto**<br>
scenarios against constraints but module 3 establishes the constraints i think yeah yeah the whole data is retrieved in module 3 and module 4 is just like a gatekeeper yeah just and that context score is like a constraint score basically You can go ahead. Please, you continue.

**Marcus Barrick**<br>
It's basically like whether, I don't know if you're saying constraints isn't like we have this much labor, and then this is a project, and this is how much labor it would cost. Then you're seeing if that fits within it.

**samw**<br>
Yeah, like resource availability, that being a constraint, the amount of resources available.

**Lukas Orsvärn**<br>
Labor availability, yeah, that too.

**samw**<br>
And it's kind of ambiguous to me if it also, I think it does collect the needs for a particular scenario. You could kind of see that in there, but it barely talks about that. And I think that it must be in there because if you look at module four, it's weighing the constraints against needs. So I assume the needs are gathered in module three, but it mentions gathering needs like once. And that would be an open question or an ambiguity I would want to bring up, which is, to what extent does module 3 gather the needs for a particular scenario? And is that just immediately put into module 4? It seems very vague to me.

**Alberto**<br>
What do you mean by needs? Do you mean the signals from all other systems and inputs?

**samw**<br>
I mean, like, Module 3 definitely tries to determine resource availability, how much resources are available for a particular scenario. But the question is how many or how much resources are needed for a scenario. I assume it also does that, but it kind of dances around the issue.

**Marcus Barrick**<br>
Yeah, it felt the same, I guess. I kept wanting to be like, oh, OAD should come into this because it says it gets ITC and FRS data. But I'm like, shouldn't OAD be like, this is what it would actually take to do this issue?

**samw**<br>
The interesting thing about that is it mentions the OAD way earlier up as being part of Module 3. And then when it gets to specifically talking about Module 3, it completely doesn't talk about it at all. So I wonder if that's a mistake or possibly if OAD feeds to another subsystem and that subsystem feeds that data into module three, and it wasn't a mistake.

**Alberto**<br>
But that's not clear to me. I read it as a mistake, actually. I thought OAD is surely in module three.

**samw**<br>
Yeah, I think it's page 24 where it links the OAD to module three of the CVS.

**Sabrina**<br>
I think I have it open here, and it says when it has existing OAD templates. But maybe if there aren't any, then it doesn't come into place.

**Gary Kent**<br>
Yeah. That's part of what he seems to be doing is he tries to do this minimal viable system at the same time that he's trying to describe and add the functionality to the entire system. And the data structure is the architecture that makes the whole system compatible, which is actually what creates trust between nodes, which seems to be the fundamental aspect of what this is. I mean, basically, that's what the monetary economic system that we exist in right now tries to do, is to create trust between people so they can interact with each other in some way.

**Marcus Barrick**<br>
Yeah, and that I'm not note I was like. Thinking about it kind of needs like either a prediction or like a commitment thing which I haven't seen anywhere in an integral and I I think it's kind of relevant to trust or like I'm committing to to building this thing for awhile and yeah, I don't know if this is kind of. Maybe outside the scope of our questioning, but I'm curious we if anything like that came up for you guys with.

**samw**<br>
Sorry, what do you mean?

**Marcus Barrick**<br>
Just within ITC, I'm just thinking of the engineering planning aspect. And you would need a commitment or a prediction for how long something would take. And I think that just points to Gary's note of trust or accountability, this kind of stuff.

**samw**<br>
That might be implied in the constraints that module 3 is gathering.

**Gary Kent**<br>
Can I make a suggestion? Please. I'd like to hear, I know I would like to share my own perspective, understanding at this point in time from the broadest view of how these modules interact with each other, how these subsystems interact with each other, and what is required for that to happen appropriately. I'd like to hear what everybody else thinks right now.

**Alberto**<br>
i i think it's it should be a pipeline um that has also branching that also branches out and merges again or or feeds back i think the feedback i think it's the better word for it um like if i would say in general or what are you asking specifically gary

**Gary Kent**<br>
Well, maybe I should outline what I think is going on first, and then people can comment on that or say they've got a different perspective on it or whatever. But we have these five modules. They have certain data records that they particularly... Own is the word that's often used in the white paper. Certain modules own certain data structures, certain, what's the coding word, the programming word for that? I'm terrible with vocabularies. But basically, it seems to me that there have to be... With each module has to have also the capacity to store permanent records. And the permanent records it stores is the records of all... records that it's responsible for. So an OAD, OAD is, you know, the design module, the designs are one particular set of data that it's going to be stored in that, in the OAD. But then there are other sub-modules of data that are also stored there that are used to in relationship to how OAD processes information and stuff. And every module has its own set of records, its own set of permanent modules that it commits to, records to, and all of them, all those permanent records from all five modules can be called on by other subsystems at any point they're needed, including the FRS, which actually acts as the bridge between nodes eventually. And this is also true for interface nodes, pre-integral nodes, proto nodes, I think they're referred to a number of times. They work the same way, but they have to have the same data set that they all access and they all use in order to create a level of trust, not only between modules, but between nodes and between federations. That's at least how I see it at the moment. That's how I understand it.

**Marcus Barrick**<br>
When you're talking about storing data, I guess it'd be good to know what context you're thinking of previously done projects or ecological data. I'm not sure how much of that is actually getting stored versus just being pulled live or something.

**Ben**<br>
There's two ways to look at it, I think. And you can look at it from the back end, like the database part, or you can look at it from the front end, like the user interface. I'm interested lately in the front end and what that would look like. How do you people envision, like when you're looking at this application, what do you see when you're looking at it? Is it going to be like interface where you can say, okay, this is what is needed from me and this is what I can get from the system? Is that the kind of thing?

**Gary Kent**<br>
It's going to be interface probably through something like a cell phone that's going to have this app running on it or the cell phone app for integral running on it. And you're going to make proposals or present problems or suggest situations, or look at things like your ITC, whatever you have in ITC credits, because that's going to be related to what resources you're able to interface with while you're interacting. At least that's how I see the front end of this. So it's largely going to be subsystems interacting with each other. And that doesn't always mean just computers talking to each other. It means sometimes the people that are running a cooperative in the COS are going to be sending information to other people or to maybe making requests or suggestions or observations about something that's not going properly, asking for a decision from CDS. All kinds of things like that happen. So, there's people involved in this at a lot of different levels. And I'm even thinking there may be more than is apparent on the surface. I know at least within the cooperative models, people are engaged in those things directly, participants. And in CDS, participants are directly engaged. Whether that's happening in the other three modules is a little less clear.

**Marcus Barrick**<br>
Yeah, in terms of the interface, I think it'd be nice to get out of like a list thing. So it's not just like a list of issues because I think you need to see like a cluster of relationships and problems or whatever. And then like this is actually interlinked with this and then having some like colored linkages to show what affects whatever and then what is maybe like the most central of the problems or a more important thing to visualize. Kind of like a graph based mind map thing.

**Alberto**<br>
And also I would add that it also is an interface to take a look at all sorts of data. Like everything is stored, that is stored and can be accessed by the participants of a node. And yeah, it's important.

**Gary Kent**<br>
I think we need to keep in mind that most of that data doesn't exist yet. Not even the modules themselves don't exist. But for this first phase, we do want to have the structural architecture for all the variables, all the records in place. Because eventually, that's where all the records will be stored. So during the test run, we're going to be probably making up OAD records that are going to be input. We're going to be doing it. We're going to personally be doing that in order to run the test to see if the MVS works.

**Regis**<br>
Can I ask something? I don't know if it's, well, it's definitely not directly related to this. But I have the feeling that this keeps popping up here and there. And that is like, I think it's, Or at least I kind of understood that one reason why we're gathered in this Discord, not this study group, but the Discord channel, is because we want to do some very thorough reading of the white paper and all of the documentation. at the same time when we're trying to look for for holes and and problems and things like that and and we we're like bumping into this kind of stuff all the time here and what i'm trying to do now is like take a step back and then ask you guys what should we do in these cases i tried to raise this uh in in one of the channels i don't remember even what it was like something Was it about the issue or some definition that was not clear? And I kind of understood that it's part of our task also to find problems on the white paper and raise those problems and try to find better definitions and better clarifications for those things. But I don't know what the process is. I don't know if we're now waiting for Peter to come up with his prototype so that we can, like, do the proper whatever process but i don't know like i keep bumping into these things and i would really like to have a place where we could just raise these questions and say hey this is not clear in the white paper we can't find the answer to this Is it that it doesn't have a good explanation? If so, then let's find a better explanation. Or is it because it's not even defined? Then, okay, we'll just have to wait or define it now, and so on. You know what I'm trying to say here. Sorry about that.

**Ben**<br>
Do you have a specific example of this, like one that you found?

**Regis**<br>
Everything Gary was saying here.

**Ben**<br>
He's kind of trying to define the back end, how the back end would work.

**Regis**<br>
I don't remember now, but I will try to find. I can ping you.

**Marcus Barrick**<br>
We even raised one today about the OAD in module 3. That is a good example, I think, of something that seemed to be a mistake.

**Regis**<br>
Yeah, every now and then we find these stuff. Yep.

**Gary Kent**<br>
the one word that Lucor decided to change, the candidate he changed to possibility, I think, or possible, the word possible. And I think that's a good change. I mean, that's a clarifying change. in terms of basic language that I think would be helpful. But that's the only thing I've found so far. And I think that if we find other things that we're struggling to understand, I know I've found this again and again. I've got pages of questions here that I've developed for myself. And almost inevitably, as I've read deeper and studied all the rest of the modules, I've found the answers to them, those questions, to a certain extent. some of the ones that i've raised here today are ones that i haven't answered for myself yet but i think that probably there should be on the discord forum we should have a space in which we raise these possible issues the other aspect of this that i wanted to point out is that peter has already taken that into account the website that he already has up and running one of the things that he suggests if you find any problems in the white paper or in the dev guide, then you submit those changes, those possible changes here. I've got a place where you can do that. Just fill this out, and I'll check it out when I get an opportunity and see if there's something that you have noticed that needs to be fixed. so it that's pipeline is already set up but i would suggest that as a working group here we should probably discuss these things among ourselves so we're not bombarding that with things that are somewhere in the paper that we've missed it's you know i agree

**samw**<br>
Aren't we doing this by going through the modules step by step? We have a list of open questions that we make as we go through them. Maybe we're at a slow pace because we're doing one module at a time. But we're carefully going through the modules. Questions come up as we do them. Is that an insufficient approach, do you think, maybe? Or is that what you're getting at? For me, it's too slow. Yeah, but we'll get faster.

**Alberto**<br>
We're just starting. Yeah, I also think so. I think we need to get to the same page first. Yeah.

**Lukas Orsvärn**<br>
Yeah, that's what I was going to say. Oh, sorry. Go ahead, Ben.

**Ben**<br>
It's not so much that there's little problems. If I look at the big picture for the integral, like the system, then I can see, okay, this could potentially work. Maybe there's some little pathways that need to be tweaked or something. But then there's, like, from this, my current, like, theory on what is going to be the problem is getting people to participate. Like, we only have, like, six, eight people here, right? Are people actually gonna use this interface? Like that's for me, and I have this tool library that I try to run with our local cooperative too. And I built a system kind of like a tool library system. And one of the biggest issues is how do you get people to actually use it and participate in the system? Not like the little interactive, the little arrows from like one section to another. Okay, fine. Maybe that can be tweaked a little bit, but how do you actually get people to use the system is my question. Do you understand what I mean?

**Gary Kent**<br>
Absolutely. The same thing was true for a time back that we played with in my area, in my community.

**samw**<br>
But isn't the strategy, maybe it wouldn't work in real life, who knows, but isn't the strategy that the initial MVS of integral would be valuable to an organization to adopt. They're not using it out of the kindness of their hearts. They would gain something from it, like organization or a cache of designs or whatever it is. And that was one thing I was thinking about the minimal viable system. Peter was just designing it such that it functioned as a cybernetic system. It worked. But perhaps another consideration is to make it attractive enough to use. And to do that, you would have to emphasize the parts of integral that are most valuable to potential proto nodes or these nonprofit organizations. But I think the bet is that integral offers value to nonprofit organizations, basically. And so they'll want to use it because it helps them, I think.

**Alberto**<br>
yeah but i also think it's oh sorry go ahead alberto i also think it's it's a little bit too early to to also think about a possible interface that we can roll out for the public i think it's also in the stage we are right now and to to get more people on board it's just activists like we are all are right it's just activists that have an interest in making uh something that is that is usable from the public's perspective. And I don't think we're not even really around the corner there. We still have a lot of work to do, right? So before we get there.

**Lukas Orsvärn**<br>
Yeah, I think when I think about this, I think about it as kind of a separate issue. But I also think that's going to be a very hard part of it. And I have some thoughts on it and stuff. But for that to even be a problem, we first need to have a system that works, kind of. Because if we don't have that, then... Yeah, that's a good problem to have, essentially. If we have a working system and no one's using it, then we can fix that. But yeah, we need the working system first. So I see it as a separate issue from looking at the system itself and stuff like that. Though, of course, something could be built into it to make it viral, for instance, or something like that, which I think it kind of is already because of being valuable, of having inherent value The problem is just starting to demonstrate it, I guess. Because that's also kind of what I think is the same as SAM, essentially, where the system needs to have value in itself. There needs to be some people, some groups start using it, and then it provides value to them and then other organizations will see that oh this provides value and then they want to adopt it because no existing organization or very few existing organizations would be very hyped about swapping out their entire governance system adding in you know time credits that they didn't have before having to account for stuff like you know input and output from their cooperative and stuff like that So it's a very big thing for an organization, existing organization to take on unless they can see that there's a clear value there, which I think there could be. Like if we make it good and there's like very clearly like we're just getting people who do work in our organization and we barely have to do anything just because it's good for them and it's good for us, then I think others would want the same thing kind of.

**Marcus Barrick**<br>
I think a lot of orgs like trying to use JIRA or other like Azure to organize and like this is so limited and like this is like orders of magnitude above and beyond. And I think it's a lot of value in it.

**samw**<br>
And another thing about that is that nonprofit organizations, some of them are really, really, really disorganized. I've worked in at least one and they need help and they would like they're all a lot of these people are just like overworked. It's chaotic. And so some sort of organizing framework they'd welcome if it helped them. And maybe part of the activism of integral will be finding out precisely which organizations are struggling with these issues and then kind of marketing to them or seeking them out.

**Lukas Orsvärn**<br>
But I would like to circle around, back around to the question that was talked about before of, you know, you brought it up, Regis, about, you know, if we find issues, what do we do with them, kind of? And I just want to like finalize that or whatever. The way we're doing it here when we're going through these modules and stuff, which Sam mentioned as well, is we have the open questions at the end of each module of like, this is stuff that we just haven't been able to figure out. So we're kind of gathering them in each module as we go. And Sam also asked this, but I don't think he got an answer about it. Like, do you feel like that is what you were looking for? And you're just like, oh yeah, I forgot that we had that or we were doing that. Or do you feel like that's not enough? Or yeah, do you have thoughts about that?

**Marcus Barrick**<br>
Was that directed to Gary?

**Lukas Orsvärn**<br>
Maybe it was Gary who talked about it. I thought it was Regis, but maybe it was Gary. I'm not sure.

**Gary Kent**<br>
Does everybody know where we're on the website? The funny one with all the green and black stuff. There is the place where you could submit problems if you see them in the white paper or in the dev guide. You can make submissions and Peter said he will take a look at it and see if there is something that needs to be fixed or made more clear. Does everybody know where that's at?

**Lukas Orsvärn**<br>
Sorry to jump in. We're going to take a five-minute break now. If you can post a link to that in the chat, Gary, let's take a five-minute break, and then we'll come back and continue talking for another 45 minutes. All right, yeah, break time. Thank you. See you in five minutes.

**Gary Kent**<br>
And so that we can critique it in order to be helpful. That's what I see our role as being partially anyway. And that's what I see this study group as making an effort to try and accomplish. I think it might be a good idea to create a particular place on Discord where we could post questions that we have that we've been unable to find on our own and just put them up there and say, hey, has anybody else discovered where this might be talked about in the white paper or the dev guide? Or can you explain to me, I don't seem to understand how this is functioning. Can you help me understand it?

**Lukas Orsvärn**<br>
You can definitely already do that in the Discord. You're free to, if there's something you don't understand, you can just make a new thread about it and ask and people can respond.

**Gary Kent**<br>
Where are we supposed to be posting that thread at this point in time? Everybody will pay attention.

**Lukas Orsvärn**<br>
It depends on what the question is about. There's one channel for each of the subsystems.

**Alberto**<br>
I just forwarded Peter's thread about exactly this. Core CDS analysis thread from, yeah, I think it was June. And yeah, so it's exactly that. Like go through all modules and critique them. So I think if you want to, I thought about putting my critique from the German chapter on there. So I'm still working on the translation, but that's where I would put it up.

**Regis**<br>
this is exactly what i meant actually but of course like this is specifically to cds i was asking in general about the whole the whole effort here but i think again part of our job here is to do this like this like um really nitty-gritty review of the whole thing and try to find holes, because if we don't find those holes, then the so-called adversaries will find the holes and it starts to become a problem. So before this goes, like, viral, we have to kind of address these issues. But that's what I meant, and thanks. This was exactly it. About... Gary, the link that you sent, it just redirects to GitHub again, and then it will be like the process where we ended up here. So there is no form or nothing like, at least I couldn't find, like how do you then make the proposal? But anyway, it's not that important, no.

**Gary Kent**<br>
Maybe we should append that link at the top of some category where just general broad questions can be talked about.

**samw**<br>
Right now we are on hiatus, remember. We're doing it unofficially. We're doing basically what we will be doing officially later. And my view is that I know that we have an end goal, which is to have simplified modules and mapping. But I think the real point is not the result of that, to have an artifact, but the actual doing of it for our own personal education. Because what I'm getting out of it is it forces me to read the white paper more closely And I learned more about it. And I think that's my perception of where we're at right now. We're just doing this as an exercise for our own personal benefit. And then when integral resumes working from its hiatus, then Peter, I guess, will direct us in a way where we will be going through every inch of the white paper and the pseudocode and be heavily scrutinizing it and eventually rewriting it. We eventually will be rewriting the entire thing together, I think.

**Regis**<br>
Yes. Yeah. Yeah. What I was trying to say is that I agree with you. This is the I think this is the main point what what we are trying to do here. But I feel that while we do this, we also at the same time find these problems, or at least it might be that they're not. It's not that they are. and that there are problems but maybe it's like about clarity so it's not very clear on the white paper what this thing does or what this thing means and so on and i think it's good it's a good that we start trying to gather those things but again lucas has answered that already i think it's good that we have these open questions there and then we collect all these things that we bump into that we can't answer and then eventually they will be part of this like scrutinization of the of the whole thing so I just wanted to bring up because this is on my mind all the time.

**samw**<br>
Yeah, no, it's definitely good we have the open questions. And then when we're done, we can send them all to Peter at once and completely bombard him with chaos.

**Alberto**<br>
Just kidding. Yeah, so let's continue going through it then, right?

**Marcus Barrick**<br>
Yeah, I was going to say I have some open questions on module three for when I go through those. Yeah.

**Lukas Orsvärn**<br>
I'm going to share my screen.

**Ben**<br>
Would you want to look at what most people see as the weakness for Module 3? What is the biggest weakness for this sub-module?

**Alberto**<br>
I think it's such a big module. It has to do so much at the same time. It has to retrieve so much data. I think maybe the weakness is exactly in the complexity of it.

**Marcus Barrick**<br>
Yeah, I think it's like trying to integrate it, but I think it's just going to be a dashboard of information that like the human would have to integrate because doing that automatically is like just so much work because I'm pretty sure you described it as like. You don't even need humans in the loop till module 5, but I feel like. You need someone to parse this data and like fetch the data to see if it's even the right kind of data. It's not just like assuming it's the right thing because of you know. or sloppy code base or something.

**Gary Kent**<br>
I was unaware that protocode is actually a thing.

**Lukas Orsvärn**<br>
Can you say that again?

**Gary Kent**<br>
Is there a general glossary of protocode terms that is out in the ethernet somewhere? Internet? What do you mean?

**samw**<br>
In the cloud? Isn't Peter's pseudocode similar to Python? Isn't it basically?

**Regis**<br>
That's how it feels to me, yeah.

**Gary Kent**<br>
It looks kind of like Python, but I think there is something called pseudocode. At least I've seen it. I did a search for pseudocode, and there seems to be an existing pseudocode out on the web somewhere.

**samw**<br>
I think Peter's pseudocode is different than regular pseudocode.

**Regis**<br>
I think he's calling it pseudocode because it's not fully functional. There are functions there that are not defined anywhere. They are just magical. There is something that does something, but it's nowhere defined. I think it's more in that sense, not necessarily that it's not a specific language. It's just Python, I think, but that is not complete.

**Lukas Orsvärn**<br>
Yeah, the pseudocode that he's referring to in the white paper is in the white paper. Like, yeah. I guess I can show it somewhere.

**Gary Kent**<br>
Google searched pseudocode.

**Lukas Orsvärn**<br>
So here's an example of some pseudocode helper type. And this is what is called pseudocode in the white paper. Or this stuff. uh yes sorry um any other thoughts about the module three we should open questions right sorry yeah that's exactly it um so it's like oh there's the echo no um if

**Ben**<br>
For example, I were to have like a proposal. I want to build a community garden and then I get it to module three and I have like in the database like a list of plants that have been successful and they're all tagged with community garden, then it would be simple enough. Like I just look in the database for things tagged with community garden and there I have my knowledge. base, I guess, and it would kind of put it together and display it. Is that simple enough? Or does it need to be more complicated than that?

**samw**<br>
I guess it would have in terms of a description of mental three. Yeah.

**Ben**<br>
I guess it would have to have some kind of like, when it's in the database, like I have plants, and I would have to have maybe outcomes or something with it. It's like this plant, and then this one turned out, this one grew very well, it was robust, whereas this one failed. So you have two plants and one failed and one is robust. And then you can kind of look at that data and say, make a decision on what to put in the community garden? Is that the kind of thing we're talking about?

**samw**<br>
That's definitely one facet of it. That's the historical records. But somehow, apparently, it's supposed to... I don't know if it's from that specifically or from other sources, but maybe I think external data sets are put into Module 2, and maybe it's from that. But how many resources a project will need how much labor a project will need, quote unquote, fairness considerations. I'm not exactly sure how that's determined. Although I think part of the ambiguity of all this is these things are all coming from different subsystems. Maybe they're more clearly established. And once we get to those subsystems, maybe it'll be more clear. But I think the purpose of module 3 is to establish constraints and the limits of what a given proposal can't violate in order for it to be a good proposal.

**Ben**<br>
How would it do that? How would it make constraints?

**samw**<br>
I mean, there's a mathematical equation at the end of module 3 pseudocode. That's how I interpret. What page is that? Let me look.

**Marcus Barrick**<br>
we still have to like realize that that mathematical equation sound like the answer is just like one way to put a number to something like actually reducing the ecological like values to one number is like the really hard part and same thing with labor and all this kind of stuff um yeah it's page 43 of the white paper i don't know if it's

**samw**<br>
I don't really understand that math. So maybe it's just a placeholder and symbolic more than anything. But also, I think we might have more clarity on all these things, because all this information is coming from other subsystems. And the other subsystems may be doing the work to crunch these numbers. So maybe it'll be solved once we go through those other subsystem modules.

**Marcus Barrick**<br>
I think it's really important. It's really important to have like a context for this. Like imagine like we need to build a greenhouse so we can build this many tomato plants or something like that. And we need all this labor, but like you also need like specialized labor and like that's only for a fairly simple system. And you know, once the systems get more and more complex, like labor isn't just like ours. It's like these kinds of tasks and we need these kinds of people with this kind of knowledge. Yeah, it's complicated.

**Gary Kent**<br>
Greenhouse might be a set of scenarios in the OAD somewhere.

**Lukas Orsvärn**<br>
The OAD would have the blueprints for the greenhouse.

**Gary Kent**<br>
Exactly, for greenhouses, among a lot of other things. Some of them will be labeled greenhouses.

**samw**<br>
Speaking of the OED, that was another. I mean, it omitted the OED from the actual specified module 3. But earlier in the white paper, it talked specifically about the OED in regard to safety constraints and architectural constraints, whatever that means, which makes me think that it should have been included probably.

**Ben**<br>
If I were to be critical about this, how do you go from a qualitative thing, like an ecological indicator, into a quantitative math equation? How do you go from qualitative to quantitative like that?

**Marcus Barrick**<br>
Well, it's literally the entire problem of trying to build a resource-based economy. We just assume money does that, but it's just a totally hand-waved thing. So we're just trying to get a resource-based economy that has a little bit more values. So it's not ever going to be this perfect thing. It's just supposed to surface up so we can make decisions based on ecological data.

**samw**<br>
How do you quantify fairness also? That's one of the factors. Fairness seems very difficult to quantify too. How do you do that specifically?

**Gary Kent**<br>
Indeed.

**Lukas Orsvärn**<br>
Yeah, well, maybe it's like if you're building a playground, maybe it's like we shouldn't build a playground next to the other playground because then a lot of people there, it's unfair that all those people get all the playgrounds. Maybe you should spread them around. So it's more fair.

**Ben**<br>
Okay, but then how do you put like a number to that?

**Lukas Orsvärn**<br>
Well, you could be like, how close is it to, like, how many people have the closest to a playground, kind of, and the closer, the fewer that is, then the lower the number is. And it can be expressed as a percentage, kind of.

**Alberto**<br>
I think it's a normalizing equation. You use an equation to normalize, and it's kind of like, it's complicated, I'm not a math... person myself, but, but I think, yeah, there are, there are existing models, but we, we have to understand them first. And I think the, the white paper talks about them, but like, yeah, if you're not into math, then you're not going to understand it.

**Ben**<br>
It would have to take kind of inputs from people surveys and say, okay, this is the result of the survey and then kind of put it statistically.

**Gary Kent**<br>
For some systems engineering, there are all kinds of men Max equations that's one of the things I studied in university back in 1969. And those usually it has to do with one of the things they used to try men Max is money. and certain resources and things like that. But what we're trying to do is to do min-max equations that take money out of the equation altogether, among other things, and profit. We're trying to take that out of the equation. So you can still use min-max equations. It's just the weighted references are different. In this case, they're going to be environmental sustainability and resource sustainability and profit. human need, and things like that.

**samw**<br>
Would you be able to explain what a min-max equation is to someone who has no idea, no good background in math?

**Gary Kent**<br>
Well, that's what I went to university to study. So I don't know exactly how, how easily I could make that understood, but did you understand sort of what I'm saying? You pick certain quantities or qualities and you try to maximize or minimize certain qualities. And, uh, there can be a balance. It doesn't have to be all one, one quality or all another. although the way the monetary market economic system is, it basically tends to maximize profit and to put it in the hands of a few people. That's what it seems to do. So it's an automatic min-max operation that goes on within economics the way we market monetary market economics right now, except we're designing a different type of So the min-max categories are different than the one in the monetary market system.

**Ben**<br>
So you want to minimize the use of labor indicators. So you need to have, for example, if you have a bunch of labor indicators and you want to use the minimum amount of labor, then you're trying to minimize that, I guess, right?

**Gary Kent**<br>
Yes, that's one of them.

**Marcus Barrick**<br>
Another way I understand it is, what are the bottlenecks of change? Are you trying to make the most positive impact with the least amount of labor? Then there's certain bottlenecks that actually affect it a lot more than a more linear approach, if you can just find these bottlenecks that might be a non-linear approach.

**samw**<br>
So for those who understand what mid-max equations are, does this approach make sense in the white paper? Does this make quantifying these things feasible and comparing them feasible? I'm just curious.

**Marcus Barrick**<br>
I think you need a lot of human in the loop, and I think people will only go through the effort of getting all this data if it's actually a critical decision to be made, because it is a lot to figure out and then make a cohesive argument for.

**Lukas Orsvärn**<br>
I think it would be interesting to hear what would be some type of data that we would need that would be complicated to get, for instance, or put into an equation or put a number to it. Ben, you were talking about it as if we need to have surveys and stuff like that. Do you have some thought about what would that be, for instance, something that would be hard?

**Ben**<br>
would it be a user interface where people can input this data? I don't know. Or would it be kind of trying to, I think he mentioned at one point you'd have like someone who would kind of record things as the job is being done. I forget where that was, but like when they're building something, for example, you'd have someone kind of keeping track of the resources and the labor and then entering that in somewhere.

**Lukas Orsvärn**<br>
Sorry, my Discord just crashed.

**Ben**<br>
Does that make sense? After you say you build a previous garden or something, then you have an indicator of this is the amount of labor that was used.

**Lukas Orsvärn**<br>
Yeah, exactly. Like when it comes to labor use and stuff like that, that would be saved like historically for your node and it would also probably be saved with like the blueprint then, right? If we're talking about a greenhouse and it's been built a hundred of these greenhouses, then you have some data about how much resources actually took to build them and in terms of time and also physical resources, for instance, and then... you could also put that together with also where in the world was it, and what climate did they have, and what resources did they have, et cetera, and have all that data in there and compare it to the things that are similar to your node, for instance. It's a very big, complicated thing to do, but that's how I imagine it in a way.

**samw**<br>
So integral really won't be efficient. Sorry, go ahead.

**Marcus Barrick**<br>
Just in the sense of like data, I'm also thinking like variable data, like the sun, like we're getting like solar power or the water would be changing. So like we can't just make a decision based on like one static number being like, this is how much water we get. And I'm just thinking maybe it's just because I'm thinking in terms of like C-sharp or object oriented programming and maybe AI can do a lot better in terms of just like throwing whatever data at the wall. But it's hard for me to imagine like an object that has all these different variability elements.

**Lukas Orsvärn**<br>
On the surface level, it should be... You can imagine doing a comparison of... You could know what each node looked like that the greenhouse was built in. And then you can... uh compare that to the state of the current node who wants to build a greenhouse and then you can find those that have similar numbers and you can sort of know which numbers are the most relevant ones like a human can decide that like maybe it's not relevant you know i don't know how rocky the ground is uh in a place when you're gonna build a greenhouse or whatever i don't know so maybe you just know that that's not relevant for this in this case But then that way you can find similar situations that have happened in the past in other places and find the most similar ones and use that as a reference for what might happen if you try to do the same thing. Does that make sense?

**Ben**<br>
Yeah.

**samw**<br>
So it's going to take a lot of nodes being functioning and compiling large amounts of data in order for integral to be efficient. It's kind of like this Catch-22, where we want nodes to adopt the integral system, but it's only efficient if a lot of nodes adopt it and generate all this data for them to make their decisions based on. Yeah, so that seems like an issue.

**Lukas Orsvärn**<br>
Yeah, definitely. But if you compare it to what we have right now, it's the same issue all the time. We have that inefficiency all the time. And there is no building up that knowledge. If we have cooperatives who want to build greenhouses, 100 across the world, that happens now, I'm sure. Maybe more, I guess. they don't have that data, that they can't share that data. But from integral and forward, everyone who's in there is going to be sharing that data, and it's going to be able to build from there, I guess. But yeah, like when we're starting out, I think it's also a very complicated thing Like, can we actually start on this level or would it be, it would probably be more human driven kind of what I think you're hinting towards and talking about Marcus, where we just, the most important thing is that we have the data so you can look at it. Cause I think we always want that because we always want to be able to see like if there's a, if the computer says, this is like a recommended way to do it, then we still need to be able to go in there and be like, okay, but what are you basing this data on? or like this recommendation on and be able to look at the data and so we can think about it because in the end, even if we're using AI or we're using like just a straight algorithm, it's all just a machine and it can't make decisions, it can't think, it can't be responsible for things.

**Marcus Barrick**<br>
Yeah, part of, I asked chat GPT how to do one of the things, I forget the question, but it gave like a really good response. And I did put like a skeleton code folder in there, I think it's in the second push, and gave like a layout of like ecological data types, which you could pull up if you wanted.

**Lukas Orsvärn**<br>
Is it this one? Or, no, skeleton code, sorry.

**Marcus Barrick**<br>
Frst ecological metrics. So like even something like a direction of concern and like thresholds are like really important if you scroll down and shows like different kinds of thresholds to. Like a warning range of critical range. Yeah, it's in like a direction of concern. It's like, well, if the value is lower, is worse, there's more risk or higher. So these are kinds of like ways they can have all, like automate the different units of like water or toxin or whatever, and then kind of make sense of that.

**Lukas Orsvärn**<br>
Yeah, this is so complicated stuff, like how to put this stuff into code and make it work.

**Gary Kent**<br>
I was talking about that. For FRS, it's going to be a real challenge.

**Marcus Barrick**<br>
But again, I think if you have the human in the loop and you actually care about making critical decisions, then it's fine. It's just a matter of like, understanding the problem space. But part of me raising that is like, I wonder how much AI can be like, oh, this is what should be relevant. And then it can like do second order searches for data. And then maybe the human loop is just like filtering out the irrelevant data or saying, like actually looking into it and be like, this is not the right use case or deleting stuff or something.

**Lukas Orsvärn**<br>
Yeah, exactly. Yeah, it needs to be able to learn and stuff like that. It's a very complicated thing. I think machine learning sort of approach is actually probably a good approach for something like this. But hopefully in the end we won't need to use actually LLMs to do this sort of stuff. We should be able to do more general machine learning where it just takes in the numbers and outputs other numbers kind of based on that because making an algorithm for it can be very complicated but we'll essentially have something like you know the old school recommendation algorithms or whatever where it just takes in oh these things you've seen these videos cool then you probably want to see these other videos you know it's just numbers in that sense But I think probably starting out a human, and then assisted by LLMs, and then eventually towards some custom machine learning thing when we have enough data. Because that's what you need to be able to do that. You need to have a lot of data.

**Gary Kent**<br>
One of the things that I really have been enjoying playing with a little bit is I imagined if we had a functional integral node, what kind of designs would I like to see implemented? And one of the things I was imagining was to have a daily node newsletter. constantly back to the node, state of the node kind of thing. And if you included that in some kind of a newsletter that could be shared over federation links to other nodes, then you would have actually a fairly trustworthy news source, which is one of the things we seem to lack everywhere these days. A trust-based news source.

**Alberto**<br>
nice add-on that's the only thing i wanted to say it sounds nice yes

**Gary Kent**<br>
Well, those designs, I mean, that's what this is partially all about, open source designs that are broadly shared and revised to be better and better in functionality as they get revised. I mean, that's kind of what doesn't happen in the monetary market system. All those things get set on by corporations and they don't share them and people can't make contributions to improve them. It's just like prohibited. And that's one of the things that this economic model encourages.

**Lukas Orsvärn**<br>
We have about 15 minutes left in the meeting. And I would like us to spend the rest of the remaining time to figure out if there is any concrete things that we should do next, like something we should do different, something we should do, like we had the git thing and stuff like that, and something we're kind of working on right now. And also, by the way, sorry to just interrupt and change the topic entirely. But yeah, I want to get this done as well. We had a workshop earlier in the week about using GitHub to contribute on this repository. And I would like to know if there's any more blockers in that sense. Should we do another workshop or anything else like that? Is there something where people are like, oh, I would like to contribute, but I can't because I don't know how to do this thing or I don't know how this thing works or I don't know if I have the permission, like social permission, like am I allowed to do this or something like that.

**Alberto**<br>
We would be interested. So if you're up to, we can meet again.

**Lukas Orsvärn**<br>
About doing another GitHub workshop? Yes. Yes. OK, nice. Would other people also be interested in learning more about using GitHub to make contributions and stuff like that here?

**Marcus Barrick**<br>
Yeah, I didn't know you guys did that. I think it could be just a little refresh on at least higher levels and stuff. Mostly just interface stuff.

**Gary Kent**<br>
I could hardly hear you. Marcus.

**Marcus Barrick**<br>
Oh, really? I was just saying, I'm so used to having the Git integrated in Visual Studio Professional and not as a separate thing. So I'm just getting used to that being separate. But yeah, I would join. To your question, though, I think maybe it's too early and this is just like a study group for us but i think seeing as integral is like a more of an ecosystem than like a this is our development project i think we need to like figure out what other open source projects we can like integrate into all of this like i posted a thing on uh regen os it's like a village os like resource management simulation kind of thing um you know whether it's that or like time credit stuff i think it's more or less how do we like stitch in all these systems that already exist instead of trying to build it from scratch so i think there was some threads talking about like a tech stack but i haven't gone through those yeah for sure i think there's also uh um

**Lukas Orsvärn**<br>
a place on the discord even for suggesting or talking about technologies that could be useful to like you do a proto node and stuff like that for instance so if people find stuff like that i think definitely share them in the discord and so that people can discuss about them and stuff like that Okay, but Git Workshop, all right, let's do another one. That sounds fun. And I'm also, like, on my list is also to write down kind of what we're doing in the Git Workshop to give documentation for people who need this information. Because workshops are great, and I think we should do them generally. But also a lot of people could just get started with reading how to do stuff, I think. So that's also on my list of stuff that I want to do. Is there anything else people can think about that they're feeling blocked by that they would like? I would contribute, but I can't because of this reason.

**Marcus Barrick**<br>
I think we don't have full we've been established like what we're using the get for like we like I kind of mostly just copied or rewrote the the white paper into this and then added some questions but I think like having a specific context to have a little bit more of an example in detail whether it's for this or for our conversations I think would help a lot is to get into the

**Ben**<br>
yeah just that natural realm of actually seeing how complex some of this stuff is like we've kind of circled around a few examples of like a greenhouse but at one point we were discussing i think we wanted to get the the mermaid diagrams done um if i have it some time this upcoming week i might try to take a look at those mermaid diagrams but yeah

**Lukas Orsvärn**<br>
Yeah, for sure. Yeah, feel free to start working on that, definitely. What specifically do you feel is missing? It sounds like you want more context around this. That, to me, would live in the readme file, right? I don't know how into programming and Git stuff you are. Is that kind of what you're thinking, too?

**Marcus Barrick**<br>
Sorry, who are you talking to?

**Lukas Orsvärn**<br>
I'm talking to you. Yeah, because you were talking about, yeah, go ahead.

**Marcus Barrick**<br>
Because like we have the mockable descriptions, but if we have like more specificity or like, I don't know how much scope, like I mentioned before, is this going to be like an object that I can point to or can I raise in and just add comments throughout or is it just supposed to be like a simplified white paper? I'm trying to get your position for it.

**Lukas Orsvärn**<br>
Have you seen the readme file? Oh, sorry. Maybe. I can link it in the chat.

**Marcus Barrick**<br>
Yeah, I'm looking at it now.

**Lukas Orsvärn**<br>
Because I feel like that is supposed to cover that sort of stuff. It's just on the front page of the repository. And if you feel like, if you read that and you feel like, well, this doesn't really, or like this is unclear from this or something like that, then you can definitely make a issue about it and discuss it. Or you can make a pull request if you have specific changes you want to, you think would be good and we can discuss that. Do you think that's good next steps for that?

**Regis**<br>
In general. I turned off my camera because I'm getting disconnected all the time. But in general, I would really wish that this would be very low barrier. You know that anybody would have any thought about anything that is there and then just go ahead and do something. If you're not very comfortable about what exactly to do, you can open an issue there. That's really the lowest barrier thing you can do. Just open an issue, point to something. Hey, I think this is not clear or this is bad or something. Or it, of course, can also be in Discord. I think in general it's good that we start learning how to use GitHub and also developing some sort of like a practice in this group because it will be one one of the main tools that we're going to use for integral so it's it's good that we know how to use it but I really wish that people don't feel like you know I don't know how to do this so I'm not going to do it or maybe I send another like I mean, the whole kind of the point of having this version control is that we can always go back. So it's not like you can break something, you know, just go there and change or propose something. So I really wish people would have like really low barrier to start doing stuff. I think it would be very, very profitable for everybody. But that's just my wish.

**Lukas Orsvärn**<br>
Yes, that's also what I try to encourage people. Yeah, just go in and do stuff. Just click around, try stuff, see what happens. If you're going to do something that's going to break something, totally, it's very clear. It's going to be like a big red button saying, like, delete the repository. Like, don't press that, you know. But no one needs to tell you that. And I think most people... We have a few owners of the repository who can invite people and stuff like that and do all that sort of stuff. But most people who come in can't even do stuff like that. That would be, yeah, that's just how it works usually, right? Not everyone can just delete the entire thing, for instance. So yeah, go in and press stuff, try stuff out. See, there's lots of features in GitHub that are interesting. So yeah.

**Regis**<br>
Yeah, and I would also like to add that if somebody who is here now or who is watching this afterwards, that feels like, okay, I really don't want to do this on my own, then just ping me, or I'm sure other people would also be available for this, ping me, and then we can do it together, you know, like we can go and try to do whatever it is that you think you can't do by yourself, right?

**Lukas Orsvärn**<br>
Yes, that's great. Yeah, and I said the same also in the last workshop we went to. If people want something, you can also ping me or ping Regis. We know about this stuff and can help you figure stuff out. But that's also the point of the workshops to kind of share that knowledge a little bit as well. Like there are many people who are new to this, so it's good to do it everyone at the same time and stuff like that.

**Ben**<br>
So yeah, that's great. If we were to... I'm just thinking about the minimal viable model. Sorry to... Yeah, it's great, the Discord thing. Just before we end here, it's just a thought I had. It's like, for a minimal viable model, would we need... Do you think... Actually, never mind. Maybe I'll address this next week. I think it's something for next time.

**Lukas Orsvärn**<br>
All right, feel free to put up an issue or something about it so we can think about it before the next meeting as well. I think that would be useful.

**Gary Kent**<br>
Do we have a little bit of time?

**Lukas Orsvärn**<br>
We have four minutes.

**Gary Kent**<br>
I'd like to ask a question. Have we got a term for what this entire five system we're trying to create is called?

**Ben**<br>
Integral.

**Gary Kent**<br>
Just integral.

**Alberto**<br>
I think so, yeah. Do you have something better?

**Gary Kent**<br>
No, I don't know. I've just kind of wondered because I haven't seen it said, well, this system is called integral. Integral collective, I guess, is really...

**Regis**<br>
I have proposed an alternate name. Not name per se, but like a name for the concept. It's the Societal Operating System, SOS.

**Gary Kent**<br>
Okay.

**Regis**<br>
But it sort of is like, you know, an operating system for the society.

**Lukas Orsvärn**<br>
Yeah. But yeah, that's how I interpret it, that it's called, it's integral and like the white paper refers to itself or like the thing itself as integral, you know, like these five parts of integral and integral is the system. And then, yeah, all the things inside of it are.

**Gary Kent**<br>
So it's the integral system.

**Lukas Orsvärn**<br>
Well, integral is the name of the system. So it's integral. Yeah. And then the integral collective, we are the people who are building integral.

**Gary Kent**<br>
Okay. The integral system, and we also have within that system five subsystems that we call CDS, COA, so on.

**Lukas Orsvärn**<br>
Yeah.

**Gary Kent**<br>
COS.

**Alberto**<br>
Yeah, I just wanted to also talk about just a second about and it's not a critique to anybody. I myself do the same, but we get distracted very easily. And maybe we kind of can like focus for, let's say, half an hour. on on on talking about the modules really and and specifically go to the um the questions part where we can actually really in in an intensive way talk about uh um the issues and and and the stuff the failure modes and the critique that we that we find um and maybe even um throw in some minimal viable build uh situation to it right so this this would be something that that um i would just just think it would bring us a little bit more uh or faster yeah more focus to the to the thing yeah like just half an hour we don't have to do the whole one and a half hour but just half an hour and kind of like do an intense thing um yeah just a suggestion

**Lukas Orsvärn**<br>
I think that sounds like an interesting idea. It would be great if you could write that down, put it on Discord in the next meeting thread, which will come up probably pretty soon after this meeting.

**Gary Kent**<br>
Meeting 10.

**Lukas Orsvärn**<br>
Yeah, exactly. Or if you prefer, you can put it on GitHub. But yeah, just so that we can see it and integrate it in the next meeting and think about it and stuff like that.

**samw**<br>
So that would just be a half-hour block of the meeting devoted solely to whichever module we're currently working on? Is that what you're saying?

**Alberto**<br>
Yes, if all are on it, yeah.

**Lukas Orsvärn**<br>
All right, great. Well, that's all the time we have. So thank everyone for attending. And yeah, I hope to see you in the next one.
