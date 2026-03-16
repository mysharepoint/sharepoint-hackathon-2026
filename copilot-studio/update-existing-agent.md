# Update Existing Copilot Studio Agent

## Purpose

Use this checklist if you already built the hackathon agent in Copilot Studio
and now want to bring it in line with the current repository state before a
recording or live presentation.

## Current Status Of The Package

The repository is now presentation-ready on the content side.

Compared with earlier test versions, the current package now includes:

- generic input handling instead of a scenario-specific source file
- updated BWEC wording and terminology rules
- three active core formats only: press release, interview briefing, and
  British-humour commentary
- default format-speaker pairing for the demo:
  - press release -> Emma Collins
  - interview briefing -> James Whitmore
  - British-humour commentary -> Sir Alistair Pembroke
- stricter output discipline in the agent instructions

## Fastest And Safest Update Path

Do not patch single files inside Copilot Studio one by one unless you have a
specific reason.

For this package, the safest path is:

1. keep the same agent
2. replace the embedded knowledge set with the current upload pack
3. replace the instructions
4. replace the visible prompt chips
5. test once in a fresh chat
6. publish again

## Step-By-Step

### 1. Open The Existing Agent

In Copilot Studio:

1. open the existing hackathon agent
2. confirm you are editing the correct English-language agent
3. do not create a second duplicate agent unless the first one is broken

### 2. Replace The Embedded Knowledge Files

Open the knowledge section for the agent.

Safest method:

1. remove the current embedded files for this demo package
2. upload the full current contents of `copilot-studio/upload-pack/`

The current upload pack contains these files:

- `communication-guidelines.md`
- `council-profile-bwec.md`
- `format-british-humour-commentary.md`
- `format-interview-briefing.md`
- `format-press-release.md`
- `media-profile-bbc-talkshow.md`
- `media-profile-british-humour.md`
- `press-profile-bwec.md`
- `speaker-profile-alistair-pembroke.md`
- `speaker-profile-emma-collins.md`
- `speaker-profile-james-whitmore.md`
- `wording-and-tone.md`

This avoids drift between old and new agent state.

### 3. Replace The Instructions

Open the instructions field and replace the full content with:

- `copilot-studio/agent-instructions.txt`

This step matters because the current instruction set now:

- supports the fixed demo speaker defaults explicitly
- handles uploaded files and pasted text generically
- normalises vague or German input into BWEC wording
- applies stricter output discipline

### 4. Replace The Description

Open the description field and replace it with:

- `copilot-studio/agent-description.txt`

### 5. Replace The Welcome Message

If your current agent still shows the default Copilot Studio greeting or an
older German opening message, replace it with:

- `copilot-studio/welcome-message.txt`

Recommended text:

```text
Welcome to the BWEC Comms Agent.

I can help turn uploaded files or pasted source text into press releases,
interview briefings, media statements, and public-interest commentary.

To get started, choose a suggested prompt or upload a PDF, DOCX, TXT, or
TXT file, or paste the source text directly into the chat.
```

### 6. Refresh The Suggested Prompts

Update the visible prompt chips using:

- `copilot-studio/suggested-prompts.md`

Recommended visible prompts:

1. agent overview
2. press release
3. BBC interview briefing
4. British-humour commentary

Keep the presidential statement as the reserve prompt.

### 7. Check The Core Settings

Before testing, confirm:

- language is English
- file uploads are enabled
- web browsing is off
- actions and connectors are off
- SharePoint knowledge is off for the MVP version

### 8. Run One Fresh Dry Test

Open a new conversation and do not rely on an old cached chat.

Then:

1. optionally run the overview prompt first
2. upload any relevant source file or paste source text
3. run the press release prompt
4. run the BBC interview briefing prompt
5. run the British-humour commentary prompt
6. optionally run an Emma Collins media statement or quote draft

Use these evaluation questions:

- Does the agent work with generic input rather than a named scenario file?
- Does the wording sound consistently BWEC-like?
- Does the press release default to Emma Collins?
- Does the interview briefing default to James Whitmore?
- Does the British-humour commentary default to Sir Alistair Pembroke?
- Do James and Emma sound clearly distinct from one another?
- Does Pembroke sound witty without tipping into parody?
- Does the output stay clean instead of overloading meta warnings?

### 9. Fix Only What Actually Fails

Do not reopen the whole package unless the dry run shows a real weakness.

Typical adjustment areas:

- prompt wording too broad
- Emma not distinct enough from James
- output too cautious or too cluttered with meta notes
- retrieved terminology not matching the wording guide

### 10. Publish Again

Once the dry run is clean:

1. publish the updated agent in Copilot Studio
2. if needed, refresh the `Teams and Microsoft 365 Copilot` channel
3. test once again in a fresh live session

### 11. Record Only After The Fresh Live Check

For the recording run:

1. use a fresh session
2. use one source input only
3. show one input turning into several outputs
4. avoid changing the knowledge pack again on the same day unless needed

## What You Do Not Need To Change Again

You do not need to rebuild:

- the BWEC context files
- the three core format files
- the speaker profiles for James and Pembroke
- the media profiles

Those are already in a usable presentation state.
