# Press Release Drafting

## Purpose

Draft a media-ready press release using an inverted-pyramid structure.

## Default Pairing

- default speaker: Emma Collins
- default organisation context: BWEC boilerplate and BWEC press contact

## Required Intake

- trigger or announcement
- core message
- source-backed facts
- quote owner
- embargo status
- press contact

## Output Format

```text
[EMBARGO: date and time | FOR IMMEDIATE RELEASE]

PRESS RELEASE

[City, Date]

[Headline]
[Subheadline]

[Lead paragraph: what happened and why it matters]

[Paragraph 2: facts, context, background]

"[Quote]," said [Name, Title].
[STATUS: APPROVAL PENDING / APPROVED]

[Paragraph 3: optional context or implications]

About [Organization]:
[Short boilerplate]

Press contact:
[Name]
[Email]
[Phone]
```

## Rules

- Lead with the most important fact.
- Use short paragraphs and concrete language.
- Keep the draft under 400 words excluding boilerplate.
- Default to Emma Collins as spokesperson unless the user explicitly requests another speaker.
- Make the relevance to wind energy and BWEC's sector mandate explicit where
  the source material supports it.
- If the source material is broader than wind energy, frame the release around
  the concrete consequences for wind energy deployment, supply chains, energy
  security, project delivery, or investment confidence.
- Use `press-profile-bwec.md` for boilerplate and press-contact details when
  the organisation is BWEC and no override is provided.
- Mark the entire document as draft material unless approval is stated.
- Do not insert unsupported adjectives or rankings.
