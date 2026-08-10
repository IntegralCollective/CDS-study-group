# Weekly Meeting 11 Transcript

2026-08-09

Note: This transcript was created by an LLM (large language model).
It has transcribed wrong in some places,
and sometimes says the wrong person said things.

**Lukas Orsvärn:**\
Hello, and welcome to the 11th Integral meeting.
Today, we're going to continue with what we've been doing so far,
which is to go through the stuff in the study group.
We're going through the modules and answering questions and stuff like that
as best we can.
So we're going to take the first half of the meeting.
So first 45 minutes to talk about module three and what we have there and see
if we can get more clarity on that.
And then we will see what we do with the second half.
Maybe we continue with that or we move on to something else.
And that's the plan.
So I am going to stream my screen.
Oh, actually, yeah, I can do that.
No, I was like recording.
Now, can I stream also?
But yes, of course I can.
This is 2026.

**Alberto:**\
Hello, lovely people.
Hello.

**Lukas Orsvärn:**\
Welcome.
Welcome.
We're just getting started.
I just said that we're going to take the first half of the meeting to look at
module three and what we have there.
Oh, that's the one button.
All right.
So I guess the best way to start
or the best place to start with this is to look at the open questions and see
if we can answer some of those.
I think that's a good place to start.
I'm not sure who put in what question because I think it could be the case
that Marcus Barrick put in many of the questions and he isn't here today.
So it might be hard if we don't understand it entirely.
So in that case, I guess we'll just skip it.
But let's just start from the top otherwise, I guess.
So how to display data.
How is a code base intended to automatically display
and make meaning from any kind of ecological metric data?
Any different ecological region slash system would need different ways to
display it and its data would be in different forms.
Are we assuming AI can display any data type?
Do we have any thoughts about this one?

**samw:**\
If anyone knows what that question means,
I'd like to hear an interpretation of it.
Not an answer, just what it means.

**Alberto:**\
I would have a basic question that may be related to this,
but not directly to this one.

**Lukas Orsvärn:**\
Okay.
So I guess I can try to explain how I interpret this question.
It's a sort of a visualization thing, I guess.
Like how is it visualized?
But if it is, then I don't understand the question either, I guess,
because I mean, I guess it would be visualized, right?
In whatever way that data would be best visualized.
And I don't think we need AI for that.
Like if we're visualizing temperatures, you know,
there would be like a graph like that or whatever.
And if we're visualizing, I don't know, something else,
we would use whatever the best way to do it would be, I guess.
So yeah, maybe you're correct.
I mean, we don't really know what the question is.

**Alberto:**\
Yeah, also the question is like,
like if we see what module three is intended to do, like it's the stuff it does,
it happens in the background.
It's usually is not displayed anywhere.
Like, or at least I didn't understand it as a module that way.
So yeah, I kind of guess that that's up for questions.
So how do you, how do one get access to the data?
Maybe that's a more appropriate question, but I don't know.

**Ben:**\
In the example, he gave, he gave a few of them.
One of them was corrosion logs.
So they're building, they're building a,
I think it was a greenhouse or something or a tool shed.
And then they have a record of the corrosion logs, I guess, of the tools,
how much they're getting rusty over time.
So that must be stored somewhere.
They must keep accurate logs, like over time,
it's like one tool maybe is 80% rusty after four months or something.
And then I guess what they would do in the,
in the knowledge thing in module three is they kind of integrate
that information.

**Lukas Orsvärn:**\
Okay.
Yeah.

**Ben:**\
Does that, does that make sense?

**Lukas Orsvärn:**\
That does make sense.
Does it say that it would be like that module three is responsible
for displaying?
It's because I'm kind of, Oh, excuse me.
What did it say?

**Ben:**\
For, for like a module three on page, I think it's 27,
it gives you example of how that would work.
And one of them was corrosion logs.
Yeah.

**Lukas Orsvärn:**\
I don't have.

**Ben:**\
On page 27, if you're looking for it.

**Lukas Orsvärn:**\
Yeah.
I don't have page numbers here.
Do you know which chapter it's in or something?

**Ben:**\
7.3, I think 7.2.
I don't know.

**Lukas Orsvärn:**\
I guess I'm not finding it.
Okay.
Well, it would be good if you could, I guess, I guess, can I find, I have,
let's go, let's go here.
I can download the PDF here.

**Ben:**\
That's easy.

**Sabrina:**\
Then you have page 27. 7.1.

**Alberto:**\
Module three.

**Gary Kent:**\
Also with designs, with designs,
a lot of those are going to be stored with ecological data based on whatever
they are.
So if you're talking about creating a tool or an item or a building
or a process, there's an ecological assessment that goes into designs
before you actually put those into the design ledger.
So that could be where some of the ecological assessments are coming from.

**Lukas Orsvärn:**\
Oh, but is it not in the CDS that you're finding?
Yeah, it is in 7.1.
I can't find the word corrosion in this page.

**Alberto:**\
I don't think it is.
Oh, it is.
It is in the example.
The system compiles airflow data,
corrosion logs in the module three knowledge and integration.

**Lukas Orsvärn:**\
All right, I'm going back to the PDF.

**Alberto:**\
Yeah, for me, there's a more basic...
Oh, this is the wrong PDF.

**Lukas Orsvärn:**\
Okay, never mind.
Yeah, because this is another PDF that I built.
So it's not the correct page numbers either.
Okay, this is very confusing.

**Alberto:**\
For me, a more basic question, or at least I think it's more basic.
How is it actually done?
So does module three go and retrieves the data
or do the other systems feed it into module three?
I have no idea how this would work digitally or in that case.
Can anyone tell me how it's usually done?

**Gary Kent:**\
I think in this case, we're looking at one particular issue
that we're dealing with in CDS.
So we have to think about it as a particular issue,
which will have a certain ecological profile.

**Ben:**\
It could be by AI or it could be by humans, I guess.
In the AI case, it would be okay.
It has a keyword, which is like tools.
And from that, it can kind of get the relevance of maybe corrosion.
And then it's okay.
We have data here about corrosion.
And then it will kind of link those.
Or if it were a human, I guess the human would say, okay, I'm looking at tools.
And then we have all of this data stored in our database regarding corrosion of
these tools that we have.
And then you link that manually.
I guess it would have to be like, that would be the process.
So it wouldn't be super simple.
But I think it would involve some kind of linkage, I guess, like that, right?
So like, as soon as you have a decision issue,
then someone would have to make that linkage to previous data for
that decision issue.
Or an AI would do it.
Does that not make sense?

**Alberto:**\
How do you define decision issue right now?
What's a decision issue?

**Ben:**\
Like a cluster of submissions.

**Alberto:**\
After it went through module two.

**Ben:**\
Right.
So you have a cluster of submissions, right?

**Alberto:**\
Yes.

**Ben:**\
Which becomes, that would become a decision issue, I guess.
That would have to be decided upon.

**Alberto:**\
Okay.
Okay.
Now I understand.
Yes.
Okay.

**samw:**\
But that's just the process of module two, right?
Isn't that just what module two does?
It makes it that?

**Ben:**\
Yes.

**samw:**\
So there's a question how it gets from module two to module three.
Or how it presents itself once it arrives at module three.

**Ben:**\
Sorry, go ahead.

**Alberto:**\
No, sorry.
Please continue.

**Ben:**\
Well, I say how I envision it.
It just goes through the module two.
And you come out with a decision issue,
which would be like a cluster of submissions.
And that object automatically goes to module three.
And then it has to be linked to previous data
that is related to it in module three.
Does that make sense?

**samw:**\
I think it does make sense.
I'm just thinking about the linking part.
I guess that's pretty straightforward.

**Lukas Orsvärn:**\
And what was the original question about this?
I think I missed it because I was looking for the white paper.
I guess maybe no one remembers.
That's fine.
Hello.
Sorry, I got kicked out and in again.

**Alberto:**\
I was also, or we were also kicked out.

**Lukas Orsvärn:**\
Oh, okay, cool.

**samw:**\
Does that happen every time a new person joins?

**Lukas Orsvärn:**\
I hope not.
It's just a Discord bug, I assume.
My entire Discord crashed, so.
But either way, yeah.
Let's get back to the thing we were talking about here with how to display data.
Ben, you were talking about in the white paper, which I now have here.
You were talking about this example.
This is the thing you were talking about, right?

**Ben:**\
Right.
So his example was corrosion logs.
So it's just a matter of linking those to the issue, to the cluster, right?
Is that all there is to it?

**Lukas Orsvärn:**\
Yeah.
But yeah.
And in the question, the thing
that I guess is a question mark in the question is, it asks how to display data.
And the thing I'm thinking about, like, yes,
it says here that it compiles the data, and the data reveals something.
But it doesn't say that it displays the data.
And I think probably that maybe happens in a later module,
because there is a module where there is a humans deliberating, right?
Something like that.
I don't remember which number it has.
And maybe at that point, it makes sense to visualize it, perhaps.

**Ben:**\
Yeah, I think that's correct.
It would probably just be in the back end at this point.
It wouldn't be displayed anywhere.

**Alberto:**\
Yes, that's what I also thought.
Yes.
The same for two also.
Like, in a minimal version, you would have somebody doing it.
But also, two would be in the back end.
Three would be in the back end.
Four would be in the back end.
Actually, it's just one and five where people come in,
and nine when it's further deliberate.
Yeah.

**samw:**\
Should we make a note of that in the GitHub,
of which are back end and front end?
That might be useful.

**Alberto:**\
Yeah, I think that's a good idea.

**Lukas Orsvärn:**\
Yeah.
Okay.
So, unless someone has a complaint, or however you want to put it,
we will say that, I guess, the answer to this question, how to display data,
is that it's not supposed to be displayed in this module.
It's actually displayed later on.
The question still applies, I guess, for that section, probably.
But it's not a module three thing.
So, I guess we could maybe move that to the module where it belongs.
And yeah, like you suggested, like was suggested,
it could be a good idea to include if a module is like a back end or front end.
So, moving on to the next one then.
How is data integrated?
How is the ecological data integrated with the resource availability, capacity,
labor data in a meaningful way?
In order to search for the right resources slash gain insight on the labor
specialization needed.
I imagine OAD would need to be involved.

**Alberto:**\
Like all systems would be involved, right?

**Gary Kent:**\
Again, it's talking about the design ledger where all the designs are stored.
And there's probably a particular design,
if they have gotten that far with this issue, that's associated with this issue.
So, then there would be that kind of data stored on that original design.
And it may have to be modified as a result of the process,
the decision-making process here.

**samw:**\
It is kind of just collected, though, in module three.
Isn't that the point?
Just like a collection to not do that much, ostensibly.
Even though I think it actually, in the fine details, if you look at it,
it kind of implies that it is doing something.
But what does integrated mean?
Does integrated just mean clustered like in module two?

**Ben:**\
Let's say that it...
Go back to the previous question for a second.
Let's say that it is displayed and AI is not involved
and you just have like a view of related data.
So, like you have this issue for creating a tool shed
and then someone has linked related data to it regarding corrosion logs.
So, you look at it and you see, okay, this is related data.
Is that...
Would that be like the manual way to do it?
And then you just look at that and then that's done?
Okay, I see there's corrosion logs.
Maybe we need to take that into account when we make the decision.

**Alberto:**\
In the minimal viable version, this module is deferred.
It is described as something that would be integrated later on.
And the minimal viable version is the version that is said to be the one
that is done fully through humans without help or at least technical help.
But you could use AI and stuff like that.
It's not about that.

**Ben:**\
So, to make it simpler, in a minimal viable version, then you could just say,
okay, this is the tool shed cluster and we have corrosion logs.
So, that would be module three done.
And you could just display that somewhere on the screen.
And then for integrating it,
it would be a question of looking at the corrosion logs and seeing, okay,
there's a lot of corrosion.
We need to give more airflow manually, right?

**Gary Kent:**\
It could be one scenario, one solution path.

**Ben:**\
I'm just trying to keep it simple because it can get really complicated,
I think, if you get, because there would be a lot of different ways of
integrating stuff.

**Lukas Orsvärn:**\
Yeah.
And that's a question I have with this question is,
what does integration mean here?
What does it mean?

**Alberto:**\
And I think it's not only related to OAD.
It's related to actually every system.

**Lukas Orsvärn:**\
Yeah.
And something I'm also wondering about with this question is,
in order to search for the right resources slash gain insight on the labor
specialization needed, but module three doesn't do that, right?
Module three doesn't care about what resources are required
or what labor specialization is required
because that's too early in the process, right?
Module three only gathers data.
So it doesn't, it doesn't have any scenarios yet,
which would involve spending certain resources
or need certain labor specializations, for instance,
or am I misunderstanding that?

**samw:**\
I think it shouldn't, and it would be consistent if it didn't,
but it seems like the way it's written, it's implied that it does,
which it shouldn't, but it kind of seems like it does.
Like things like external resource dependency.
Dependency is resource requirements, it seems like.
You're searching for the right resources, you kind of,
it presupposes that you need to have,
need to know what resources are required in order to seek out
where you need them from.
But you're right, there's no scenario to base it on.

**Lukas Orsvärn:**\
My interpretation of that, what I think you're referring to,
is that that's just talking about like making,
painting a picture of what are we working with here?
Like gathering, gathering the data of what resources do we have?
What labor do we have?
It's not saying we need these resources or we need this labor.
It's just saying we have 100 units of wood
and we have 50 hours of labor in these times or whatever, you know,
stuff like that.
But it doesn't say, oh, we actually need them.
It's just as if paint like makes the frame of this is what the later modules
will have to work with and they have to stay within that frame because otherwise
it's, there's whatever solution they come up with, it won't matter kind of.
That's how I interpret something.

**Alberto:**\
It does.
Well, there's this step 3.5 or this bridge step that Peter built in.
And that's where actually 3 does exactly that.
While it sends it to 4, it kind of comes up with scenarios itself, right?
And these scenarios are the scenarios
that are then tested then in 4 against constraints.
So it's true that 3 doesn't do that.
But 3 does the basic groundwork for this step to happen.

**Gary Kent:**\
I think those scenarios come from a lot of different places.
Some of them can come in in terms of proposals from the very beginning in the
submissions.
Then some of them may come in from the designs of whatever they're working on,
if that's associated with the issue.
And then once you get to module 5,
people are sitting there and they're discussing all this and they say, well,
I have another idea.
We could do this instead or maybe we could modify this proposal and try this
as a scenario instead.
So if they do that, one of the things that's going to have to happen from module
1 is that issue is going to have to be run back from module 2 all the way
through for constraining and everything else.
So there's going to be this constant process of looping the issue through all
the first stages as the decision is trying to be managed.

**Lukas Orsvärn:**\
Yeah, I believe that's correct as well.
In terms of this question specifically,
I feel like we have a few questions about the questions,
about the question itself.
I'm not sure if we can get much further on it.
Does someone think that that's incorrect or should we move on?
Should we?

**Alberto:**\
I would have just a basic question, the one that I had before.
How is the data managed?
Is it retrieved by 3, module 3?
Or does other systems and other modules give it to 3?
How does that work?
Or do you have an idea?

**Lukas Orsvärn:**\
I think in this case, it's worded in this case, in my opinion,
as if module 3 gets the data.
But in practice, it doesn't really matter.
That's kind of an implementation detail.
I think also the way that, for instance,
module 1 is laid out in the white paper is probably not how you want to do it.
I don't think you necessarily want to associate every piece of evidence with an
issue, for instance.
Maybe all the evidence is just in a flat list
and then they can be associated with an issue at some point, maybe in module 3,
for instance.
Because then that's when it starts mattering, kind of.
So if there's a broken shelf somewhere, I can just take a picture and be like,
there's a broken shelf.
Okay, cool.
It doesn't need to be associated with an issue.
But right now it does.
So that's an example of something that maybe that's just a thing
that lives alongside everything else.
And things are just like taking stuff from it when it needs.
And it doesn't necessarily need to be related to a specific module at all,
for instance.
But yeah, whether it gets the data or if it gets giving the data,
I think that's an implementation detail,
not something we need to really worry about for understanding how it works.
Do you disagree or agree?

**Alberto:**\
I'm just clueless.
That's why I cannot agree or disagree.
So I just take the word for it now.

**Gary Kent:**\
If the data was requested,
I would think it would be submitted through module 1
before it caught up with the issue.

**Lukas Orsvärn:**\
Okay, let's move on to the next one then.
Why is the OED missing from the pseudocode?
The OED is said to be involved in module 3 on page 24 of the white paper,
but it's left out of the pseudocode.
Is this a mistake?
I haven't looked into this one specifically myself, but I can look at the page,
page 24.

**samw:**\
It's not 24 of the PDF file.
It's 24 as listed in the actual white paper.
Do you have page numbers on there?

**Sabrina:**\
No page numbers.
No page numbers.
Okay.

**samw:**\
Well, it's page 27, I think, then of the actual PDF.
All right.
Thanks.
It's where it says safety standards, architectural constraints,
design references from OED in the bullet point.

**Alberto:**\
So it is not missing, or what's the point?

**Sabrina:**\
In the pseudocode, it's missing.

**Alberto:**\
Oh, okay.

**Gary Kent:**\
Well, the pseudocode is kind of random throughout.
Sometimes it uses it to really highlight details, and sometimes it's missing.

**Lukas Orsvärn:**\
Oh, yeah.
I think something that's good to understand,
and maybe that's a misconception that people have,
it's an easy misconception to have, I guess,
is that the pseudocode is not comprehensive.
Like, it does not cover everything.
The pseudocode just covers a few key parts
that Peter thought would be important to have pseudocode for, I guess.
But there would be many, many more functions and much, much, much,
much more code than what's in the pseudocode,
so even if it's shown here as it's taking something from OED
and it's not represented in the pseudocode, that's, to me,
not something to be worried about.
In my opinion, not even worth having a, like,
it's not an inconsistency in some way,
because there's a lot of things that are not in a pseudocode.

**Gary Kent:**\
I can give you some good examples of that,
because I've been working directly from the possible schemas,
and what I do is that when I find a particular reference
that might be some ledger data that you want to record somewhere,
I have been searching through all the white paper
and the development guide to find every reference to that particular term,
and some of them are just missing.
For instance, governance is mentioned at one place as a major data schema
for this module, I think, and, or for, not for this module,
but for the subsystem.
And if you look up governance,
there's a lot of references throughout the white paper and the dev guide,
but they're basically descriptory.
They're not, they're never defined as a data set or a variable of any type.
When you look at, like, governance, I think,
I can't remember the term right now.
I can look it up real quick.

**Lukas Orsvärn:**\
Yeah, that's another example.
Which is, for the most part, fine, unless it's some, you know,
important central thing that we need to know what it is,
then we should try to define things as best as we can, I guess.
That's my opinion, anyway.
That's fine.

**Gary Kent:**\
There's, there's listed in one part of the,
where they list that table of CDS pointing to FRS,
and he calls it the governance signal.
If you look up the references for that, you won't find any real reference,
any data related to that.
That's in the development guide 4.2, the core data contracts between systems,
is what it's called.
And you won't find any kind of a pseudocode for a governance signal.
I haven't been able to find it anyway.

**Lukas Orsvärn:**\
Okay.
Yeah.
That could be, could be worth mentioning.
It could be something that's just fine,
that it's not covering everything everywhere, I guess, on every front.
But in terms of this specific thing,
where the OAD is said to me about in module 3 and page 24 of the white paper,
but it's left out of the pseudocode.
Is that a mistake?
My answer would be, it's probably not a mistake.
It's just not everything is expected to be in the pseudocode that's also
elsewhere in the white paper, kind of.

**samw:**\
Should we add it to the GitHub module summary?

**Lukas Orsvärn:**\
I'd add the OAD stuff.
Yeah, let's do it.
And what did you say, Sam?

**samw:**\
I was just asking if we should add this OAD related stuff to our module 3 GitHub
summary simplification.
It's not in there right now, I don't think.

**Lukas Orsvärn:**\
Yeah, that could be something worth adding, for sure.
I'm always, my perspective is always whatever makes it easier to understand
should be added.
I don't think for, like for that purpose or for that reason,
I don't think everything should be there.
Like there are many things that don't really make it easier to understand,
but yes, it's specified in the white paper, for instance.
So that's, in my opinion, one of the things that we should weigh.
But yeah, it's a case-by-case basis.
In terms of this specific question, though, yeah.
So my take on this specific question is that I don't think it's a mistake,
and I don't think we need to worry about it.
Do we have someone who has another take on it,
or should we move on to a different, to the next question?

**Alberto:**\
I'm okay, you could move on.

**Gary Kent:**\
I was just going to comment that
if we make a mobile app that's going to be the main interface between people
and the Integral system,
we're going to need a mobile app guide to help people know how to interact with
that.
And that's going to be probably, you know,
a version of the white paper in the dev guide.

**Lukas Orsvärn:**\
Okay, thank you for that comment.
So moving on to the next one, then.
And by the way, I should also add, the reason, like at the end,
I'm summarizing it like that is to make it just clear where we are.
And it also helps with, like, the transcription,
people reading the transcription, people.
And then we have the summary, automated summary and stuff like that.
So it helps with all that stuff.
And also to check if people have anything to add as well.
So there's several benefits to that.
So yes, next question.
Where does historical data come from?
Is the historical data and rationale sourced from previous instances of this
node, perhaps from module 7, or from outside cases where these projects were
done?

**Alberto:**\
I'd say both.

**samw:**\
I agree.
I mean, the external data sets could refer to,
it mentions external data sets as an input that could refer to outside cases
where these projects were done.

**Lukas Orsvärn:**\
Yeah, I think it could be either.
And I'm thinking if it's possible, it's good if outside cases could be used.
But it's also, like, one of the things with Integral is
that it collects a lot of data so that you have that moving forward.
And the way we work right now in the current society,
we usually don't collect that much data,
at least not in a way where it's meant to be, like, shared on and stuff.
So, like, if a company builds a greenhouse,
it's not like they keep track of exactly how many hours it took to, you know,
build it and how many people and what are exactly all the resources
that it took to build it and stuff like that.
So, it could be hard to do that,
but probably if there are no other things to go on,
I feel like outside cases would be where things are taken from.
But then it's not, like, from a data perspective, maybe.
Maybe it's more like a reference thing, perhaps.
I'm not sure.
I'm just, like...

**Gary Kent:**\
What do you mean by outside?
Outside the CDS system or outside Integral?

**Lukas Orsvärn:**\
Outside Integral, yeah.
That's how I interpret it, in a way, the question.

**Alberto:**\
I interpret it as another node.
It's instances of this node or from outside cases, so other nodes.
That's how I interpreted it.
And for me, the answer to that would be both.
But, yeah, you could be right.

**Lukas Orsvärn:**\
Yeah.
That's what I...
Yeah, so go ahead, Gary.

**Gary Kent:**\
I don't think anybody that was making an important decision would be against
taking information from outside if it contributed to making the decision.
However, I think one of the things that I've come to recognize this week
when I'm trying to understand what these ledgers are and where they exist is
that every subsystem has its own ledger, permanent ledger,
that records everything that happens in that system.
And those ledgers are accessed by other subsystems, for various reasons.
So that's where a lot of the data is coming from, is those other records,
those other ledger records.
Even in this particular CDS 10-module group, in Module 7,
there's a detail about how every step along the way is recorded in the final
ledger, including the scenario creation and all kinds of things, are actually
recorded in the ledger before everything is all done.
So every step of the way is in history from that point forward, and somebody,
anybody, should be able to come in and access those records of that decision
and all the data that went into making it.
So all the issue, different names they have for issues, the structured issue,
the issue, structured issue,
and I think there's a couple of other references to different types of issues,
will, at each stage, will be recorded in that permanent ledger.

**Ben:**\
I think for a simpler, like minimal viable system,
I think we should focus on the very minimal amount of complication,
just to get this through.
And in that case, it would be, okay, you just submit this information,
the same as you would submit an issue.
So you say, okay, I'm going to submit a corrosion log,
and then that would be there.
You have your corrosion log, and then in step three,
someone looks at the submission and says, there's a corrosion log.
I'm going to link that.
So it's simple.

**Alberto:**\
Yeah, but just to be...
Sorry, Luca.

**Lukas Orsvärn:**\
I was just going to ask, or like say, Ben, just to be clear,
we're not specifically talking about the minimum viable system now, right?

**Ben:**\
But it gets way too complicated if we don't.
I think we should.
What are we talking about then?
Like the full system?
Like after completion?

**Lukas Orsvärn:**\
Yeah.
So the purpose of the study group is to understand the white paper,
essentially understand Integral as it is in the white paper.

**Gary Kent:**\
I think if we don't understand the full functionality of it,
when we try to do the minimum viable system, which is a test,
we're going to possibly miss important data fields.
So we need to be able to define all the data fields.
And the idea between the minimum viable system is that we need to have those
before we actually run the test.

**Ben:**\
But is the minimum viable system not an example of the full system?

**Gary Kent:**\
Yes.
It is from a data perspective.
That's the point of it.
Yes.

**Alberto:**\
But you do have to leave spaces for deferred systems
or deferred modules in this case.
So, like I said before, like what you just said,
nobody would do something in module three.
What would be done?
It would be done in module six in the minimal viable version that Peter offered.
It would be done on module six where everything happens.
You do the discussion.
You look at everything that you have until there, every information,
every constraint and stuff like that.
That all happens in six and also in six happens the decision making.
And this is the point.
So you have one is not deferred, two is not deferred, six is not deferred,
seven is not deferred, and eight is not deferred.
Everything else is deferred.

**Lukas Orsvärn:**\
Yeah, I think a large part of what we're doing
or like why we're doing what we're doing now in the study group of going through
everything is because that seemed to be the thing that we would be doing when we
get back to a real Integral business, right?
We're going to go through all of CDS and stuff like
that to ensure people understand it.
So we're kind of doing a head start on it here in a sense.
Okay.
But yeah, no worries either way.
But it's good that we're on the same page with
that at least of what we're thinking of here.
I have a comment on...

**samw:**\
What's the distinction between historical data and evidence?
Is there a distinction between those two things?

**Gary Kent:**\
Oh, yeah, sure.
Historical data maybe just references other times
when something that's related to the decision that's being made have occurred.
It may not be, it's not evidence of any particular event, but...

**Lukas Orsvärn:**\
Yeah, exactly.

**samw:**\
It's hard for me to separate those things.

**Lukas Orsvärn:**\
If you think about it like...

**samw:**\
Sorry, go ahead.

**Lukas Orsvärn:**\
It's like we're making a decision about the shed.
We want to like, should we build out the shed?
It's too small.
And then it's like, okay, cool.
Historical data.
We decided that the shed was supposed to be built two years ago in June
or whatever.
And here are the decisions we make with that.
That's how we came to that decision and everything around that.
And then evidence would be a picture of the shed
or like the logs of the shed show that we are at 90% capacity
and it's going to go over if we don't make it bigger.
That's like evidence, I guess.
Or maybe someone taking a picture of it or maybe evidence could be, you know,
we couldn't store this thing that we wanted to store
because we didn't have space for it.
That could also be evidence, for instance.

**Alberto:**\
Okay.

**samw:**\
Makes sense.

**Alberto:**\
What about the distinction between historical data in system
and historical data out system?
So this is also a distinction that is being made, right?
Or that needs to be made.

**Lukas Orsvärn:**\
And what do you mean by that?

**Alberto:**\
Okay, maybe we do not have a, like a,
a specific design for a problem in the Integral nodes federation.
But we do have it, let's say, somewhere outside in some report,
in some repository somewhere else.
Also, it doesn't even have to be in the market economy or something like that.
But that's, that's a thing, something that has been done in the past,
but outside of the system.
So, so there also needs to be some kind of like, what do you say?

**Sabrina:**\
Categorization?

**Alberto:**\
No, you have to have this, this, this docking.
Yeah, you have to dock to, to the, to the, to the, to the outside world.
So, yeah, maybe I'm doing it, I'm describing it wrong.
I hope this makes sense.

**Lukas Orsvärn:**\
Well, you're kind of talking about using the outside,
outside of Integral world as historical data as well.
As well.

**Alberto:**\
Yeah, yeah.
Let's say there's some design that was made like in 1990,
that solves a specific problem
that has not been talked about in integrals itself.
For me, I think the question is about the interfaces with the outside part of
Integral, which is maybe not related to now.
So, sorry for that.

**Sabrina:**\
But maybe it just has to be labeled differently.

**Alberto:**\
Yeah, taken in also, right?

**Lukas Orsvärn:**\
Yeah, it's an interesting, it's an interesting, yeah.
It's an interesting thing, for sure, that we, we need to think about as well.
But we are at soon 45 minutes.
So, I think we should take a break now.
And then when we come back, we can probably continue with this.
But let's check in when we get back and see, see what people feel.
So, yeah, let's take a five minute break.
And I'll see you here then.
All right.
I was just going to jump in and continue the meeting.

**Alberto:**\
The five minutes have passed.

**Lukas Orsvärn:**\
So, sorry to interrupt.
But we should be focused on module three.
Or should we?
Because only the first half of the meeting was dedicated to module three.
And we're not done with all the questions.
But I also want to check in with people and see if there's no clear-cut agenda,
for the most part, for these things.
Do people agree that we should continue with it?
Or does someone have a great idea
for what we should do with the latter half of the meeting?

**samw:**\
Definitely do at least the next question,
which in my mind is the juiciest question.

**Lukas Orsvärn:**\
Sounds good for me.
So, yes.
Before we move on, we were kind of like at the end of
where does historical data come from, I guess.
Or, yeah, we're talking about that.
And I just want to kind of wrap that up at least and see if people agree
that we're ready to move on.
So, when I was looking at this, we had different interpretations of it.
So, I interpreted outside cases as being from outside of Integral.
And Alberto, you said that maybe it could be outside of the node.
And in my opinion, what makes sense here
and what probably would be the best way to do it is it depends on what data it
is like that you're talking about.
Because historical data for a specific, if you're talking about this shed,
for instance, it doesn't make sense to have historical data about the decisions
about other sheds necessarily because it's this shed that we're talking about.
But if we're talking about building a shed, then it makes sense to see, oh,
wait, a hundred sheds have already been built in other nodes.
Let's get their historical data about how it went when they built their sheds
and how it's gone for them with their shed since they built it, for instance.
And there's a lot that can be taken from that.
So, I think that in my mind,
the answer to this question of
where does historical data come from would be wherever it makes sense
that it comes from.
So, if it's useful to get data from other nodes, then do it.
If it's not useful, then don't do it.
If it's useful to get it from outside of Integral entirely and, you know,
and there is good data for that and maybe there is no other data.
So, we need to do that in the beginning, perhaps.
Then let's do that.
But that's less of a systemic thing, I guess.
That would be kind of more, you know, bootstrapping it in the beginning,
I suppose.
But, yeah, that's my take on this one.
Does anyone feel like they want to keep discussing it?
Then let's move on to the juicy question, I guess.
Why isn't the context score vector an output?
Shouldn't the context score vector be considered an output?
Or is it technically part of the context model?
Or is it merely symbolic and not actually involved in a module?

**Alberto:**\
Like how I understand it,
this context score vector is then used to help create the scenarios in the
bridge step.
So, in my opinion, if I understand it correctly,
they are already baked into the scenarios that are tested against four.
But please, if I'm wrong, please tell me.

**Lukas Orsvärn:**\
Can you say that again, Alberto?

**Alberto:**\
Maybe I'm imagining this wrong.
But for me, I thought the context vector that or the context score
that it's reached, this is then used to create the scenarios in the bridge step
against the constraints.
Or do I have this wrong?

**Lukas Orsvärn:**\
Sorry, I crashed.
That sounds correct to me.
But I'm back.
But you were saying that you think
that these scores are used in module 3.5 to create the scenarios.
I think it's used for that.
It was a while.
I mean, I've read through all of the CDS when we started this study group.
And I've read through it several times before that as well.
But it was a while since last time.
So, I don't remember exactly where that would be used otherwise.
But in my mind somewhere,
I have the thought that it's also used as a general thing
when you come up with solutions to rate the solutions.
Even if it's not automatically generated, if someone says, oh, hey,
let's use this blueprint from OED to build it.
And that's a scenario I'm going to put together.
Then that scenario will get a rating based on these scores as well, I guess.
But that could be another score that's taken from somewhere else.
And I might be mixing stuff up.
So, I'm not sure.

**Alberto:**\
Does somebody else have an interpretation on how this is done?

**Gary Kent:**\
The context score vector created in module 3?

**Alberto:**\
Yeah.
How is this further used?

**Gary Kent:**\
Can I share a screen for a minute?

**Lukas Orsvärn:**\
Yeah, sure.

**Gary Kent:**\
Can everyone see this?
Yes.
Module 7?

**samw:**\
It's a little small, but I see it barely enough.
If you can make it bigger, that'd be helpful.

**Gary Kent:**\
That'd help.

**samw:**\
Fine.

**Gary Kent:**\
Okay.
Well, I, this is what I came across when I was thinking about
where everything is recorded.
And if you look at this and you read all the things, it records everything.
So, that vector is recorded in one of the system, one of the little issues,
versions, as it passes through the things, it's going to be added to the ledger,
the CDS ledger that records everything institutionally, as he calls it,
institutional memory.

**Lukas Orsvärn:**\
And you're saying that this is where the context score vector is stored?
Is that what you're saying?
Or what's the...

**Gary Kent:**\
Yeah, it may not be definitely mentioned right here in this,
but that's what this whole module does.
It stores everything that is not,
that's related to the issues that this module processes,
and all the stage steps in between, the votes,
all the votes that happened to Module 5,
all the additions and changes to the issue that were added in earlier modules,
all the constraints that were put in.
Everything is recorded in versioned control ledgers.

**Alberto:**\
But to what is this question related?
Is it related to the code that there's, in the pseudocode,
that there's no use of the score?
Or how is this, how is the question meant?
The question in the module 3.
Yes, in the module 3.
Not for you right now, Gary.
It's, yeah.
I want to put it into context of the question, because I agree with you,
module 7 does store everything, right?
And at the same time, I don't know, I don't really know what the vector score,
how that is also further used.
Is it further used, or is it just stored in 7?
Or does it help with the scenario building?
That's the question I would just ask right now.

**samw:**\
I'd just like to interject that confusion I have, which I,
also in the next module, there's another math sketch of something.
I guess this is module, or that, I don't think that's in the pseudocode either.
So I'm confused about how these math sketches at the bottom of these module
outlines are, if in general, not just this one, but in general, they are of
utility for the module, or what they're supposed to be, how they fit in.

**Lukas Orsvärn:**\
Yeah, that's an interesting question as well.

**Gary Kent:**\
Does anybody know what all those coefficient vector data representations were?

**Lukas Orsvärn:**\
Coefficient vector data representations?

**Ben:**\
Let's say that there's some input somewhere that determines, like,
you have a coefficient, environmental coefficient of 5,
and a labor coefficient of 1 or something.
I'm not sure where you would get that exactly.
Someone would have to input that, or it would be AI.
But anyways, you get these coefficients, and then you look at the knowledge,
like the corrosion index, and you say, okay, it's really difficult to do this,
unless you do it manually.
You say, okay, this one, the corrosion index is related somehow to environment,
because it's going to maybe affect, like, leech into the lake or something.
So it has some impact there.
I really don't know.
It's hard, right?
How would you do that?

**Alberto:**\
I wouldn't say hard, but complex, I think.
And to get the big picture, we would have to grasp a lot of concepts at once.
And that's what we are trying to do right now.
So I get you.
It's hard.

**Lukas Orsvärn:**\
Yeah, definitely.

**Ben:**\
Like, for minimal viable, I don't think that some of those, so, like,
you have environmental coefficient, so you just kind of skip that,
because it wouldn't really be applicable to the rust.
And you just end up with, okay, one, it's the same as anything else.
And then you move on.

**Gary Kent:**\
That information is going to have to be stored in some data somewhere.
You even need that in the MV3 or MVS, as well as the full modules,
if it's actually relevant data to making, helping make decisions.

**Alberto:**\
Yeah, but I think in the minimal viable version,
so you wouldn't actually go that deep.
Like, I would imagine in a way that you could actually do it yourself.
You go and you do research, like, you on your own, and this is part of it,
in the minimal viable version.
So maybe you have module three, like, in a blank state,
where you put an A or not available data inside.
But for the purposes of a minimal viable version,
to not make it that complicated, which I agree with you a lot,
you would actually do it kind of conventionally, right?
Doing your own research,
bringing the papers to the meeting where we talk about it and stuff like that.
And if there's already an infrastructure to take this data
that you yourself researched to update it somehow,
then we would gladly take that.
But the node has to be possible to that node.
And as I understand it, nodes are not going to be equal from the beginning.
Some nodes will have more infrastructure to work with than others.
So, yeah, it is going to be messy.

**Lukas Orsvärn:**\
Yeah, for sure.

**Ben:**\
I guess it's possible, like,
you could have a node that has a specific coefficient
where they like power tools.
So, like, they have a very high power tool coefficient
where they want to use power tools.
It's just like an example.
And then when you get to the tool shed issue, they say, okay,
we have a high power tool coefficient.
So we're going to have to have some kind of allowance for more power tools,
I guess.

**Lukas Orsvärn:**\
Is that what the coefficients are for, though?
Like, if we look at the math sketch, and those are being, you know,
put together into the context score vector.
I mean, module three.

**Gary Kent:**\
What page was it on?

**Lukas Orsvärn:**\
I don't know what page, but it's in chapter 7.1 in module three.
It's the inputs it's taking there.
It's ecological indicators, resource indicators, labor indicators,
and social slash fairness indicators.
So I think, like, the rust thing is probably not going to be necessarily a part
of that.
It's more like, I think the coefficients in this case would be more related to
what's more important right now, kind of.
That sort of thing.
Like, just because it's like, what's more important?
The ecological factors or the social or fairness factors?
Like, there is no automated way or deterministic way to determine that.
You just have to agree somehow that, well,
we think it's more important with the social or fairness factors.
So that's, like, a higher coefficient or lower or whatever.

**Alberto:**\
Yeah, I think that's a community thing, right?
This is a constitutional thing that has to happen beforehand.

**Lukas Orsvärn:**\
Yeah, exactly.
That would be probably decided through the CDS,
through a decision process somehow, I assume.

**Alberto:**\
Yeah, that's the thing that I'm a little bit struggling with, but I think we,
this is off topic a bit, because that's the thing.
So we need to have set some ground information for a specific node.
They can do the constitutional outliers themselves, but at the same time,
how is it done?
Is it already done with CDS, or does it have to happen beforehand, before CDS,
so that module 3 and module 4 have some context?
You know what I mean?
Because CDS can only work with, well, the latter part, only works with 3 and 4.
So, yeah, I'm still a little bit fuzzy on how it all should work.

**samw:**\
Probably a default starting point.

**Lukas Orsvärn:**\
Yeah.
I guess it's possible.
Sorry, go ahead.
Yeah, so what Sam, what you said, it's probably a default starting point,
like just default values for them, I would assume.
And I think you don't determine them on a case-by-case basis, I don't think,
because I understand it.
It's like a separate decision.
Like, is the coefficient,
the ecological indicator coefficient 3 or 3.1 or whatever?
You decide that separately,
and then that's just used every time in all of the decisions, kind of.
That's how I have understood it.

**Ben:**\
I guess it's possible.
Like, for example, for this,
you could say there's a company that's trying to push into the knowledge
integration a lot of very toxic paint, and they're giving a lot of knowledge
records of their toxic paint and how it's valuable.
And then when you're making the constraint checking, then you would say,
we have a high environmental coefficient, so we can't use this toxic paint.
And that would kind of help to eliminate that bias and say this knowledge is not
as relevant.

**Lukas Orsvärn:**\
Yeah, in a sense, I guess the paint wouldn't be valued at all by what they think
about the paint in that sense, right?
It would be valued by how long does it last
before you need to do something with it, or like upkeep on it,
like how much upkeep is it?
And like how much resources does it take to use it,
how much resources does it save because you have painted it
and it protects what you painted it with, you know, stuff like that.
So it's not really, there are no like ratings or anything like that, right?
Or a person who can say like, oh, I think this is good,
so therefore you should use it.
But if a node starts putting in like false data, then that's a problem, I guess.
And I think that's probably solved on a different level, probably,
where you just, other nodes would say, oh, hey,
this node is probably inputting false data.
It doesn't make sense.
And so you would kind of just like, you know, okay,
we're not going to interact with that node, whatever data they have,
we're just going to ignore it and go on with our lives.

**Ben:**\
Well, wouldn't that be taken into account here during the context score?
That would be the purpose of the context score,
because they would no longer be contextually relevant based on the coefficients
that matter to the community.
So you say that the coefficients that matter to the community, like environment,
and so on, and labor, the knowledge
that is trying to be pushed here is not contextually relevant.
Like if you have, for example, a paint company, and they're trying to give you,
they're trying to put into the knowledge, in step three here,
they're trying to integrate knowledge that's going to affect the decision.
So they want to put in like, a ton of papers about the benefits of their paint,
right?
So at this point, you're going to look at the context building,
the context coefficients and say, okay, these are not contextually relevant,
even though this person who is a member of the community wants to add all this
information, they can't, I see this as a kind of a way of eliminating that
bodice, maybe.

**Lukas Orsvärn:**\
Yeah, maybe that could be the case.

**samw:**\
Could that be where the fairness indicators come into play?
Or maybe not, but I'm wondering how is the score vector related to the context
model?
Are those different entities?
Is it the same thing?
I mean, is the score vector a part of the model?

**Lukas Orsvärn:**\
That's a good question.
I don't know.

**Ben:**\
I see the score vector as something that's being determined and saying, okay,
this is because you're adding knowledge, right?
You're adding these pieces of knowledge,
and you're giving them each of them a score vector.
And that will be determined, determine the relevance in subsequent module,
right?
Is that not correct?

**Gary Kent:**\
Related to the scenario.

**Alberto:**\
Yeah, there's scenarios that are derived from module three,
that are then passed on to module four.
But that's the thing.
That's where I see that this fits in.
Like this coefficient is not output, but this coefficient happens,
or not coefficient, this mathematical equation happens.
And then with this information, and then with this information,
then the generation starts.
Okay, we can generate this scenario.
And we can take this proposal, change it a little bit,
and then we can add it to that.
And then all sorts of scenarios are produced.
And then at the end, they get to module four.
And this is where I think, yeah, it is already baked into the scenarios.
Like there wouldn't be scenarios proposed to module four
that would violate this equation.
That's how I see it, yes.

**Gary Kent:**\
Constraints are added in module four.

**Alberto:**\
That's what I thought.
Like, I still think that the information for constraints,
and also all sorts of other informations are already there in module three,
with the scenario.

**Gary Kent:**\
I can look up the scenario fields that are defined in some of the code,
pseudocode, if people want me to do that.

**Ben:**\
Like the context score vector is what we're talking about, right?
The context score vector gets assigned to a piece of information that's added at
stage at module three.

**Gary Kent:**\
Yeah, that's what I'm saying is if I look at the,
if it's added in the scenario data, I'll have a record of that in my notes.
I can look it up real quick.

**Ben:**\
So everything gets assigned to a context score in module three,
all this piece of information.
And then in module four, you only use those ones that are contextually relevant.
Like if you have someone, for example, saying by it, they have a very,
I think I'll use the orange paint example.
They have a very strong cultural bias towards orange paint,
but that doesn't pass.
It doesn't get a very high context score.
So when you're looking at it in module four, you're going to say, no, this one,
this piece of information is not relevant
because it has such a low context score.
So is the context score act acting as constraints of some kind
or just thresholds that it,
I think it's just determining
if it's contextually relevant like this in terms of environment resources and
so on is this piece of information that they're trying to use.
Maybe it's, maybe it's like a list or something, right?
And they're trying to determine if it's relevant when making the decision.

**Gary Kent:**\
Okay.
If you're still looking at my screen, here's the scenario data class.

**Alberto:**\
Okay.
Scenario.
Okay.

**Gary Kent:**\
So it has a field called indicators.
And here's the reference.
Project outcomes filled by modeling.

**Lukas Orsvärn:**\
Yeah.
In terms of what you're talking about, Ben, with what it's being applied to,
I'm not sure I see that anywhere.
Like the biggest context score thing,
like defining what it is and stuff
that I can find is this math sketch with a multi-criteria indicator aggregation,
because that's the context score, right?
That's what calculates the context score.
Or am I mistaken about that?

**Ben:**\
But what do you use that context score for, right?
It gives, it's assigned to an, I believe it's assigned to a piece of knowledge.
Am I right?

**Lukas Orsvärn:**\
Yeah.
But is it?
I don't know if it is, because if you look at what it inputs here as an example,
it's ecological indicators, resource indicators, labor indicators,
and social fairness indicators.
And that's what creates the context score vector.

**Gary Kent:**\
That's what this integrated indicator fields is about right there.

**Ben:**\
But what gets the context score, and it has to be, it's in module three.
So I think it's a piece of knowledge.
Like this is maybe, for example,
it's a list of corrosion or someone's submitted a document, right?

**Lukas Orsvärn:**\
Yeah, that's, that's the thing that I'm not sure about.
Because I don't know what it's being assigned to.
This is all I have to go on of ecological indicators, resource indicators,
and labor indicators.
So what you're saying might be true.
But from what I can find, it could be that,
but this isn't very clear about what is this actually,
what are these indicators and stuff like that.

**Ben:**\
I think that's what it is.
Someone has submitted a document or a piece of evidence,
and it's being assigned a context score.

**Lukas Orsvärn:**\
Yeah, but it's, it's hard to talk about that, unless we can find that,
we know that that's what it is.
Because that might be what it is.
What else could it be?
Well, I, like I explained before,
it could be that it's just like a general score of stuff.
Like a general, like, what is the context even?
Like, what is that is contextual to the issue?
Is it contextual to the context of the node?
Like, what is the context that it's referring to even?
And we, like, like, I, it might be very clear somewhere, but I,
it's not clear to me so far, at least, of what is it about?
So it could be that it's just about, you know, taking, you know,
how much resources do we have?
And how much do we value having resources?
And that's the coefficient that you apply to that.
And then you normalize it,
so that you have now a value of 0.8 in the context of like, well,
we have quite a few resources, one is as much resources as we can have.
And that's, and that's it.
That's, that's what my interpretation kind of has been of it.
But it could very well be, like, what you're saying,
that every single thing gets a context score,
because everything is scored in the context of the issue, kind of.

**Ben:**\
I don't understand how it would not be, like, I'm not understanding your, your,
okay, where it's like a general context score for module three,
where it's kind of like, because this is trying to integrate knowledge, right?
So are you saying that, like, all of the knowledge that has been integrated,
like people are submitting documents,
and you have historical records or something,
and everything combined is getting a single context score?

**samw:**\
I think yes.
I think it's based on the issue.
That's my intuition, that it's that the issue gets the context score.
And then, and scenarios are weighed against the context score later
that address a particular issue.
I don't think that's correct.
I think it's because, I only say that
because scenarios are weighed against the data.
And it wouldn't make sense in my mind,
if scenarios were weighed against a context score of like,
one little piece of data, like one piece of evidence.

**Lukas Orsvärn:**\
I think we can continue discussing this,
because I think it's a really good discussion to have,
but it sounds like it's a sort of thing that's better done in text,
where we can just like lay out like, what we think this is my sources,
and then we can, you know, think about it over a longer time period, perhaps.
So I think we should put this specific one to rest.

**Gary Kent:**\
Can I make one suggestion first?

**Lukas Orsvärn:**\
Sure, go ahead.

**Gary Kent:**\
If you want to find out what indicators means throughout the white paper
and the dev guides, just do a search and look at what the indicators,
where they are, and where it is, is referenced,
relevant to whatever it is you're trying to understand.
That's the way I've been doing things.
Like when I looked up governance,
and found out it was mostly used as a descriptor, and not as a variable.
So that's the way I've been researching things.
I'm going to close my page if that's, if we're done with it for now.

**Lukas Orsvärn:**\
Yeah, thanks.
Thanks, Gary.
Yes, thank you.
And thanks for the tip.
All right.
Yeah.
So we're closing in on the end of the meeting.
And just to give some time to talk about stuff
before the end of the meeting that's relevant to, you know,
our operations or whatever, like, in this time, we have talked about, you know,
scheduling, you know, should we have Git workshops and stuff like that?
And what are we doing in the next meeting?
So essentially, I think we should talk about what are the next steps
that we want to do.
Intuitively, for me, I feel like we're not done with module three.
I want to keep discussing it on GitHub and everything like that,
and then continue talking about it in the next meeting.
Do people think that sounds good?
Or does someone have another idea?

**Alberto:**\
Yeah, I would suggest that maybe we take a look into the video
that Peter did about the CDS module, maybe specifically this this section,
to see what how he worded it in the end,
or maybe an example that he made or something like that.

**Lukas Orsvärn:**\
Yeah, yeah, you mean module three, module three from the CDS,
but he did a whole CDS video on that.
Yeah, yeah, that sounds like a good idea.
Yeah.
Okay, so we continue with this on GitHub, check out the video,
and then we continue talking about it in the next meeting.
And see, and we also have to apply some of the things we talked about here,
we have some, some conclusions,
kind of that we've come to in this meeting about some of the questions
that we can do stuff with as well.
Can you link that video, or someone link that video in the chat or somewhere,
just so we have it?
That would be great.

**Gary Kent:**\
Up on Discord somewhere, but it's on YouTube and Revolution Now, I think.

**Alberto:**\
We're looking it up right now.
I'll just put the link into the chat, and then we at least have it there.
Excellent, excellent.

**samw:**\
Should we anticipate finishing module three in the next meeting,
and then starting to talk about module four also?

**Lukas Orsvärn:**\
I think so.
Yeah, I think so.
We may not finish it in module three, but I think we can,
we should definitely start thinking about that we might finish it.
So in that case, this is kind of maybe what you were thinking about.
Is there something that needs to be done for the module four document
for us to be able to do that?

**samw:**\
I think I've looked at it closely, personally.

**Gary Kent:**\
About the bridge.
Maybe we should talk about that after we do module three.

**Alberto:**\
Yeah, I think that's very, very important.

**Lukas Orsvärn:**\
Good, good.
Then we do need someone to do that,
because we don't have any version of the bridge stuff.

**Alberto:**\
But that's the hard part.
I think there is none.
That's like omitted, basically.

**Gary Kent:**\
We could even, we could either incorporate it into module three as three A, B,
and C, or we can create an extra module.

**Lukas Orsvärn:**\
Is there no...

**samw:**\
You know, Peter does talk about that in the, in the, that episode,
that CDS episode he does.
So maybe that should be the source of truth, module three, module four,
because that might be where the most detail is.

**Alberto:**\
Yeah, but we could do it together next time.
We could actually just start some, some points that we,
that we actually want to have in there, maybe.

**Lukas Orsvärn:**\
I would like us to gather all the information that we do have about it.
Because, yeah, I've been confused about this,
because I haven't really come across a bridge step
when I've been looking at stuff.
I mean, if it's out there, I've definitely,
I've watched all the videos and read everything.
So I've seen it, but it's not like in my mind somewhere as a thing that exists.
So I think the first thing,
the most important thing is to gather everything we do know about it.
Like, where did people learn about it?
Is it just this video?
Is it written somewhere?
So I think that's an important thing to do.
And we should do that, I think, as soon as possible, so we can start, you know,
thinking about it and stuff like that.
So if someone has something, just send it in the chat or, or wherever,
just so everyone has access to it about the bridge step.

**Gary Kent:**\
Then the raw mermaid file that Peter created is where the 3A, 3B,
and 3C stuff is.
The bridge steps are mentioned in other places, I think, in the dev guide.
But in the white paper, it doesn't talk about it.
It's just all of a sudden scenarios show up in module four.

**samw:**\
It is briefly mentioned in the white paper.

**Alberto:**\
Okay, nice.

**samw:**\
The bridge step?

**Alberto:**\
Yes, it is.
I also can recall that.
But just briefly, and I think it's also in one line of code,
also as one word or something like that.

**samw:**\
All right, nice.

**Lukas Orsvärn:**\
Yeah, let's try to...

**samw:**\
In that video, Peter makes a big point of saying that he forgot to, like,
fully describe it in the white paper,
then takes that as an opportunity to do so at that point in the video.
We'll have to re-watch that.

**Alberto:**\
That sounds perfect.
Before we meet the next time, yeah.
And also with that, Lucas, I don't know, we talked about it on Thursday.
I would like to propose something before we end.
Maybe if everybody here would be open to it,
how about having a second meeting the week?
Or how are your capacities?

**samw:**\
I'm available, so I'd be up for it.

**Lukas Orsvärn:**\
Yeah, I may be available.
It depends on when it is and stuff like that.

**Gary Kent:**\
Yeah, I'm the same.
I think everybody wants to move a little faster, but this coming week,
I actually have some doctor's appointments that I need to attend on Thursday
and following Monday, I think.

**Alberto:**\
I think we should set up a, how do you say, some sort of meeting?
How do you say?

**Sabrina:**\
Survey.

**Alberto:**\
Some survey to determine the second day of meeting.
How about that?
That sounds good.

**Lukas Orsvärn:**\
Yeah, feel free to do that.
Will you do that?

**Alberto:**\
Yeah, yeah, we could do that.
We already do it with the activist group that we have.

**Lukas Orsvärn:**\
We do it on Discord.

**Sabrina:**\
Do we still have the threads for every meeting, or is it done?
No, we still have threads for every meeting.
Then we do it for the next one.

**Alberto:**\
Okay, then we will try to do it, and then we will put it up on Discord.
Yeah, okay.

**Gary Kent:**\
Or maybe we could have a module, a meeting 12B, a bridge step to meeting 12.

**Ben:**\
Sounds perfect.
I have a question for the people here.
Do you think that we should be offering to help Peter with his GitHub?
I know he's working, he says he's working on his CDS system,
and I just feel like it's a monumental task.
I don't know, like, how much we can actually contribute,
but would it be worth asking him if we're, I just,
I just want to see something out of that.
I don't know where he's at with it.
And it's a lot of software development for one guy.

**Gary Kent:**\
Does it trouble anybody that GitHub is all Microsoft stuff?

**Lukas Orsvärn:**\
Okay, we should, the time is up.
So thank you everyone for joining the meeting.
I'm gonna stop the recording, and then we can keep talking afterwards,
but just to give people permission to leave and stuff like that.

**samw:**\
So yeah, thank you everyone for joining, and I'll see you in the next one.
