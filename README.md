# SharePoint 2026 Hackathon

Minimal demo package for a communications-focused Copilot Studio agent built
for the SharePoint 2026 Hackathon.

## What This Repository Contains

- a compact English knowledge pack for communications outputs
- speaker profiles, media profiles, and format rules
- BWEC demo context for the British Wind Energy Council scenario
- a curated Copilot Studio upload pack
- demo prompts, runtime input, build checklist, and publishing notes

## Who This Is For

This repository is meant for people who want to understand how skill-based AI
agents can be prepared in a structured way before they are implemented in a
tool such as Copilot Studio or, later, SharePoint.

It is especially useful for:

- Microsoft 365 Copilot practitioners
- SharePoint and Microsoft 365 builders
- communications and knowledge-work teams
- anyone who wants to learn how structured skill files can shape AI behaviour

## Prerequisites

The practical entry barrier is relatively low.

The most important requirement is not deep platform engineering. It is a basic
understanding of how to describe a use case, a communication goal, and a set
of reusable skill files clearly enough for an AI system to use them.

This repository focuses mainly on that preparation work.

The skills themselves are written as structured Markdown files. The same logic
can then be used in Copilot Studio today and may later become useful in
SharePoint-based skill experiences as well.

An important part of this repository is also the working method behind those
files:

- use Copilot, Codex, ChatGPT, or similar AI tools to draft the first skill
  structure
- describe the requirement in natural language
- ask for a structured Markdown version
- review, criticise, and refine it until it fits the real use case

In practice, much of this can even be done by voice instead of typing.

In this project, a large part of the work was created through spoken
interaction: describing requirements, asking for formats, refining outputs,
and correcting weak drafts until the files became usable.

So the real prerequisite is mainly:

- curiosity about Microsoft 365 Copilot and future SharePoint skills
- a basic understanding of communication tasks or knowledge work
- willingness to work with structured Markdown files

Everything else can be learned from the example in this repository.

## Practical Perspective

This repository is not meant as a theoretical or academic treatment of agent
design.

It is a hands-on, practice-driven example based on real experimentation:

- define the requirement
- speak it into the AI tool if that is faster
- let the AI draft the first structure
- refine the result until it becomes specific and reusable

That is the main idea behind this package: practical skill design through
iterative collaboration with AI.

## Core Demo Outputs

- press release
- interview briefing
- British-humour commentary

## Repository Map

| Folder | Purpose |
| :-- | :-- |
| `common/` | Core organisation context for the fictional British Wind Energy Council |
| `docs/` | Public-facing guidance on how to design and build a skill pack |
| `formats/` | Internal skill definitions for the three demo output formats |
| `references/` | Background documentation, knowledge-pack source files, and planning notes |
| `demo/` | Demo prompts, runbook material, and reusable public demo assets |
| `copilot-studio/` | Copy-paste-ready instructions, upload pack, runtime input examples, and deployment notes |

Each top-level folder also contains its own `README.md` with a short guide.

## Start Here

If you want to understand the method behind this repository, begin with:

- `docs/how-to-build-a-skill-pack.md`

## Intended Use

This repository is designed as a small, portable project that can be uploaded
to Copilot Studio and demonstrated quickly in a live hackathon setting.

## What This Repository Does Not Try To Be

- not a production-ready publishing system
- not a complex workflow or approval platform
- not a large enterprise knowledge base

It is a compact proof of concept for showing how structured skill files can
shape communication outputs in a reusable way.
