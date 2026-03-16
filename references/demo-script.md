# Five-Minute Live Demo Script

## Goal

Show one current-affairs input turning into three different communication
outputs for the British Wind Energy Council.

Current source scenario:

- `copilot-studio/runtime-inputs/source-material-north-sea-summit-2026-01-26.md`

Current operator prompt source:

- `demo/demo-prompts.md`

## What To Prepare Before Recording

- Open the agent in Copilot Studio or Microsoft 365 Chat.
- Start a fresh chat.
- Keep the North Sea Summit Markdown file ready to drag into the chat.
- Keep the three prompts ready to paste.
- Do not change settings or knowledge files right before the recording.

## Live Flow

### 0:00 to 0:30 - Opening

Say that the demo shows a simple but realistic communications use case:
one daily briefing comes in, and the agent turns it into three different
outputs for three different communicators.

Core line:

One input, three roles, three outputs.

### 0:30 to 1:00 - What The Agent Knows

Show the compact package structure only briefly and explain:

- organisation context
- wording and communication rules
- three output formats
- three speaker profiles
- two media profiles

State that the setup is intentionally lightweight:
no custom code, no flows, no complex integration.

### 1:00 to 1:20 - Source Input

Drag the North Sea Summit Markdown file into the chat.

Explain that this is a daily briefing about the Hamburg North Sea Summit in
January 2026, focused on offshore wind, energy security, grid development, and
industrial strategy.

### 1:20 to 2:10 - Output 1: Press Release

Run:

```text
Draft a BWEC press release in English based on the uploaded file or pasted
source text, focused on what the North Sea Summit means for the British
windmill industry and the wider UK economy.
```

What to point out:

- the agent turns a briefing into a public press release
- Emma Collins is used as the default voice
- the sloppy phrase `windmill industry` is normalised into proper BWEC wording
- the output focuses on offshore wind, jobs, investment, and energy security

Only show:

- headline
- first paragraph
- quote
- boilerplate

### 2:10 to 3:10 - Output 2: BBC Interview Briefing

Run:

```text
Prepare a BWEC BBC interview briefing based on the uploaded file or pasted
source text, focused on what the North Sea Summit means for the British
windmill industry and the wider UK economy.
```

What to point out:

- same source, different format
- now the agent prepares James Whitmore for broadcast
- the output is internal, not public
- it contains key messages, likely questions, bridge lines, and watch-outs

Only show:

- opening framing
- three key messages
- one or two likely questions
- one bridge line

### 3:10 to 4:10 - Output 3: British Humour Commentary

Run:

```text
Write a BWEC British-humour commentary based on the uploaded file or pasted
source text, focused on what the North Sea Summit means for the British
windmill industry and the wider UK economy.
```

What to point out:

- same facts, third rhetorical mode
- now the speaker is Sir Alistair Pembroke
- this is designed for social video, short commentary, or podcast use
- the output is more pointed, character-driven, and memorable

Only show:

- hook
- one strong middle paragraph
- closing line

### 4:10 to 4:40 - Why This Matters

Make the key point explicit:

The value is not that AI writes text.
The value is that the same source can be transformed into different
communication formats when roles, rules, and wording are clearly defined.

### 4:40 to 5:00 - Close

Close with three short points:

- this is a lightweight proof of concept
- the same pattern could work for many communications teams
- the next step is to bring this closer to SharePoint skills and libraries

## Recording Tips

- Do not scroll through full outputs.
- Stop at the strongest parts of each answer.
- Say explicitly when the format changes from public to internal to commentary.
- Call out the wording normalisation once, because it demonstrates the value of
  the wording rules.
- If time is tight, skip the architecture explanation first, not the third
  output.
