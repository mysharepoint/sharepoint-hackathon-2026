# SharePoint 2026 Hackathon Plan

## Goal

Show a minimal English communications copilot that helps a press or corporate
communications team turn simple source material into usable outputs in minutes.

The demo should prove three things:

1. One small knowledge pack is enough for a useful communication workflow.
2. The agent can switch between different output formats without complex
   orchestration.
3. Speaker and media profiles improve the output without needing custom code.

## Recommended MVP

- Platform: start in Copilot Studio with embedded files
- Agent count: one agent
- Language: English
- Knowledge sources: the flat mirrored upload set in
  `copilot-studio/upload-pack/`, derived from `common/` and
  `references/knowledge-pack/`
- User interaction: chat plus optional file upload
- Disabled for MVP: web browsing, actions, flows, approvals, large SharePoint
  libraries

This is the smallest setup that is still easy to explain in a five-minute demo.

## Core Demo Pattern

| Input pattern | What the user gives | Main output |
| :-- | :-- | :-- |
| Source file or pasted source text | Background note, fact sheet, daily media summary, briefing note | Press release |
| Same source material reframed for broadcast | Public-interest issue that needs spokesperson preparation | Interview briefing |
| Same source material reframed for public commentary | Topic for video, podcast, or social-media commentary | British-humour commentary |

These three patterns cover external press output, spokesperson preparation, and
public-interest commentary. The `common/` files provide the reusable
organisation context and boilerplate needed across all three outputs.

## Why These Three Formats

### 1. Press release

Use this as the most recognizable external output. It is familiar to judges and
easy to evaluate quickly.

### 2. Interview briefing

Use this to show the value of speaker and media profiles. It makes the demo
feel more realistic than a generic writing assistant.

### 3. British-humour commentary

Use this to show that the same source input can also be turned into a clearly
different public-facing output with a strong rhetorical character.

## Build Sequence

1. Curate the knowledge pack.
2. Include the two `common/` files as the organisation layer.
3. Keep the internal format skills under `formats/` as the structural source of
   truth.
4. Mirror the flat upload set into Copilot Studio.
5. Paste the baseline instructions into the agent.
6. Add one overview prompt plus three suggested prompts matching the three demo
   outputs.
7. Test one prompt per output format.
8. Rehearse the five-minute narrative so the transition between prompts feels
   deliberate.

## Suggested Prompts

1. "Draft a BWEC press release in English based on the uploaded file or pasted
   source text."
2. "Prepare a BWEC BBC interview briefing based on the uploaded file or pasted
   source text."
3. "Write a BWEC British-humour commentary based on the uploaded file or pasted
   source text."

## Five-Minute Storyline

- Minute 1: explain the problem and show the small knowledge pack
- Minute 2: upload a source file or paste source text and run the press release
  prompt, noting that Emma Collins is the default spokesperson for this format
- Minute 3: run the BBC interview briefing prompt, noting that James Whitmore
  is the default speaker for this format
- Minute 4: run the British-humour prompt, noting that Sir Alistair Pembroke is
  the default speaker for this format
- Minute 5: explain why the architecture is simple, portable, and easy to
  scale later

## What To Explain To Judges

- The solution is intentionally slim so it can be adopted fast.
- General organisation context and press boilerplate are kept in separate
  common files, which makes the pack portable.
- Communication quality comes from explicit rules plus task modules.
- Profiles add context without retraining or code changes.
- The same pattern can later expand into SharePoint libraries, approval flows,
  or more modules.

## What Is Still Needed From The User

- Organization or demo brand name
- Sector or scenario for the demo story
- Preferred spokesperson name and role
- Preferred media target or journalist type
- One concrete trigger event for the demo
- Preferred platform path:
  - Copilot Studio only
  - Microsoft 365 Copilot agent later

## Intentionally Excluded From This Package

- full governance and publishing setup
- tenant-specific SharePoint paths
- Power Automate flows
- legal review logic
- large multilingual knowledge packs
