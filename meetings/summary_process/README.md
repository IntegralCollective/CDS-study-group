# Summary Process

This is the process we use to automatically generate summaries
of study group meetings.

It has been tested with OpenAI's frontier GPT models.
It is unknown how well it works with other models.

This process uses Codex by OpenAI,
which is a program that runs on the command line.
It relies on being able to create and read files
and run sub-agents.

1. Place these files in the working directory:
   - Meeting agenda.
   - Meeting transcript.
   - <instructions.md>.
2. Give the agent this prompt: `execute instructions.md`.

Here is an overview of what <instructions.md> tells the agent to do:

1. Write a summary.
2. Run a sub-agent to fact-check the summary against the transcript.
3. Run a sub-agent to simplify the language in the summary.
4. Split the summary into several messages under 2k characters if needed,
   so it's ready to be posted to Discord.

Sub-agents are used to ensure the outputs are based on a clean context.
This is meant to avoid issues where the agent accepts things as they are
because that's what it has in its context.
This might be unnecessary,
so it might be good to experiment with not using sub-agents.

Read through the summary and edit it if needed before posting it.
