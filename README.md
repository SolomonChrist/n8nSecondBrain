# n8n Second Brain Starter Kit

This project packages the assets a new user needs to get an n8n-based second brain running:

- `docs/user-profile.md` — paste-ready Google Doc template describing the user.
- `sheets/second-brain-schema.csv` — importable Google Sheets schema for memory and actions.
- `workflows/` — n8n workflow exports (to be added in the next build pass).

## Intended setup flow

1. Copy `docs/user-profile.md` into a new Google Doc and complete the prompts.
2. Import `sheets/second-brain-schema.csv` into a new Google Sheet.
3. Import the n8n workflows from `workflows/`.
4. Add credentials and environment-specific IDs in the workflow configuration.
5. Run the setup/check workflow before enabling automations.

## Design principles

- Human-readable source files are the canonical templates.
- The spreadsheet separates durable memory from actionable work.
- Workflows should be safe to run repeatedly and should avoid silently overwriting user data.
- Secrets and provider-specific IDs belong in n8n credentials or environment variables, never in exports.
