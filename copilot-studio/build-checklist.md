# Build Checklist

## Before You Start

- Use one Copilot Studio agent only.
- Use embedded files only.
- Do not add SharePoint knowledge, actions, or flows for the first build.
- If you are updating an existing agent instead of building a new one, use
  `copilot-studio/update-existing-agent.md`.

## Build Steps

1. Create a new English-language agent in Copilot Studio.
2. Upload every file from `copilot-studio/upload-pack/` as embedded knowledge.
3. Paste `copilot-studio/agent-instructions.txt` into the instructions field.
4. Paste `copilot-studio/agent-description.txt` into the description field.
5. Replace the default greeting or conversation-start text with
   `copilot-studio/welcome-message.txt`.
6. Add the first four prompts from `copilot-studio/suggested-prompts.md` as
   visible suggested prompts.
7. Keep the reserve prompt outside the visible list unless you want a fifth
   demo path.
8. Enable file uploads in the agent settings.
9. Keep web browsing and actions disabled.

## Runtime Steps

1. Open a fresh test chat.
2. Optionally run the overview prompt first so the agent explains its core
   capabilities.
3. Upload a relevant source file or paste source text directly into the chat.
   Suitable runtime uploads include PDF, TXT, or CSV files.
4. Run the press release prompt.
5. Run the BBC interview briefing prompt.
6. Run the British-humour commentary prompt.
7. Use `copilot-studio/dry-run-checklist.md` to evaluate the outputs.

## After A Successful Dry Run

Continue with:

- `copilot-studio/publish-to-m365-copilot.md`
