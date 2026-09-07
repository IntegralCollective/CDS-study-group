# Meeting Transcription Instructions

1. Download noScribe here: https://noscribe.de/en/ (if not already downloaded)
2. Open noScribe and select the audio file you wish to transcribe.
3. Adjust the settings to the following:
  - Language: English
  - Model: Precise
  - Mark Pause: None
  - Speaker Detection: Auto
  - Overlapping Speech: No
  - Disfluencies: No
  - Timestamps: No
4. Hit "Start"
5. Listen to the portion of the audio file in which speaker 0 speaks.
   When you recognize who it is, find and replace all with the speaker's name in noScribeEdit.
   For example: find "speaker 0" and replace all with "John".
   Do this for each speaker.
6. Copy and paste the entire transcript into Chat GPT 5.6 Sol (effort: high). 
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

7. Download the file.
8. Copy and paste the following text to the top of the file:

   ```markdown
   # Weekly Meeting 12 Transcript

   2026-08-16

   Note: This transcript was created by an LLM (large language model).
   It has transcribed wrong in some places,
   and sometimes says the wrong person said things.
   ```
9. Change the date and meeting number
10. Upload file to: 
https://github.com/IntegralCollective/CDS-study-group/tree/main/meetings/transcripts
