# 30-Day AI Second Brain Challenge

![30-Day AI Second Brain Challenge](30-Day%20AI%20Second%20Brain%20Challenge.png)

This repository contains the files for setting up the AI Second Brain shown in the video. It is designed for people who already have **n8n** and **Claude** and want to get the core system running quickly.

<p align="center">
  <img src="n8n-symbol-accent.png" alt="n8n" width="120">
</p>

## What you need

- An n8n account or self-hosted n8n installation
- Access to Claude
- A Google Drive account with permission to create Google Sheets

## Setup steps

### 1. Upload the n8n workflows

Open the [`workflows`](workflows/) folder and download the workflow JSON files:

- [`Second Brain - Chat Input.json`](workflows/Second%20Brain%20-%20Chat%20Input.json)
- [`Second Brain - Daily Report.json`](workflows/Second%20Brain%20-%20Daily%20Report.json)

In n8n, import each JSON file using the workflow import option. After importing, connect your own credentials and configure the required Google Sheets, Claude, and other service connections shown in the workflow.

Before activating a workflow, search its imported settings for the placeholder values beginning with `YOUR_` and replace them with your own details. In particular, configure `YOUR@EMAIL.COM`, `YOUR_SHEET_ID`, `YOUR_MEMORY_TAB_ID`, `YOUR_ACTIONS_TAB_ID`, `YOUR_N8N_CHAT_URL`, and `YOUR_KEY` where applicable. The key should be a new private value stored in your n8n credential or secret-management setup.

Do not share or commit credentials, API keys, or private document IDs. Configure those inside your own n8n instance.

### 2. Upload and convert the Second Brain spreadsheet

1. Download [`Second Brain - Inbox.xlsx`](sheets/Second%20Brain%20-%20Inbox.xlsx).
2. Upload it to your Google Drive.
3. Open the uploaded `.xlsx` file with Google Sheets.
4. Convert it to a native Google Sheet rather than leaving it as an Excel file.
5. Use the resulting Google Sheet when configuring the imported n8n workflows.

That is the complete initial setup. The Google Sheet serves as the memory and action layer for the workflows.

### 3. Open the user profile as a Google Doc

1. Open [`docs/user-profile.md`](docs/user-profile.md) from this repository.
2. Copy its contents into a new Google Doc, or upload/open the Markdown file and save it as a Google Doc.
3. Complete the profile with the user's information, goals, priorities, preferences, and approval boundaries.
4. Keep the completed Google Doc available as the user's instruction and context document.

## Included files

| File | Purpose |
|---|---|
| [`workflows/Second Brain - Chat Input.json`](workflows/Second%20Brain%20-%20Chat%20Input.json) | n8n workflow for sending input into the Second Brain |
| [`workflows/Second Brain - Daily Report.json`](workflows/Second%20Brain%20-%20Daily%20Report.json) | n8n workflow for generating a daily report |
| [`sheets/Second Brain - Inbox.xlsx`](sheets/Second%20Brain%20-%20Inbox.xlsx) | Spreadsheet to upload to Drive and convert into Google Sheets |
| [`docs/user-profile.md`](docs/user-profile.md) | User profile to open or upload as a Google Doc |
| [`Second Brain Transfer Prompt.md`](Second%20Brain%20Transfer%20Prompt.md) | Reference material for the project; not part of the user setup steps |

### Finished versions

The finished versions are also included for users who want the completed files shown in the video:

- [`workflows-finished/Second Brain - Chat Input - FINISHED.json`](workflows-finished/Second%20Brain%20-%20Chat%20Input%20-%20FINISHED.json)
- [`workflows-finished/Second Brain - Daily Report - FINISHED.json`](workflows-finished/Second%20Brain%20-%20Daily%20Report%20-%20FINISHED.json)
- [`sheets-finished/Second Brain - Inbox - FINISHED.xlsx`](sheets-finished/Second%20Brain%20-%20Inbox%20-%20FINISHED.xlsx)

## 30-Day AI Second Brain Challenge

After watching the video, go ahead and build out your very own Second Brain AI OS System. The goal is simple: use the Second Brain consistently for the next 30 days and save **3 or more hours** during that period. Track the time saved as you capture ideas, manage actions, and use your system daily.

After 30 days and hitting success, don't just stop there! Repeat the process again for 6 months. Keep upgrading and updating the system and it will help you save REAL time! YOU GOT THIS!!

Please share your results in the [n8n Community](http://community.n8n.io/) and make sure to tag `@solomonchrist` and share your amazing results with the world!!

## Reference material

[`Second Brain Transfer Prompt.md`](Second%20Brain%20Transfer%20Prompt.md) is included for reference and project context. It is not intended to be used by end users as part of the setup process.

## Sponsorship and affiliate disclosure

This video was sponsored by n8n.

If you are not already using n8n, you can sign up through my affiliate link: [n8n Affiliate Link](https://n8n.partnerlinks.io/SolomonChristAI).

## Safety and privacy

- Review every imported workflow before activating it.
- Use your own credentials and least-privilege access wherever possible.
- Do not put passwords, API keys, recovery codes, or other secrets in the spreadsheet or profile document.
- Confirm that the Google Sheet permissions are appropriate before connecting it to n8n.
