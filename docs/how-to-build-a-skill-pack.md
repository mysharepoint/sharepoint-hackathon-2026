# How To Build A Skill Pack

## Purpose

This guide explains how to build a reusable skill-based communication package
like the one in this repository.

The focus is not the last mile in Copilot Studio. The focus is the preparation
work that makes any later technical implementation useful:

- defining a real use case
- describing the organisation and its point of view
- specifying formats, speakers, and media contexts
- turning that logic into structured Markdown files

If this foundation is weak, the agent will stay generic. If this foundation is
clear, the implementation platform becomes much less important.

## The Core Idea

A good communication agent does not start with prompting.

It starts with a structured description of:

- who the organisation is
- what it wants to say
- how it speaks
- who is speaking
- where the message will appear
- what kind of output is required

In this repository, those layers were separated into:

- organisation context
- wording and communication rules
- speaker profiles
- media profiles
- format skills

That separation is what makes the package reusable.

## Start With The Use Case, Not The Tool

Before writing any files, define the communication problem in plain language.

Useful starter questions:

- What kind of incoming material do people receive?
- What must be produced from that material?
- Who speaks for the organisation?
- Which audiences or media formats matter?
- What makes a good output in this scenario?

For this hackathon project, the use case was:

One incoming current-affairs briefing should be transformed into three outputs:

- a press release
- a BBC interview briefing
- a public commentary with a strong speaker voice

The fictional British Wind Energy Council was only one example. The same
pattern could work for a company press office, a trade association, a policy
team, or a communications department in a public institution.

## Step 1: Define The Minimum Viable Skill Pack

Do not start too broad.

For a first working package, you usually need:

1. one or two organisation files
2. one or two wording and communication rules files
3. two or three speaker profiles
4. one or two media profiles
5. two or three output formats

That is enough to demonstrate whether the idea works.

In this repository, the minimal live set became:

- `common/council-profile-bwec.md`
- `common/press-profile-bwec.md`
- `references/knowledge-pack/communication-guidelines.md`
- `references/knowledge-pack/wording-and-tone.md`
- three speaker profiles
- two media profiles
- three format definitions

## Step 2: Build The Organisation Layer

The organisation layer is the stable identity behind every output.

It should answer:

- Who is the organisation?
- What is its mission?
- What are its priorities?
- Which audiences does it speak to?
- Which recurring messages define its position?

In this project, that logic lives mainly in:

- `common/council-profile-bwec.md`
- `common/press-profile-bwec.md`

### Practical Tips

- Start from existing boilerplates, About pages, mission statements, and press
  materials if they exist.
- If no real organisation exists yet, write a compact fictional profile that
  still feels realistic.
- Keep this layer strategic. Do not overload it with operational details.
- Make the core messages explicit. Do not assume the model will infer them from
  a vague mission statement.

## Step 3: Define The Communication Style

This is often the most valuable file in the whole package.

The communication-style layer explains how the organisation should sound across
all outputs.

It should cover:

- preferred terminology
- tone of voice
- framing principles
- phrases to avoid
- recurring messaging priorities

In this project, that work is split between:

- `references/knowledge-pack/communication-guidelines.md`
- `references/knowledge-pack/wording-and-tone.md`

### How To Find A Communication Style

Look at real material such as:

- press releases
- website copy
- executive quotes
- policy papers
- annual reports
- interview transcripts

Ask:

- Which terms appear repeatedly?
- Which words are never used?
- Does the language sound institutional, technical, journalistic, activist, or
  commercial?
- Does the organisation lead with economics, risk, public value, innovation,
  or mission?

### Practical Rule

Write the wording guide as if it were an internal editorial handbook, not a
vague brand note.

The more precise it is, the more visible the effect will be in outputs.

### How To Use AI For A First Communication Style Draft

If the organisation already has communication guidance, do not start from
scratch.

Use what already exists:

- communication guidelines
- brand language rules
- editorial handbooks
- website tone-of-voice material
- executive messaging notes

AI tools such as ChatGPT or Copilot can help turn that material into a first
structured wording guide.

That first draft should then be tightened and adapted until it reflects the
real communication style of the organisation.

### Example Prompt For A Communication Style File

```text
Draft a communication style file in English for an AI communications agent.

Use the following source material as input:
- company communication guidelines
- website copy
- boilerplate text
- executive messaging notes

The output should define:
- preferred terminology
- tone of voice
- phrases to avoid
- recurring framing principles
- editorial rules that should apply across all outputs

Write it as a practical internal wording guide in Markdown.
Keep it specific, structured, and reusable.
```

## Step 4: Define Speaker Profiles

Speaker profiles are not just biographies.

They explain how a specific person or spokesperson should sound when the agent
writes in their name.

A useful speaker profile should include:

- role
- function in the organisation
- tone
- sentence rhythm
- rhetorical habits
- preferred themes
- things to avoid
- how the style shifts by format

Examples in this repository:

- `references/knowledge-pack/speaker-profile-james-whitmore.md`
- `references/knowledge-pack/speaker-profile-emma-collins.md`
- `references/knowledge-pack/speaker-profile-alistair-pembroke.md`

### How To Find A Speaker Style

Use real source material if available:

- speeches
- interviews
- quote sheets
- LinkedIn posts
- conference appearances
- panel discussions

Then describe:

- What makes this person recognisable?
- Are they formal or conversational?
- Do they sound strategic, punchy, calm, witty, technical, or statesmanlike?
- Do they use short sentences or long ones?
- Do they build arguments with contrast, examples, statistics, or slogans?

### Practical Tip

Do not describe only personality traits.

Describe writing behaviour.

Bad:

`smart, dynamic, experienced`

Better:

`short, clean sentences; often uses three-part lists; starts with a practical
point before expanding the argument`

### How To Use AI For A First Speaker Profile Draft

Speaker profiles become much stronger if you start from real language samples.

Useful inputs include:

- speech transcripts
- interviews
- published statements
- conference remarks
- articles or posts written in the speaker's name

AI tools can help analyse those materials and turn them into a structured first
speaker-profile draft.

The key is not to accept that first version blindly.

Use it as a starting point, then sharpen:

- what feels too generic
- what is truly distinctive
- how the style changes by format
- which verbal habits should be visible in the final outputs

### Example Prompt For A Speaker Profile

```text
Draft a speaker profile in English for an AI communications agent based on the
attached or pasted source material from a spokesperson's previous speeches,
interviews, and statements.

Analyse the material and describe:
- tone of voice
- sentence rhythm
- rhetorical habits
- preferred themes
- how the speaker sounds under pressure
- what the speaker should avoid
- how the style should shift across formats such as press quotes, interviews,
  speeches, and commentary

Write it as a practical internal speaker-profile file in Markdown.
Keep it specific and behaviour-based, not generic.
```

## Step 5: Define Media Profiles

Media profiles explain the target environment for the output.

This matters because a press release, a BBC talkshow briefing, and a social
commentary do not use the same register even when they talk about the same
facts.

Examples in this repository:

- `references/knowledge-pack/media-profile-bbc-talkshow.md`
- `references/knowledge-pack/media-profile-british-humour.md`

A good media profile should cover:

- likely audience
- expected tone
- length and pacing
- what counts as strong material
- what feels out of place
- how sharp, formal, or playful the output may be

### How To Find A Media Style

Study the output environment, not just the outlet name.

For example:

- broadcast interviews reward clarity, brevity, and quotability
- trade press rewards sector detail and relevance
- social commentary rewards hook, distinct voice, and memorability

Think in terms of rhetorical fit, not just publishing channel.

### How To Use AI For A First Media Profile Draft

You do not always need to start from a blank page.

AI tools such as ChatGPT or Copilot can already help generate a strong first
draft for a media profile, because many media formats are publicly
recognisable in their pacing, tone, and rhetorical expectations.

A practical workflow is:

1. name the outlet, format, or channel
2. ask the AI for a first structured media-profile draft
3. review the result critically
4. remove generic parts
5. add the specific traits that matter for your use case

The same principle applies to almost all skill files in a project like this.

In many cases, the best starting point is not a blank page, but a generic
AI-generated draft that gives you a usable structure. From there, the real
work is refinement: adapting the draft to the organisation, the speakers, the
intended outputs, and the actual communication goals.

In other words:

Use AI to generate the first framework.
Use human judgement to make it specific, credible, and reusable.

### Example Prompt For A BBC Media Profile

```text
Draft a media profile in English for a BBC talkshow format to support an AI
communications agent.

The profile should explain:
- likely audience expectations
- tone of voice
- pacing and sentence length
- what counts as a strong broadcast answer
- what feels too long, too technical, or too corporate
- which kinds of questions are likely
- what a spokesperson should do and avoid in this setting

Write it as a practical internal guidance file for a communications skill pack.
Keep it structured, concise, and reusable.
```

## Step 6: Define The Output Formats

Format skills are where the package becomes operational.

Each format should describe what the output is supposed to do.

In this repository, the core formats are:

- `formats/press-release/SKILL.md`
- `formats/interview-briefing/SKILL.md`
- `formats/british-humour-commentary/SKILL.md`

And the flat mirrored format files used in the knowledge pack are:

- `references/knowledge-pack/format-press-release.md`
- `references/knowledge-pack/format-interview-briefing.md`
- `references/knowledge-pack/format-british-humour-commentary.md`

Each format should answer:

- What kind of output is this?
- Who is it for?
- What structure should it follow?
- What should always be included?
- What should never happen?
- Which speaker is the default for this format?

### Practical Tip

Formats should be outcome-oriented.

Do not write:

`Generate text about topic X`

Write:

`Prepare an internal interview briefing with key messages, likely questions,
bridge lines, and do-not-say topics for a broadcast appearance`

### How To Use AI For A First Format Draft

Many communication formats already have a well-known structural logic.

That means you often do not need to invent the first version from zero.

AI tools can help generate a generic first draft for formats such as:

- press release
- interview briefing
- position paper
- product description
- campaign statement
- policy note

The first draft gives you the formal skeleton.

After that, your real task is to adapt it to:

- the organisation
- the speaker defaults
- the expected output quality
- the specific communication purpose

### Example Prompt For A Format Skill

```text
Draft a format definition in English for an AI communications agent.

The format is: press release.

The file should explain:
- what this output is for
- who the audience is
- what structure it should follow
- which sections should always be included
- what should be avoided
- what kind of tone is appropriate
- what makes the result publishable or at least press-ready

Write it as a reusable Markdown file for a communications skill pack.
Keep it practical, structured, and easy to adapt.
```

## Step 7: Create Realistic Source Inputs

A skill pack becomes easier to test when the inputs are realistic.

Use:

- daily briefings
- background memos
- fact sheets
- policy summaries
- media round-ups

In this project, example runtime inputs were stored under:

- `copilot-studio/runtime-inputs/`

### Practical Tip

Keep the input material realistic but compact.

You do not need a full data warehouse. You need a source text that forces the
agent to interpret, prioritise, and adapt.

## Step 8: Use AI As A Structuring Partner

One of the strongest lessons from this project is that AI tools are very good
at helping turn rough requirements into structured files.

That does not remove the human task. It changes it.

The human contribution is:

- defining the use case
- deciding the communication intent
- recognising what sounds right or wrong
- approving the final structure

The AI contribution is:

- expanding rough notes into structured drafts
- turning style descriptions into usable profile language
- tightening wording guides
- generating first versions of speaker and media profiles

### Good Way To Work With AI

1. Describe the use case in plain language.
2. Describe the desired speaker, format, or tone.
3. Ask the AI to turn that into a structured Markdown file.
4. Review it critically.
5. Sharpen what is too generic.
6. Repeat until the file sounds specific enough to be reusable.

### What To Watch Out For

- generic corporate wording
- vague personality language
- styles that sound interchangeable
- too much abstract branding language
- lack of clear do-and-don't rules

If the file feels like it could belong to any organisation, it is still too
weak.

## Step 9: Test For Difference, Not Just Quality

A skill pack is not successful only because the outputs are fluent.

It is successful when the differences between outputs become visible and
defensible.

Test questions:

- Does each format produce a clearly different output?
- Do the speakers sound distinct from one another?
- Does the wording guide visibly affect the language?
- Does the same source material get reframed appropriately?
- Is the organisation perspective clear?

The best test is not:

`Is this well written?`

The better test is:

`Does this sound like the right person, in the right format, for the right
context?`

## Step 10: Package For Reuse

Once the files work, organise them so others can understand and rebuild the
logic.

This repository separates:

- `common/` for organisation identity
- `formats/` for structural output logic
- `references/knowledge-pack/` for the detailed skill content
- `demo/` for prompts, examples, and presentation-ready demo material
- `copilot-studio/upload-pack/` for the flat operational file set
- `docs/` for public-facing explanation

That separation makes the package easier to reuse, simplify, or port into
another environment later.

## A Good Working Sequence

If you want to repeat this process yourself, this order works well:

1. define the use case
2. choose the outputs
3. define the organisation
4. write the wording guide
5. define the speakers
6. define the media environments
7. write the format skills
8. test with real source material
9. refine until the differences are clear
10. package and document the result

## What Will Matter Later In SharePoint Too

Even if the technical implementation later happens somewhere else, the core
preparation work will stay the same.

You will still need:

- clear use cases
- structured skill descriptions
- explicit wording rules
- defined roles and speaking styles
- format logic that can be reused

That is why this preparation is not just a workaround for Copilot Studio.

It is the main design work behind any future skill-based communication setup.

## Final Advice

Keep the first version small.

Do not try to model the whole communications department at once.

A small package with:

- one organisation
- three speakers
- two media contexts
- three formats

is already enough to prove whether the concept works.

Once that works, you can always scale.
