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

Do not share or commit credentials, API keys, or private document IDs. Configure those inside your own n8n instance.

### 2. Upload and convert the Second Brain spreadsheet

1. Download [`Second Brain - Inbox.xlsx`](sheets/Second%20Brain%20-%20Inbox.xlsx).
2. Upload it to your Google Drive.
3. Open the uploaded `.xlsx` file with Google Sheets.
4. Convert it to a native Google Sheet rather than leaving it as an Excel file.
5. Use the resulting Google Sheet when configuring the imported n8n workflows.

That is the complete initial setup. The Google Sheet serves as the memory and action layer for the workflows.

## Included files

| File | Purpose |
|---|---|
| [`workflows/Second Brain - Chat Input.json`](workflows/Second%20Brain%20-%20Chat%20Input.json) | n8n workflow for sending input into the Second Brain |
| [`workflows/Second Brain - Daily Report.json`](workflows/Second%20Brain%20-%20Daily%20Report.json) | n8n workflow for generating a daily report |
| [`sheets/Second Brain - Inbox.xlsx`](sheets/Second%20Brain%20-%20Inbox.xlsx) | Spreadsheet to upload to Drive and convert into Google Sheets |
| [`docs/user-profile.md`](docs/user-profile.md) | Optional profile document template for describing the user |
| [`sheets/second-brain-schema.csv`](sheets/second-brain-schema.csv) | Lightweight reference schema for the memory/action layer |

## 30-Day AI Second Brain Challenge

The challenge graphic is included above as the visual for this project. Start with the two setup steps, then use the system consistently throughout the 30-day challenge. Additional instructions and the official YouTube walkthrough will be added here when they are finalized.

## Sponsorship and affiliate disclosure

This video was sponsored by n8n.

If you are not already using n8n, you can sign up through my affiliate link: [n8n Affiliate Link](https://n8n.partnerlinks.io/SolomonChristAI).

## Safety and privacy

- Review every imported workflow before activating it.
- Use your own credentials and least-privilege access wherever possible.
- Do not put passwords, API keys, recovery codes, or other secrets in the spreadsheet or profile document.
- Confirm that the Google Sheet permissions are appropriate before connecting it to n8n.
