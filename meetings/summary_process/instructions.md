# Instructions

Write a short summary of the most important outcomes of a meeting transcript.

- Maintain a checklist when working through this.
- The target audience is people who attended the meeting,
  and those who missed it.
- Focus on where each each discussion was left,
  not on who said what or what lead up to the outcomes.
  Keep it short and clear.
- Write the notes to a new file.
- After writing the notes,
  launch one sub-agent after the other for each below point, not in parallel.
  The sub-agents should not inherit your context.
  Use their output to improve the notes
  after each sub-agent comes back with its results.
  Do not do any other work while the sub-agents are working.
  The instructions for each sub-agent can be found later in the instructions.
  Do not add anything more to the sub-agent's prompt.
  Do not give your own context to the sub-agents:
  1. Fact checker.
  2. Language review.
- Have the instructions of the sub-agents in mind
  when writing the first iteration of the notes.
  They are a safety guard,
  the goal is that they shouldn't have anything to bring up.

AFTER you have applied the feedback from the sub-agents,
if the file is above 2k characters,
edit the file to split up the text into messages under 2k characters.
Split at headings if possible, it does not matter which level,
and prioritize having fewer but longer messages.
Use a counter at the top of each message, like this:

```md
`[1/2]`
<content>
```

## Checklist

- Read the transcript
- Write notes.md
- Run fact checker
- Run language review
- Split into messages

## Fact checker

### Output file

fact-check.md

### File access

- Transcript
- Agenda (if available)
- WIP notes

### Model weight

Medium, medium reasoning

### Prompt

```text
You are a meeting note auditor.
Your job is to fact check these notes based on the transcript.

- Flag if some part of the notes *might* not match what the notes say.
- It's better to flag too much than too little.
- Use line numbers to point to each issue.
- Only point out issues, do not write when facts are correct.
- Write which LLM and reasoning level you're using at the top of the file.
```

## Language review

### Output file

language-review.md

### File access**

- Transcript
- Agenda (if available)
- WIP notes

### Model weight

Light, medium reasoning

### Prompt

```text
You are an editor.
Your job is to do a critical review of the language in the notes.

- Flag words that could be replaced with easier ones, and suggest words.
- Flag sentences that could be made easier to read, and how.
- Check the transcript before flagging something to ensure your changes retain meaning.
- It's better to flag too much than too little.
- Use line numbers to point to each issue.
- Only point out issues, do not write about good words or well structured sentences.
- Write which LLM and reasoning level you're using at the top of the file.
```

## Formatting

- Format it for Discord.
- Use `#` for the title,
  `##` for major sections,
  and `###` for sub-sections if needed.
- Do not have an empty line before or after headings.
