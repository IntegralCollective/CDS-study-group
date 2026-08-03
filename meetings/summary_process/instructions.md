# Instructions

Write a short summary of the most important outcomes of a meeting transcript.

- Maintain a checklist when working through this.
- The target audience is people who attended the meeting, and those who missed it.
- It will be posted on Discord
  - Use `##` for major sections, use `###` for minor sctions.
  - Do not have an empty line before or after headings.
  - Do not use semantic line breaks.
- Use a bullet point for each thought.
- Focus on where each each discussion was left, not on who said what.
- Write the notes to a new file.
- After writing the notes,
  launch one sub-agent after the other for each below point, not in parallel.
  The sub-agents should not inherit your context.
  Use their output to improve the notes
  after each sub-agent comes back with its results.
  Do not do any other work while the sub-agents are working:
  1. **Use a medium weight model**:
     Do a sceptical fact check of the notes against the transcript.
     Tell it to flag if some part of the notes might not match the notes.
     Use line numbers to point to where every issue is found.
     Do not write when facts are correct, only point out issues.
  2. **Use a light model**:
     Do a critical review of the langauge in the notes.
     Flag words that could be replaced by simpler ones,
     and sentences that would be easier to read if a certain change was made.
     Reference the transcript to retain the original meaning.
     Use line numbers to point at where each issue is found.
- Have the instructions of the sub-agents in mind
  when writing the first iteration of the notes.
  They are a safety guard,
  the goal is that they shouldn't have anything to bring up.

AFTER you have applied the feedback from the sub-agents,
edit the file to split up the text into messages under 2k characters.
Split at headings if possible, it does not matter which level,
and prioritize having fewer but longer messages.
Use a counter at the top of each message, like this:

> `[1/2]`
> <content>

## Instructions for This Particular Transcript

- No decisions were made in the meeting,
  so no need to mention if a decision was made.
- The agenda and transcript are in this folder.
- Write out the sub-agent responses to separate files so I can review them.
