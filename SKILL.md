---
name: sharepoint-2026-hackathon
description: Build a minimal English communications copilot demo for a SharePoint or Copilot Studio hackathon by curating a small knowledge pack, drafting agent instructions, and preparing a five-minute demo for corporate communications or press-office scenarios. Use when Codex needs to package existing communication modules into a slim Microsoft Copilot setup with three core output formats, sample speaker and media profiles, and clear setup guidance.
---

# Build The Hackathon Package

## Purpose

Create a lightweight English demo package that shows how an existing
communications workflow can be turned into a Microsoft Copilot setup for a
short live presentation.

## Use These Files

- Use `common/` for organisation-wide context such as council identity,
  mission, press boilerplate, and media contact details.
- Use `formats/` for the internal format skills that define the three active
  demo output types.
- Use `copilot-studio/` for the paste-ready build assets: minimal upload pack,
  instructions, suggested prompts, runtime input, and dry-run checklist.
- Use `demo/` for prepared showcase inputs, rehearsal source material, and
  scenario-specific demo assets.
- Use `references/knowledge-pack/` as the runtime knowledge set for the demo
  agent.
- Use `references/copilot-agent-instructions.md` as the starting point for the
  Copilot instructions field.
- Use `references/hackathon-plan.md` to keep the scope small and explain the
  architecture.
- Use `references/demo-script.md` to rehearse the five-minute walkthrough.
- Use `references/source-map.md` to trace which local source materials were
  adapted into this package.

## Default Scope

- Build one English agent, not multiple specialist agents.
- Keep the knowledge pack small enough to explain in one slide.
- Include one general council profile and one press profile as the common
  background layer.
- Focus on three core format files:
  - press release
  - interview briefing
  - British-humour commentary
- Support three simple input patterns:
  - uploaded background note or fact sheet
  - journalist request or interview setup
  - uploaded or pasted source text for public commentary

## Working Rules

- Prefer portable markdown files over tenant-specific setup steps.
- Keep every knowledge file self-contained; do not rely on folder-relative
  references inside the files.
- Ask for missing required details in one structured batch.
- Treat current user instructions and uploaded case material as more specific
  than the embedded knowledge pack.

## Intentionally Omitted

- SharePoint actions, Power Automate flows, and approval automation
- broad site-wide knowledge ingestion
- non-English variants
- additional communications modules that do not improve the five-minute demo
