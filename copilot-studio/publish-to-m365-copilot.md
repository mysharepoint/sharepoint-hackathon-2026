# Publish To Microsoft 365 Copilot Chat

## Purpose

Describe the simplest current path to publish the hackathon agent from Copilot
Studio so it can be used in Microsoft 365 Copilot or Copilot Chat, with the
option to broaden distribution later.

## What This Means In Practice

For this project, "publish as a Microsoft Copilot Chat agent" means:

1. publish the agent in Copilot Studio
2. add the `Teams and Microsoft 365 Copilot` channel
3. make sure `Make agent available in Microsoft 365 Copilot` is turned on
4. install the agent for yourself first
5. open Microsoft 365 Copilot or Copilot Chat and call the agent there

Publishing alone is not enough. Microsoft documents that the agent is not
automatically deployed to Microsoft 365 Copilot and Teams just because you
pressed `Publish`.

## Important Distinction

Publishing in Copilot Studio is not the same as broad deployment to users.

Current Microsoft guidance distinguishes between:

- publishing the agent from Copilot Studio
- connecting the Teams and Microsoft 365 Copilot channel
- choosing how the agent is made available to users

## Prerequisites

Before you try the live publish path, check these points:

- you already completed `copilot-studio/build-checklist.md`
- the agent works in the Copilot Studio test chat
- target users can use Microsoft 365 Copilot
- your tenant allows Power Platform apps in Teams
- you can access a Copilot Studio environment

If one of these conditions is missing, the channel or availability options can
be limited.

## Recommended First Path

Use the smallest path first:

1. publish the agent in Copilot Studio
2. connect the `Teams and Microsoft 365 Copilot` channel
3. make sure `Make agent available in Microsoft 365 Copilot` is selected
4. install it for yourself first
5. if successful, either share it to a small test group or submit it for admin
   approval

This is the safest route for a first real-world test.

## Step-By-Step

### 1. Finish the Copilot Studio build

Before publishing, complete the build from:

- `copilot-studio/build-checklist.md`

You should already have:

- the embedded knowledge uploaded
- the description in place
- the instructions in place
- the suggested prompts configured

### 2. Publish the agent

In Copilot Studio:

1. open the agent overview page
2. select `Publish`
3. complete the catalog form fields
4. confirm the publish action

Note:

- Microsoft states that publishing prepares the agent, but does not by itself
  automatically deploy it broadly in Microsoft 365 Copilot and Teams

### 3. Connect the Teams and Microsoft 365 Copilot channel

In Copilot Studio:

1. open `Channels`
2. select `Teams and Microsoft 365 Copilot`
3. confirm `Make agent available in Microsoft 365 Copilot`
4. select `Add channel`

If this option is not selected, the agent is available only in Teams.

### 4. Install it for yourself first

Still in the same channel configuration:

1. select `See agent in Teams`
2. add the agent
3. open Microsoft 365 Copilot or Copilot Chat
4. invoke the agent with `@` mention or from the sidebar, depending on tenant
   behavior

This is the fastest way to verify the live path without broader rollout.

### 5. Start a fresh live conversation

Before judging the live result:

1. start a new conversation in Microsoft 365 Copilot or Copilot Chat
2. call the agent with `@`
3. upload or paste the same demo input you used in Copilot Studio
4. rerun the same prompt flow

Microsoft notes that existing conversations can still show older behavior or
cached results. Use a new conversation if the newest version does not appear.

### 6. Choose the availability path

After publishing and adding the channel, open `Availability options`.

You currently have these practical choices:

#### Option A - Share Link

Use this for a very small internal test if the target users already have access
to the agent.

#### Option B - Show to my teammates and shared users

Use this for a small hackathon test group.

This is the best next step after personal testing.

#### Option C - Show to everyone in my org

Use this to submit the agent for admin approval so it appears more broadly in
the Teams app store or Microsoft 365 Agent Store.

Only do this once the agent is stable enough for a wider audience.

#### Option D - Download .zip

Use this if you want the admin-managed route through Microsoft 365 admin
center.

## Fastest Recommended Path For This Demo

Use this order:

1. `Publish`
2. `Teams and Microsoft 365 Copilot` channel
3. `Make agent available in Microsoft 365 Copilot`
4. `See agent in Teams`
5. open Microsoft 365 Copilot or Copilot Chat
6. test it yourself
7. only then share it more broadly

This is the cleanest way to move from private test to real use.

## Admin-Center Route

If your organization prefers central deployment:

1. in Copilot Studio, go to the channel availability options
2. download the `.zip`
3. in Microsoft 365 admin center, open Copilot Control System
4. go to `Agents > All agents > Upload custom agent`
5. upload the `.zip`
6. assign it to `Just me`, a test group, or a broader audience
7. finish deployment

This path is useful when rollout should be governed centrally.

## Recommended Rollout Order

1. just me
2. small test group
3. broader internal release if needed

Do not jump to organization-wide distribution before one clean live run.

## Operational Notes

- after changes, publish again so users see the latest content
- Teams and Microsoft 365 can cache prior state, so reinstall or start a fresh
  session if updates do not appear immediately
- if you change visible app details after admin approval, a fresh approval may
  be required
- if you only changed agent content and not the visible catalog details,
  Microsoft says you can republish without going through a new admin approval
  cycle
- users who installed an earlier app-store version might need to reinstall to
  see changed icon or description details

## Best Recommendation For This Project

For the current hackathon package:

1. publish from Copilot Studio
2. add the Teams and Microsoft 365 Copilot channel
3. install it for yourself first
4. if the live run works, share it to a small audience
5. use admin approval or admin-center deployment only if you need broader
   visibility

## Official Microsoft References

- https://learn.microsoft.com/en-us/microsoft-copilot-studio/publication-add-bot-to-microsoft-teams
- https://learn.microsoft.com/en-us/microsoft-copilot-studio/microsoft-copilot-extend-copilot-extensions
- https://learn.microsoft.com/en-us/copilot/microsoft-365/agent-essentials/m365-agents-admin-guide
