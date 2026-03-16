# Demo Prompts

## Purpose

Use these prompts with either:

- an uploaded source document
- pasted source text

They are designed for the BWEC hackathon demo and map directly to the current
knowledge pack.

## Current Shared Demo Focus

For the current North Sea Summit scenario, all three core prompts should work
from the same strategic question:

What does the North Sea Summit mean for the British windmill industry and for
the wider UK economy?

The wording is intentionally left slightly imprecise in the operator prompt so
the BWEC wording rules can demonstrate how the agent normalises user language
into the preferred sector terminology in the output.

This common focus should shape:

- the press release by Emma Collins
- the BBC interview briefing for James Whitmore
- the British-humour commentary by Sir Alistair Pembroke

## Prompt 1 - Press Release

```text
Use the uploaded file or pasted source text to draft a BWEC press release in
English. Use format-press-release.md, communication-guidelines.md,
wording-and-tone.md, council-profile-bwec.md, and press-profile-bwec.md.

Turn the input into a clear, media-ready release about what the North Sea
Summit means for the British windmill industry and the wider UK economy.
Emphasise offshore wind expansion, energy security, industrial growth, supply
chains, investment confidence, and strategic infrastructure. Include one quote
and mark it APPROVAL PENDING. Keep all claims tied to the source material and
date-sensitive where needed.
```

Default speaker for this format: Emma Collins.

## Prompt 2 - BBC Interview Briefing

```text
Use the uploaded file or pasted source text to prepare a BWEC interview
briefing for a BBC talkshow appearance. Use format-interview-briefing.md,
media-profile-bbc-talkshow.md, communication-guidelines.md, and
wording-and-tone.md.

Focus on what the North Sea Summit means for the British windmill industry and
the wider UK economy. Prepare likely public-interest questions, short
broadcast-ready answers, bridge lines, and do-not-say topics. Keep the tone
calm, strategic, and public-facing.
```

Default speaker for this format: James Whitmore.

## Prompt 3 - British Humour Commentary

```text
Use the uploaded file or pasted source text to write a short British-humour
commentary for a two-minute video, podcast segment, or social-media clip. Use
format-british-humour-commentary.md, media-profile-british-humour.md,
communication-guidelines.md, and wording-and-tone.md.

Make it witty, memorable, and serious in substance. Focus on what the North
Sea Summit means for the British windmill industry and the wider UK economy.
Do not turn the underlying issue into a joke. Make the tone dry, lightly
sardonic, unmistakably British, and more absurdist than a standard opinion
column. Land on a clear practical argument about offshore wind, industrial
strategy, or economic resilience, not just style.
```

Default speaker for this format: Sir Alistair Pembroke.
Default intensity for this format: Strong.

You can also trigger:

- `British Humour Light` for a more restrained, polished version
- `British Humour Strong` for the current full absurdist version

## Prompt 4 - Presidential Statement

```text
Use the uploaded file or pasted source text to draft a short external
statement from James Whitmore. Use
speaker-profile-james-whitmore.md, communication-guidelines.md,
wording-and-tone.md, council-profile-bwec.md, and press-profile-bwec.md.

Length: 120 to 160 words. The statement should sound statesmanlike, measured,
and quotable. Emphasise resilience, industrial confidence, and the need for
practical action without sounding opportunistic.
```

## Recommended Live Order

1. Press release
2. BBC interview briefing
3. British-humour commentary
4. Presidential statement if there is time or as backup output
