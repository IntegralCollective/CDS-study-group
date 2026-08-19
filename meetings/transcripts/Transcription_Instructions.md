# Meeting Transcription Instructions

1. Upload audio file of meeting to noScribe 
(download noScribe here: 
https://noscribe.de/en/)
2. Listen to meeting audio and manually replace each “speaker x” with the appropriate speaker’s name. 
Do this only for the first time each speaker speaks.
3. Use find - replace all for each speaker name to fill in the remaining “speaker x” labels
4. Copy and paste the entire transcript into Chat GPT 5.6 Sol (effort: high). 
   Give Chat GPT the following instruction:
   
   ````markdown
   Convert this attached file into a markdown file. 
   Format said attached file in the following way:  

   ```markdown
   **John:**\
   This is the first speaker’s text.

   **Joe:**\
   This is the second speaker’s text. 
   ```

   Notice the name is bold, 
   the speech is on the next line after the name, 
   and there is a space between one speaker’s speech and the name of the next speaker. 
   Also, semantic line breaks should be used for the speech. 
   Moreover, don't change any of the actual transcription.
   ````

5. Download the file.
6. Copy and paste the following text to the top of the file:
```markdown
# Weekly Meeting 12 Transcript

2026-08-16

Note: This transcript was created by an LLM (large language model).
It has transcribed wrong in some places,
and sometimes says the wrong person said things.
```
7. Change the date and meeting number
8. Upload file to: 
https://github.com/IntegralCollective/CDS-study-group/tree/main/meetings/transcripts
