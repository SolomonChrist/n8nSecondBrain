# Second Brain Setup Prompts

These are the prompts used to build and upgrade the personal Second Brain system one stage at a time. Replace bracketed placeholders with your own values when needed.

## Prompt 1

We are building a SIMPLE personal Second Brain in n8n, one stage at a time. Please first inspect available nodes and my n8n version. Propose the smallest workflow for Stage 1: authenticated chat input -> validate text -> append a row to a Google Sheet -> confirm storage. Show me the node plan and required credentials before creating anything. Never publish or alter a live workflow, or expose secrets without asking. After building, test with a fictional note and report the actual execution result.

## Prompt 2

Open my Second Brain - Inbox sheet and make a tab called 'Memory' with id, captured_at, type, title, note, person_or_project, due_date, status, source, file_url, last_updated. Make a second tab 'Actions' with id, proposed_action, frequency, owner, approval_status, last_run, next_run, outcome; show only the basic columns necessary now, leave the rest for later. Keep rows human-readable.

## Prompt 3

Update our n8n workflow to match the memory and action system. We also want to be able to have a daily email sent to us via n8n using the gmail node that gives us an update using AI to tell us the most useful things I should pay attention to based on the previous days notes ONLY. Do not go back more than a WEEK.

## Prompt 4

Using ONLY the supplied active sheet rows, write a Daily Three email. Section 1 WHAT MATTERS: up to three dated commitments, earliest due first. Section 2 WHAT IS NEXT: one concrete next action per commitment. Section 3 WHAT AI CAN PREPARE: at most two draft ideas, with no auto-sending. Include sheet row IDs, never invent people, dates or promises, and say "No verified item" where needed. Under 180 words. Update the workflows and spreadsheet

## Prompt 5

I want you to upgrade the daily report email and make it more visually appealing. Add better HTML and UI/UX to make it look easy to read and like a world class UI/UX person created the email. From there I want to make it so that when I chat via n8n, the AI will take my chat and extract things that are done or marked done so they do not show up in a next report. I also want the AI to take action on anything I approve and do things (Like outline draft for the nova project) and keep the output inside of the google drive and give me a link to that created file which could be a google doc, google slides or some other artifact.

## Prompt 6

Here is my Google Drive folder for my AI Second Brain files: [YOUR FOLDER URL]

Keep the memory sheet. Add file_url, file_type, short_summary, extraction_status, updated_at if not present. Upload a fictional invoice PDF and a fictional receipt photo using the same chat interface as we are upgrading the n8n chat to now include file uploads. Keep the originals unchanged and make sure they upload to this folder.

## Prompt 7

I want you to now upgrade the workflows and add my Gmail and Google Calendar so that you get the last 7 days of emails and events and we can add that to our Daily THREE report

## Prompt 8

I want to see my calendar and email items that are important and only read 25 messages and 25 of the last calendar entries and then tell me. I also should have my main system and spreadsheet take that data as well as emails come in and the past 25 emails if they are NOT already in the spreadsheet so that they are able to be placed in my daily report.

## Prompt 9

Here are my Brain Rules which has information about me that I will update over time. I want this to be in my system so that when I'm working with AI from my n8n Second Brain system, this becomes the operating manual for my assistants.

[YOUR DOCUMENT URL]
