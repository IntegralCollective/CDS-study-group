**Lukas Orsvärn**  
Hello, everyone, and welcome to the seventh integral meeting. Yeah, last meeting, we decided that we would use these meetings for a study group. So that's what we're doing. I don't really have much plan for how we're going to do it exactly and stuff like that. But we can do breakout groups if we think that's a good idea. And other than that, I think either way, we should just start together like we are now. Talk a bit about how people are feeling about the work in general, I guess. How do people feel about it? Have people had time to read through it? I myself, only since I've been traveling, I've been away. I've read through it, but I haven't had much time to really reflect on it. Where are people at with it themselves?

**Sabrina**  
just quickly a hello to everyone and I have Alberto right beside me he's part of the German activist group and yeah also already we are both like dealing with Integral together and also with a German activist so if there are no objections he would like to join to also learn more and also to give input and stuff yeah if that's alright with you guys but I wanted to ask first yeah

**Alberto**  
Yeah, of course. Hello. Nice to meet you all.

**Lukas Orsvärn**  
Yes, nice to meet you too. Was it Alberto? Yes.

**Sabrina**  
Nice to meet you. In our case, we both read CDS and we already started to do the simulation on GITI. Maybe you want to say something about that?

**Alberto**  
Yeah, we read it actually the day, or actually really early when it came out, the CDS in the integral paper, but it wasn't that clear. I think the dev guide made it a little bit more clearer just because of repeating the whole stuff. Yeah, and because of that, I mean, we kind of sped things up and started spinning and we started by simulating something similar to Integral in a specific game that we did. And after that, we realized very, very fast that we have no idea what we are doing with this new game and how we are trying to approach it. So we stepped a bit back and then we started to get more into Integral and into how it is actually to be implemented. And that's where we are right now, just kind of a bit toying around with it. with specifically the CVS module, but in relation to Git T now. So it's not GitHub, like it is planned with Peter, but it's Git T. It's not the same, but it's still in the similar ballpark in these kinds of programs. And that's where we are at the moment where we defined a kind of a pipeline that continues, how it's intended, kind of like. But it's still just something experimenting. We're just trying out the pieces and we're certainly sure that this is not a working prototype at all. This is just to get the feel for it.

**Sabrina**  
Yeah, also to feel for the modules and stuff. Yeah, but what we are doing here now also.

**Lukas Orsvärn**  
Okay, so you have a pretty good grasp of it then, I guess, if you've even worked with it a little bit, kind of like trying to implement some things and so on. That's nice.

**Sabrina**  
Yeah, at least we talked a lot with people about it. And I think it helped to repeat a lot because there's so much information.

**Alberto**  
And make all sorts of assumptions also. You have to make all sorts of assumptions. We have integral and it's pretty clear where it leads, but we do not have the little details. That's what we need to figure out first, I guess. That's why we are here, yes.

**Lukas Orsvärn**  
Yes, exactly. All right. I'm just going to give the word to someone so people don't have to feel like they need to jump in. So I'm just going to give it to Sam. Where are you at with the reading of the things?

**samw**  
Yeah, I read everything. And then yesterday, I also watched the Revolution Now episode where Peter goes over the CDS. I forgot that existed. But that actually really clarified things for me. And it also made me realize how important, I don't know if, I forget if we said we were going to read the pseudocode or not, but it made me realize how important reading the pseudocode is because the actual, I guess the pros leading up to the pseudocode in the white paper leave a lot of stuff out. And if you look at the pseudocode, which I don't fully understand, I could get a general idea of it. And there's all these, there's mechanisms within it that aren't described normally and it seems necessary to read the pseudocode in order to really understand the CDS. So yeah, most of my impression of the CDS comes from that podcast, actually, which explained both and highlighted the parts of the pseudocode that one should understand.

**Lukas Orsvärn**  
OK, interesting. Yes, I'm just going to pass the word on, and so everyone can get to say where they're at. Markus, what about you?

**Marcus Barrick**  
Yeah, I feel like it was ironing through, doing a few layers to feel better read for the first few modules. It's a good idea to review the Revolution Now thing, because I watched that a while back.

**Ben**  
Yeah, I have some of my questions and stuff that I laid out. I don't know if this is the right time to dive into that.

**Marcus Barrick**  
But yeah, just kind of seeing visually how it all clusters and then where knowledge gets integrated.

**Lukas Orsvärn**  
Yeah. Okay, nice. Gary, what about you?

**Gary Kent**  
Well, I've certainly been struggling to try and understand the details of what Peter has proposed here. I've been trying to simulate it to a certain degree, like the others were mentioning earlier, and played through these roles in my head over and over again. One of the things that I've recognized is that there's going to be massive amounts of data that we're going to have to store and access to make this functional. And I'm not sure how that's going to happen in this federated construction type thing. The CDS in particular seems to me to be a critical module. And I think that our focus on that is great. But again, I don't see how this is yet going to play out, although I think I have some notion of what the precursors for the decision-making, how they're modulated by the filters, the pre-filters going forward. But the details, again, are far from wrapping my head around a lot of that.

**Ben**  
okay thank you and lastly ben i've also gone over uh i've read the white paper um i i tried to understand it um my like you're saying uh gary there is like a lot of data so in my mind it's okay we need a database to organize it so I kind of go directly, I try to think of how the database would look. It's how I would try to envision it. I don't know if it's the correct way, but so I put a little bit of tentative work into trying to build like kind of a database for that. Not a lot though. So that's where I'm at.

**Lukas Orsvärn**  
Okay. Very nice. So now that we've gone through a little bit of what we've read and stuff, it sounds like everyone has read a significant amount of stuff and some have even simulated things and things like that. So that's great. And then we're able to talk about things. So the question is then, how do we do this? Do we want to split it up into two groups of three or do we want to do it everyone together, six people together? Do people have an opinion on that?

**Ben**  
I think six is fine. It's not too many.

**Lukas Orsvärn**  
Okay, six people it is. I see people nodding as well. And a thumb up as well. Two thumbs up. All right, cool. Yeah, so who feels compelled? Who has like a question or something they want to bring up about it? Shoot.

**Marcus Barrick**  
I'm looking at module 3, which is the knowledge and integration context engine. I'm trying to, like, just imagine, like. Are you guys envisioning it like a sequential. Saying module by module, and if you have to wait to. To add any information on. like afterwards because I'm trying to imagine like I'm coming from like object oriented programming like if the proposal is an object and then I know there might be like one that's like duplicate so then that kind of like gets merged I think in the second one but it seems to me like not module three is almost like like contextual information that might not live inside of that node, but might just be like, or might not live inside of the issue, but might just kind of live in the node. So I'm just, yeah, I'm thinking developmentally and like from an organizational standpoint, like it might help if we can paralyze stuff as much as possible. Do you have any thoughts on where things live?

**Alberto**  
Can you repeat the question, maybe from a different angle? I'm not following.

**Marcus Barrick**  
Yeah. So you have a node, and then you have an issue that gets raised. One of them says make a bridge. And then in module 3, there's all this other information from the FRS and COS and all the other systems, other geospatial information. So I'm wondering. if you just have the issue and then you're like okay let's add in like geospatial information i don't know if that has to done get done manually or if we can get done like automated but that would be like a significant amount of effort whereas if you just had geospatial information that was kind of in module three and then it would be like oh this is relevant for this issue then you could do geospatial information. You could do module 3 in parallel. And then as issues and stuff percolate up, then it can kind of merge in a way, instead of having to re-duplicate all this work always.

**samw**  
You're talking about the external data sets under the pseudocode inputs, where it says external data sets. And then there's all this stuff that can be inputted. Is that what you're referring to?

**Marcus Barrick**  
Kind of. I haven't adjusted the pseudocode, but yeah.

**samw**  
Because that was a question for me, too, where it's just random information that needs to be inputted to give context. Where is that coming from? Who's deciding to put that in? Yeah, it seems complete. It seems ambiguous.

**Ben**  
So for some of these things, I think it must be relying on some kind of AI, I think, to put this in.

**Alberto**  
Yeah, that's also my impression that module three and four are modules that should be automated pretty quickly, I guess. And that's data that is stored from decisions beforehand. And also in general, I guess you were right. Like it comes from all sorts of systems. Yeah. But I also had the impression that this is a module or three and four is three and four are not even in the minimal version in the dev guide. So they are left out deliberately.

**Marcus Barrick**  
So just as a stepping back, like. we seeing it as like a sequential thing like we have to wait to do module three once like module one and two are done or they can kind of be done in parallel

**Lukas Orsvärn**  
I think it has to wait. Like a lot of these modules, as I understand it, kind of like happen very quickly once you get there. But for this to make sense, to integrate knowledge and context, you need to have some reason to do that. You can't just like, if you're going to get to use spatial information, like a piece of a map or something, like, well, what piece are you going to get? Well, it needs to be something related to something. Like, are we going to build something? Oh, well, that's the piece of the map we want to get then, you know? So for that to be the case, you need to first intake the issues, right? And then there's the Model 2 that frames and structures stuff. And then it's like, okay, we now have something to talk about. Then you gather all the data from outside and that adds more information that you can use to further down the pipe. But as I understand it, like you're saying, like has been said as well, this would probably be automated to some extent, and LLMs could be used as well to some extent. In the case of a map, for instance, it could be fairly straightforward. Something is like, oh, we're doing something related to a building or whatever. Then it can just pull in the surrounding area automatically and present that as part of the information that's relevant to this, for instance. And any other information like that as well. That's how I think about it in a way. Does that sound like a probable thing? Yeah, someone go ahead.

**Ben**  
like in my mind sorry go ahead no you've been sorry i i so like in in my mind is it's um like yeah in the procedure you start with i guess the the cds and then it calls data from these other modules in step three But the data, like building that data, doesn't necessarily need to wait because you can have that data available for when it's ready, I guess, in the database. So you have like the map and maybe like a keyword or something, and it would look at the keyword and say, this is matching with the CDS proposal. And then it was kind of pull it together.

**Lukas Orsvärn**  
Yeah, exactly. That's how I also imagine it. The data would already exist. It would just pull in the relevant data. Yeah, go ahead. I don't remember your name. Can you say your name again, by the way?

**Alberto**  
alberto alberto yeah yeah i was just curious if if you were thinking about it from from a coding perspective on how it would be logically how to deal with that kind of of of modules three and four maybe but uh but but i think uh lucas and ben just just um summarized it pretty pretty pretty good that's how i also understand it yeah i was getting an image of like

**Marcus Barrick**  
Not necessarily object-oriented, but almost like a membrane, if that even means anything to you, of module three data gets inputted, relevant to that task, but maybe it could still stay in the pool of module three data for that node so that it doesn't just get held within these issues. It can kind of still maybe grow. Maybe that's like a more FRS kind of thing to have data accumulated over time.

**Lukas Orsvärn**  
Yeah, the way I imagine a lot of this data stuff is that it would be just like references to things. So like you wouldn't necessarily... A map is a good example. You wouldn't want to take a copy of a map and pull it in. You would want to have a live reference to this is the map of the location. Because it doesn't matter what it looked like a year ago. It's the most up-to-date version is the one that's the most relevant. So that's the way I imagine it. But that's also something that... I haven't looked super closely at which data lives where, what's actually stored in the database and stuff like that, and how that's supposed to work. And I'm not sure that's actually entirely specified, but that's how I imagine a lot of this stuff, that it would just be references to things. Yeah, do you feel like we're done with that question then, Marcus?

**Marcus Barrick**  
Yeah, yeah.

**Gary Kent**  
Can I make a comment? Go ahead. Well, I think that we should keep in context what it is that Peter seems to be trying to accomplish here. He keeps emphasizing this minimal viable system, especially the CDS modules in particular and the CDS system or CD system or however you want to refer to it. I think that in that vein, What Peter seems to be asking for at this point in time is for the modules that are being dropped out will be basically ignored. But we're trying to construct a database or a file data structure that will be compatible with everything else going forward. So that's one of the main things that we're trying to do is to create that record file, that issue record file. And each of the modules, the first one, two, and three modules contributes to that to some extent. And in the minimum viable system, my perspective on this or my understanding of this is that it's probably going to be basically just input from us. the people that are working on it right here on Discord to fill those data files, data spots out in the record file. We're trying to construct a full record file that will come out in the end of the CDS and be then attached to some database on a permanent basis. but then once we go beyond the minimal viable system, we'll be able to use the same record file that we've created.

**Lukas Orsvärn**  
Yeah, exactly. That's one aspect of it as well, that it should be compatible when we build it. But for what we're doing now for this study group, we're not focusing on the minimum viable system and things like that. We're just looking at the entire system as... Yeah, we're reading through the chapter 7.1 in the white paper and also the dev guide and all the information and just trying to understand it together is kind of the idea. So we don't need to be so focused on that, oh, it needs to be written out in the dev guide or something like that. If that's the impression you had, Gary, does that sound... Is that a valid response to what you said?

**Gary Kent**  
Sure. I mean, I guess I didn't completely understand. I mean, I agree with what you're saying about the study guide. We could be broader in it. But I think the long-term goal, obviously, of Peter is to actually have a programmed system that's functional. So that's where we're trying to get to.

**Lukas Orsvärn**  
Yeah, absolutely. Okay. Yes, so does, yeah, some other people also had things they wanted to bring up, right? Does someone else, except for Marcus, who already brought up one thing, have something they want to talk about here?

**Alberto**  
Yeah, I was thinking, well, I'm a bit nervous, so sorry for that. But I was thinking, like, We have to keep in mind that the part that is done by people, like the people that do the input, this is just one part of this whole pipeline. I think we need to keep that in mind, that actually when we go through the modules, then there's actually just module one, five, and nine are actually just modules that get input from people. Everything else is actually some module that needs to needs to needs to get the data from from where what gary just explained you know what i mean so so that's how we also need to keep this in mind like it's it's it's a pipeline that should work um and input from people is just one aspect of it so that's that's a big part that that I think also people struggle to think about, right? Because when we talk about decision-making, lots of people directly think that they have to do the decision-making and stuff. But also thinking about yourself as just one part of a bigger pipeline, this is something also that needs to click And I think it's not just for CDS. I think CDS is the most prominent one, but I also think that it goes through all systems. And I even think that FRS is also actually fully automated at some point. But yeah, I think you get what I'm getting at, right?

**Lukas Orsvärn**  
Does someone have a response to that? I don't want to respond to everyone, so I'm giving the word to someone.

**Ben**  
Yeah, that sounds correct.

**Alberto**  
Okay, then I don't know if you're eager to say something. Well, I would have the most because we have done a little bit of stuff with that. So for us, it was also something that has been talked here also very much. And it's about the module five. I don't know. And it's about blocking objections and bad faith actors. That's something that for me also in how we try to simulate it, it's also like, a stopping point where we have to actually think about it first before we can actually somehow put it into this pipeline.

**Sabrina**  
I agree with that.

**Gary Kent**  
I've worked with the same thing in terms of something that's going on in the valley here where I live in terms of trying to understand that consensus-making process, which is what the Module 5 is all about. And I think it's an incredibly important thing to focus on. Uh, you know, part of the decision making is simplified because we have all these precursors that lead us in these filters that kind of say, well, we're not going to consider things that are impractical in terms of environmental sustainability and things like that. So that happens automatically. And that limits to a certain degree, the decisions that we have to make, but there's still that human input that people come from so many different, uh, I notion ideas and ideals and positions. It's really difficult to imagine that for me as well. I tried to play with it locally and also getting people. One of the things that I've found difficult is getting people to get thinking about how people are going to be motivated to get on board with this, as opposed to continuing to function within the existing economic structures around us, because there are so many powerful motivations in those things. And I'm not clear what the motivations are going to be in this system, whether it's going to have to do only related with the ITC, or whether they're going to be other things that people can that will motivate people to want to be engaged with this process, the integral process.

**samw**  
The thing about module 5 is that the reason why it may not be as much of a Wild West scenario as it may at first seem is because the modules before it do everything they can to kind of structure what's being talked about in a way that's as close to objective as possible. Module 4 is really a test, I think. It's a test of the proposals to see if they meet certain constraints. That's pretty objective. So I don't think deliberation, well, I mean, obviously deliberation can get out of control. And there might be edge cases that are difficult to resolve. But I think for the most part, it'll fall logically from, the previous modules and what they guide people to decide almost. Because it's supposed to be at least more objective than pure subjectivity, I think. That's the impression I get.

**Lukas Orsvärn**  
Yeah. Yeah, exactly. I've thought a bit about this aspect as well of making decisions on things and blocking objections and things like that. What if someone's like, well, in my local culture, in my family, it's really important that the buildings are orange. And it's like, you can just come up with whatever you want, like, because it's cultural and the culture goes down all the way to family and individual level as well. And so should all buildings be orange? Just because on everything that we do, I'm just like, I think it's important it should be orange. And no one is like, well, what are we going to do? It's a cultural thing, you know? But I think on some level it needs to be also, there needs to be a democratic thing about that as well. Like, even a blocking objection needs to be able to be overridden if everyone's like, well, that just doesn't make sense. So it's just like... We don't want to have a symbol on every building that's related to you specifically or whatever, because you raise a blocking objection every time, right? there needs to be some way to override even those, for instance. That's something that I've thought about that's also related to this sort of deliberation thing. And when I add that in on anything, on everything, it kind of helps dissolve all problems, for me at least. Because, like I say, all the earlier modules kind of help sort down what are the possible things that we could do or should do. And it's like, OK, do we do A or B, kind of, or whatever? Or maybe we just, maybe, probably it will just go down to, well, A is the best thing to do, like according to the systems before. Because there's a lot of numbers in there, I guess. So it should be hopefully finding some optimal thing based on whatever data we do have. And so then it becomes a question of, do we want to do this or not? And, you know, that's usually a fairly simple thing to think about and answer.

**Alberto**  
I also think that you have to add some kind of layer where blocking objections is not just saying I'm blocking and you just say one word or something. It has to be kind of also the commitment to get rid of that blocking objection. The thing is, you cannot force people to do stuff, right? This is also something, maybe somebody's just not equipped to do something. or to remove the own block that it's set. But that's where I'm at right now. I've tried to think about this, or we've tried to think about this in the group, and it's that. It's like committing. Of course, the first layer is that what we are doing here, people that are interested. Like we are right now good faith people, like we meet and we try to work on it, right? So that's the first layer. And then the second layer would be, yeah, I object, but I actually want to work through this with other people that are, that are willing to work with me and then to remove this block that I just said. This is something that is one layer, but also the next layer would be not just blocking objections, but also describing the problem and also sourcing it. I think sourcing stuff is one of the bigger things because You can have a blocking objection, but it cannot be the same waiting mechanism for a blocking objection that has nothing to go for it or something that is heavily sourced by science. You know what I mean? Like if you have so much going for it, then at some point this blocking objection is legitimate. You know what I mean? And that's also another layer that would prevent this. But then again, I also think about it from the other side. Well, there are fringe cases where you cannot apply this and then it gets a little bit messy. But then again, like we have to keep the bigger picture somehow in hand. Yeah.

**Sabrina**  
Maybe what I wanted to say earlier, maybe it's a good idea to start with, uh, with the faith and good faith actors, uh, right now. And, um, yeah, to maybe postpone this also a little bit because we can't have all the answers right now. Yeah.

**samw**  
Yeah. But one thing about that point, sorry, go ahead, Marcus.

**Marcus Barrick**  
I think it's good that we have module 3 and 4 beforehand to build knowledge so that a blocking objection has to reference things. We have different types and subcategories that would get added on. So I think a proposal or an objection would really have to speak to many of those. And then if it can't, I think there's more possibility to reject it or something.

**samw**  
And one thing about blocking objections that are valid. In module 6, there's a quantification of severity and scope of objections. So these things are intended to be measured so that the ones that are actually valid do hold up as blocking, and the ones that aren't don't. And that does sound kind of tricky in measuring how valid someone's blocking objection is, but at least the intent is for an integral is to program it in so that it doesn't even have to be a subjective debate, really. It's kind of quantified in that way, made objective.

**Gary Kent**  
Peter mentioned five consensual levels at some point in one of the documents.

**Ben**  
So do we have them at hand?

**samw**  
I think.

**Ben**  
for module six after module five, where you have the objections, module six is a weighted consensus engine. So I think that is where it says it synthesizes preferences and objections into a non-coercive mathematically transparent decision signal. So it's kind of, when it does that, I think it must have some kind of mechanism for doing that. It says it evaluates the strength of support across participants for one thing. So I guess that would be like someone has very strong support of maybe painting the building orange and then most people have like rated very low and it evaluates that and says, okay, most people think this is non-important, so it should not be done, I guess.

**Alberto**  
Is that what you're saying? Do you all also think, it's just a question in that direction, that at the end with the consensus, we just get a number between zero and one? Do you have the impression that's how it works? Because that's how I see it. Like we have this one number between zero and one, and then we have thresholds. And if this number is above this threshold or below this threshold, then something happens.

**samw**  
Yeah, it explicitly says that. That's how it works. It's a more complex calculation with multiple factors. The objections, how valid they are, the preference gradients. I think that's like negative three through positive two or I forget something like that. And then there's also an option for participant weight, where someone votes. And if someone's an expert, possibly in certain situations, their score counts for more. All that's calculated. You get a final score, and that's compared to thresholds and the other scores of a proposal. And if three proposals are good, but one score is higher, we go with that one. And these are also, the three possible outcomes, I think, are approved, revised, or sent to module nine. I think those are, anyways, yeah, you get a score for each scenario. They're ranked and sorted into different outcomes. And then one is kind of just objectively picked from there. That's, I think.

**Gary Kent**  
I think understanding those things, though, defines pretty much for us certain aspects of Module 5 that have to be present. In particular, you have to have some kind of a decision process that arrives at the people that are going to make the decision. And they need to be listed in the record, as well as their particular consensus position on the issue. So you need a space to have that participation discussed in. And you need to know who decides. I mean, this is kind of something that's related to... the tragedy of the commons, when you have several people participating in some aspect, one of the clear things that has to happen is clearly defining the ones that have responsibility for making the decision. And in this case, we have to include those in the record. And probably every time they change their position on their consensus opinion would have to be recorded in some way for future references. This is why there's so much data involved in all this.

**samw**  
I think that might be what Module 7 does, possibly.

**Alberto**  
I thought Module 7 is just the record keeping, right?

**samw**  
Is that not what he was, maybe I misunderstood, is that what he was referring to?

**Gary Kent**  
No, that's when you, yes. I mean, that's when the thing gets recorded eventually. But everything leading up to that from module one all the way through to module seven is filling out all the data and fields that need to be preserved for future references.

**Lukas Orsvärn**  
Yeah, it's a bit confusing in that sense, because it's not entirely a pipeline. So it's not like 1, 2, 3, 4, 5, 6, 7. So for module 7, it says at the start of the chapter that module 7 creates a temporary evidence historical record of every stage of the CDS process. So I think it does do that, like you were saying, Sam. Module 7 would kind of just archive if someone... you know, sends in a report, it's module seven that records that and stores it kind of, which is, it's an interesting way that this white paper is constructed. To me, that would kind of be implicit in some way that yes, you know, the data is stored. So I'm not totally certain about it, but it also lists kind of interesting pseudo code for, you know, just, validating the integrity of a chain, for instance, and appending stuff to a log. So it's like, it is a very basic thing. It looks like it's just like module seven is the database, I guess. It's kind of what I gather from it.

**Marcus Barrick**  
I'm curious if you could explain how you guys have like ran through it or simulated it.

**Alberto**  
Yes, I would maybe even love to share my screen and show you the GitT pipeline. But yeah, I'll take a second for that. So you can talk a little bit and I'll just jump in when I'm done.

**Marcus Barrick**  
I was curious, I forget which module it was, but I think module 8 where the proposal gets sent to OAD. I'm curious if you guys think that like OAD is kind of like out of the picture until it gets like the requirements or if like OAD would kind of be the one or maybe one of those that would like propose it at the earlier set. Just sort of like the technicality of it is like feasible in the, you know, the decision making process. So it is the one that's actually building things, right?

**samw**  
It's probably a two way street, right? Feedback into each other.

**Gary Kent**  
I guess as human beings, it's going to be us that's going to be the important aspect of this eventually. If everything gets automated and we get these large language models, and this is a question I had to ask, I need to ask too. I'm not as familiar with what's going on on GitHub at this point in time. Is the actual programming going to be basically asking the AI to write the modules?

**Lukas Orsvärn**  
Right now, there's nothing going on on GitHub. I know that. But when we do write things, I assume that we're going to be writing it, that we're not going to be using LLMs to do it just for us. I don't think that's a good idea because it doesn't produce very easily maintainable code and stuff. And it's important that we know exactly how it works and things like that. So we can definitely use LLMs as a tool when building it, but it's not going to be just like... giving the LLM just like a diagram and then it builds it for us or something. That's at least I hope not how we're going to make it because that would be a very bad idea.

**Gary Kent**  
I'm just curious. I don't completely understand the relationship of the LLIs, largely LLMs, to the programming.

**Lukas Orsvärn**  
Where they come into the picture is to understand text, essentially. If someone writes a comment on something like, oh, we're going to build this shed, and someone's like, I think the shed is an excellent idea, blah, blah, blah, in text, then an NLM can look at that text and go, oh, this means that the person is somewhat positive to it. And they can categorize that. And then later on in the process, people don't have to necessarily... you know interact specifically with the like one two three four five things and stuff like that you can kind of get an idea of the consensus so people don't have to read through all that text and try to categorize them manually and stuff like that so it can help with things like that and other similar things where there's usually usually text is what they're good at i guess Nothing really pops into my mind as to what would be good, but that's an example, for instance, of where LLMs could be used to automate things. But in that case, we wouldn't train an LLM for it, I don't think. I think we would use an existing LLM and integrate it into the system in that case. Always to automate something that otherwise humans would have to look at it and just do a bunch of repeat work that we don't want to spend time on.

**Alberto**  
Specifically, module two would be an LLM work, I would say, like structuring, reframing. That's something that would be more accurate under an LLM. I found the webpage we are working on. I'm no expert on the IT part, so I'm going to share my screen right now. And I've worked with somebody in the German in in a german tzm chapter in a german activist group that that we are and and the guy that did this is an expert is an i.t expert i think yes and yeah i i'm like i said i don't know my ways with kitty or github but as i understand it you you put you you can kind of like put make like a pipeline here so it's this is how we um solved it but but like i said please bear with me i cannot answer too much questions when it comes to the technical part but we kind of just like started with having like this um this issue that you can, the proposal, right? You can write here every step of the proposal that is suggested in integral. I'm not going to go into the details because it's also in German, so it's kind of hard to to translate, but yeah, you do the proposal first. This is how you do it. And then after that, then you change the label of this, of this proposal from, I think directly to module two. I don't know why we don't have module one, but it's kind of that way. So we change it to module two and that does the structuring. That's where a bot brings in semantic links. This is also talked in the white paper. There's some kind of also semantic links that are fed back into the system before module three, mind you. So this happens when you set this label to module two, you get semantic links and you also get these structured questions where you restructure what has been written up here. And this is how we did it is we oriented ourselves by using the minimal version. So this is not done by an AI or an LLM. This is just actually the questions that need to be answered. on how to restructure what is up here so somebody needs to do this and somebody just copies these questions out uh paste them in the next issue or i don't know if it's called issue i'm just going to name it that way and then then a person manually has to write down has to restructure the the The data that was put in first, the proposal. So, and after that, after somebody has done it, how do you say? A moderator would have done it. And then you put the label onto module three context, and then that's where it starts. That's where three starts, where it gets, the bot fetches information from the FRS and from the OAD commons, and then you still have to manually put it to module four, and then it goes to the constraints database and it fetches there the relevant data that is needed. And then after that, you set it to module five to the discussion. Oh, sorry, that's not how it should work. You set it to Module 5, Discussion, and then you start the discussing. And it's also intended to be done here, so people start discussing here. And this is where we are at at the moment. We haven't continued because, as I said at the beginning of the meeting, we are at this moment where we have to outline the rules in Module 5. on how to deal with blockage and stuff like that. I hope I did a decent job with the summary, so please feel free to ask anything.

**Marcus Barrick**  
You're using it in a social context? Can you explain the group or...

**Alberto**  
This is an activist group. I don't know if you know the TZM, the Zeitgeist Movement. Well, this is some kind of like the German chapter of that. But we're not that anymore into the TZM label in itself. We are more just activists right now. So we just came together under this label and we just try to do all sorts of stuff. uh and right now we are in integral and this is specifically done with with with that in mind so this what we just developed we developed parallel with the with with the simulation that peter has on his on his home page so we we had both open and then we just started to to copy and paste stuff out also and also always translating into german because the it guy that is working with me on this He cannot speak in English or talk in English, so we have to do this translational work first. It kind of sucks, but that's the way how we function right now. Please feel free. Yeah. Yeah. So, so yeah. And, and, and we are always also looking for input, right? So when we're at some point, I also said to Sabrina beforehand, when she was alone in this group doing this stuff, that, that, that we can like, like, like talk to each other and then just, just, just make, make things better, like stuff like that, because we, we, we have a lot of, how do you say, potential here in Germany. There are people that want to do stuff, but they are just held back by the system and stuff and by not having a group to work with.

**Lukas Orsvärn**  
Yeah, it's really interesting to see your approach to it, I think. It brings up one of the things that I've been thinking about, which is how to kind of decide when something happens. Like in what you've done, it's based on, yeah, like it's based on a Git forge, as it's called. Like GIT is a Git forge. GitHub is a Git forge. And someone submits a thing, and it becomes a thing that people kind of needs to respond to in a way. But in the automated system, when I look at, for instance, module 2, there's no way, as I see it, for someone to just be like, oh, this is a thing everyone needs to talk about. You just submit things to it. You just say like, oh, I see that there's a hole in the wall here or whatever. And someone's like, oh, I need a water pipe for this thing. Or like, I don't know, whatever. And then module 2 structures, just issue structuring and framing. And I'm not entirely sure. That's one of the question marks that I have of like, how does that happen actually? And how do you do that manually when you can't do that? Do you have a thought about that? Like, have I misunderstood how it works? Or do you have a thought about how that works in your system? Or does someone else have a thought about it?

**Ben**  
The pseudocode actually says that it's using a... llm i think to do that based on on a keyword where it kind of matches up keywords in the proposals and kind of groups them into clusters yeah and that clusters them but when is it decided that a decision needs to be made about something

**Alberto**  
Yeah, for our system. Oh, sorry.

**Ben**  
No, go ahead. Okay, I'll just go quickly. So my understanding is that you have the clusters and the clusters are then passed on through the module. So like the cluster would eventually reach module five, and then you'd have a decision made on or like a discussion type thing. Sorry, go ahead.

**Alberto**  
I don't know if I've understood Lukas correctly. Like for the version we have right now, everybody needs to get a GitT account. But I myself, but everybody's going to be notified. Notified. Not notified automatically, the people that are in these kinds of issues. I don't know how to call them. But where I see it in the future, I see it in your direction. It has to be some kind of a different interface. There still needs to be a backbone, a digital backbone somewhere. But for the most people, it has to be some kind of app. It has to be some kind of just, yeah, there's this issue. i have and i have to to set the proposal and it has to be for for for maximum engagement and that's what we want it has to be as easy as possible it has to be just a form really really easy or even maybe like really in the future, even maybe an LLM that you just asked, oh, I have this issue. And then the LLM just asks specifically, so what is the issue? So the next thing and the next thing, and then you just respond in the end. And that's how I would say that the signal intake has to happen at some point for maximum participation. But for now, we are just as lost as everybody else. We're just, okay, GitHub, what is that? I have to get into that.

**Marcus Barrick**  
Yeah. Yeah, actually, I had a chat with Peter in like one of the links that you were talking about the kind of ontology space of this. Like how do we visualize and cluster it? Because I think it's really important to like not just have a list of like issues and problems that just like clogs everything. We almost kind of want to see them in a cluster and then see like if I only care about a certain scope or maybe this thing is important but it's not important to like, I don't know, unless some other thing is done first or like that a year down the road or something like to be able to kind of use some kind of 3D map and add more visuals, more icons. Especially when this scales up, I think it really overrides our cognitive system for reading a lot. So we want to have visual cues and relationship color schemes and stuff just to have more cognitive ease.

**Lukas Orsvärn**  
Yeah, definitely. Yeah, especially when we're building it and working on it, I think that's very important. And then as we go, things will be more and more automated in a sense. And I think in the end, we will end up with something like the ideal system is somewhere where we end up with an LLM who decides on things or who can see like, oh, this is an issue that we need to bring forward to the next step. And then, you know, It keeps going from there, kind of. So there isn't the first.

**samw**  
Also, one thing.

**Lukas Orsvärn**  
Yeah, go ahead.

**samw**  
Sorry. One thing in the video, the Revolution Now podcast, Peter says that this wasn't explicitly written in the white paper, but I think it is in the pseudocode, that there is a step, there's a bridge step between module 3 and module 4. And that bridge step is that automation is used to just generate new proposals just automatically from the previous modules. So that might be an answer to your original question somewhat, Lucas, is like who decides, I think you're asking who decides, who makes sense out of all these submissions into module one and they're structured. There is an automated process where brand new proposals, not made by a person, made by the system are created and move into module four

**Ben**  
Go ahead, Ben. I'm a little bit worried about relying too much on ILLMs for making decisions because they can be biased. Um, as long as I suppose it's, it's just something that is pretty objective, like kind of connecting keywords together and it's okay. But once it becomes something like that, um, can be biased by certain things, it might be an issue. So it might be worth discussing, like before I'm just hesitant of relying too much on LLMs for too much stuff. Right.

**Lukas Orsvärn**  
Yeah. Yeah. I'm also, I'm in the same camp because it's not just bias or like, I guess it is bias, but not bias in the sense that we think of like, oh, I'm biased towards X or Y. Like that's a problem also, but it's also like kind of just like bias in the model itself where it's, Like, LLMs are kind of, they're just, they're stupid. Like, they don't actually think about stuff. They don't know anything. It just puts letters after one another. And so relying on them to do any decisions is very tricky. Something that I've thought about that could be a way to check that is to have a human verification system of things where the LLM is like, oh, this comment has this meaning as I see it. people who use the app, for instance, would get served like, oh, hey, can you help categorize this? What would you categorize this as? Is it like positive, negative, like neutral or whatever, like this statement or whatever? And then it would use what humans say and check that against what the LLM said and use that to help fine tune the LLM towards actual reality. So we can actually use ourselves, like actual humans, to double check whatever automated things we do. just to avoid us getting into the biases and the weird stuff that can happen with them.

**Alberto**  
But I also think... Oh, sorry.

**Marcus Barrick**  
Sorry. I think, like, LLMs in, like, certain layers as interfaces so that it's, like, obvious, like, where the data is coming from. It's not just, like, in the soup of, like, this person in the comment that's, like, specific in this context. But then if it's just a giant LLM, it would kind of just use that and paint it wherever it wants to. So just so it's, like, contextually aware and within the whole stack.

**Alberto**  
I also think it's also... Yeah, sorry. It's important to... to think about the minimal viable system. Also, that actually, if we do that first, then there's no LLM worked into that. But with making a version that is really, really reliable, then we can add on to it and maybe build LLMs in. So, sorry.

**Lukas Orsvärn**  
No, no worries. I just said that yours is the last comment because we're running out of time. We have only one minute left and we should have some closing words. Thanks everyone for the discussion around this. It's been really interesting and I've learned a lot here today. I think... Something that I think a next good step would be to try to kind of start boiling down what we know about this into something that's easier to parse, like I mentioned, or like we talked about in the last meeting. If we have to write it down ourselves, then we will understand it better. And we can also write it in a way that's easier to understand than the way it's written in the white paper, for instance. So that would be my suggestion of what we do next of just essentially taking what we know and in the white paper and what we know and just working on it to kind of boil it down to what is it that it actually is saying, right? There was also talk about mapping things out as well. And I think that can also be done in parallel and we can check them between each other to see if they match and also with the white paper and so on. What do people think about that? Is that a good path forward or does someone have another suggestion?

**Gary Kent**  
You're asking for a description of all five systems?

**Lukas Orsvärn**  
I just focused on the CDS for now.

**Gary Kent**  
Okay. Okay.

**samw**  
that sounds good probably that would just be on github you mean yeah i think so yeah uh it would be in github do you have any ideas for the next meeting

**Lukas Orsvärn**  
I think if we start with this, then I think that will raise questions and we will have more to talk about then about it. Because then it's also easier because then we have something to talk about and we have a shared understanding of it, like literally written down. And then if we write it down, maybe someone's like, hey, I don't think that's right. Or, you know, or maybe we should have something there or whatever. So that makes it easier to have something to talk about and actually something to work on in a sense. That's the way I imagine it in a way. Except two things. Yeah, go ahead.

**Marcus Barrick**  
You mentioned two things, and one of them was a subsystems map. So is that within Mermaid, or is that still a GitHub thing?

**Lukas Orsvärn**  
Both. So Mermaid is just code, right? So that would be Mermaid code on GitHub, I guess, in that case. I think the idea, if we need to have a nested thing, because Mermaid is kind of a node-based thing where you have a thing that points at a thing and stuff. And Peter mentioned you can have hyperlinks on them. So you can have a node and you click on it and you get into that and you can see what that contains and so on. I think that could be something that we could use for this as well. That's a good idea, I think. Could be a good way to help show the information flow and how things link together and stuff, I guess.

**Marcus Barrick**  
I don't know about you guys, but I'd be open to doing 90 minutes for the next... I could even stick around today.

**Alberto**  
I wanted to suggest that. I would say 45 minutes and a five-minute break and then 45 minutes again. That's kind of like a sweet spot. That's something that I've experienced as a sweet spot. I second that very much.

**samw**  
I'm cool with whatever you guys want as far as time.

**Gary Kent**  
If you're asking us for homework to put something on GitHub, I'm going to need some help understanding how to do that.

**Lukas Orsvärn**  
Yeah, let's talk about it on Discord and stuff. Let's try to keep all the discussion about it in this meeting, in the thread for this meeting, so that everyone knows where to find the information. And we can try to, you know... get everyone where they need to go to know what we're doing. But right now, nothing exists. I think Regis made a repository, at least. I just read his comment about it.

**Ben**  
Oh, yeah, he made a repository, yeah.

**Lukas Orsvärn**  
But yeah, there's nothing there yet. But let's talk about it in Discord and try to get something up so that we can start working on it, if people think that sounds good. All right.

**Alberto**  
I just have one last question. Just asking if everybody's okay if I can join you weekly or did I talk too much?

**Lukas Orsvärn**  
No, you're very welcome, I would say. It's highly unconventional. You haven't gone through the process, I guess. I did apply, though.

**Alberto**  
So it's not that I didn't apply.

**Lukas Orsvärn**  
Yeah, but I think for me, it's totally fine. Yeah, it's been good to have you here. So yeah, thank you for joining.

**Alberto**  
Thank you, all of you. I love to talk to people that are like-minded like this.

**Lukas Orsvärn**  
Yeah, likewise, likewise. All right. Sorry for going a little bit over time. Thanks, everyone, for joining today. Let's continue in Discord and see what we can make. See you, guys.

**samw**  
Thanks, guys.

**Ben**  
Thanks, Lukas. Thank you.
