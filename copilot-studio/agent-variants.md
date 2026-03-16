# Agent Variants

## Purpose

Use this note to keep the two recommended Copilot Studio variants clearly
separated.

Do not mix both modes into one agent if you need predictable demo behaviour.

## Variant 1 - Demo Safe

Use this variant for:

- recording
- live presentation
- jury demo
- repeatable dry runs

Configuration:

- language: English
- embedded knowledge: `copilot-studio/upload-pack/`
- web search: off
- SharePoint or OneDrive sync: off
- actions or flows: off
- file uploads: on

Why this variant exists:

- maximum control over tone and structure
- reproducible outputs
- strongest BWEC and wind-energy alignment
- lowest risk of retrieval drift

Best uses:

- press release
- BBC interview briefing
- British-humour commentary
- overview prompt during demos

## Variant 2 - Live News

Use this variant for:

- current-affairs monitoring
- same-day reactions
- live topic exploration
- latest-news response drafting

Configuration:

- language: English
- embedded knowledge: `copilot-studio/upload-pack/`
- web search: on
- SharePoint or OneDrive sync: off at first
- actions or flows: off at first
- file uploads: on

Why this variant exists:

- combines BWEC framing with current public information
- useful when the user asks for the latest developments
- supports reactive drafting on fast-moving stories

Risks:

- less predictable outputs
- more drift toward generic web summary language
- weaker reproducibility in recordings or judged demos

Recommendation:

- keep this as a separate agent or a duplicate of the demo agent
- do not use it as the primary recording setup

## Decision Rule

Choose `Demo Safe` when consistency matters more than freshness.

Choose `Live News` when freshness matters more than strict repeatability.
