# Copilot Studio Build Runbook

## Goal

Build the smallest viable Copilot Studio demo from this folder with no custom
actions, no flows, and no external knowledge sources.

## Build Decision

Use one agent with embedded files only.

This is the right level of complexity for the current demo package.

## Upload Set

For the fastest first build, use the curated minimal folder:

- `copilot-studio/upload-pack/`

This folder is already reduced to the files needed for the current MVP.

If you later want the broader package, go back to `references/knowledge-pack/`
and `common/`.

## Upload Set Contents

### Common Files

- `council-profile-bwec.md`
- `press-profile-bwec.md`

### Core Rules

- `communication-guidelines.md`
- `wording-and-tone.md`

### Format Files

- `format-press-release.md`
- `format-interview-briefing.md`
- `format-british-humour-commentary.md`

### Speaker Profiles

- `speaker-profile-james-whitmore.md`
- `speaker-profile-emma-collins.md`
- `speaker-profile-alistair-pembroke.md`

### Media Profiles

- `media-profile-bbc-talkshow.md`
- `media-profile-british-humour.md`

## Internal Skill Structure

Inside the repository, the three active demo formats also exist as standard
skill folders under `formats/`.

For Copilot Studio, keep using the flat mirrored files from
`copilot-studio/upload-pack/`.

The internal source files remain in `common/`, `formats/`, and
`references/knowledge-pack/`.

## Optional Later Additions

Add these only if the first build shows a concrete need:

- `references/knowledge-pack/media-profile-trade-press.md`

## Instructions Field

For the first live build, paste:

- `copilot-studio/agent-instructions.txt`
- `copilot-studio/agent-description.txt` into the description field

The broader reference version remains available in:

- `references/copilot-agent-instructions.md`

## Suggested Prompts

For the actual Copilot Studio prompt chips, use:

- `copilot-studio/suggested-prompts.md`

The longer operator prompts remain available in:

- `demo/demo-prompts.md`

For the live demo, start with four visible prompts:

1. Agent overview
2. Press release
3. BBC interview briefing
4. British-humour commentary

Keep the presidential statement as a reserve or fast fifth example.

## Runtime Demo Input

During the demo, either:

- upload a relevant source file such as PDF, TXT, or CSV
- paste source text directly into the chat

For operator guidance, see:

- `copilot-studio/runtime-inputs/input-guidance.md`

## Settings

- Language: English
- Web browsing: off
- File uploads: on
- Actions/connectors: off
- SharePoint knowledge: off for MVP

## Expected Demo Flow

1. Show the compact knowledge pack.
2. Optionally run the agent-overview prompt as a quick orientation step.
3. Upload a source file or paste source text.
4. Run the press release prompt.
5. Run the BBC interview briefing prompt.
6. Run the British-humour commentary prompt.
7. Mention the presidential statement prompt as a fifth reusable path.

## First Dry Run

After the first build, evaluate the three outputs with:

- `copilot-studio/dry-run-checklist.md`

## Why This Is Enough

- The package already covers rules, organisation context, speaker identity,
  media adaptation, and output structure.
- One uploaded or pasted source input is enough to generate multiple output
  types.
- No technical integration is required to demonstrate value.

## What To Avoid In The First Build

- tenant-specific SharePoint setup
- Power Automate
- approvals or publishing logic
- large file sets
- additional modules that are not used in the demo
