# Invoice OCR — Google Form (n8n Workflow)

Automates invoice data extraction from PDF uploads via Google Form.
Powered by Gemini Vision OCR and logged to Google Sheets.

## What It Does
- User submits a Google Form with one or more invoice PDFs
- Workflow downloads each file from Google Drive
- Gemini 2.5 Flash extracts invoice fields (supplier, date, line items, expense category)
- Results are written to Google Sheets — one row per line item
- Confirmation email sent to submitter when done

## Tech Stack
- n8n (workflow automation)
- Google Forms + Google Sheets (intake + storage)
- Google Drive (file storage)
- Gemini 2.5 Flash (Vision OCR)
- Gmail (email notification)

## Setup
1. Import the workflow JSON into n8n
2. Replace all `YOUR_GOOGLE_SHEET_ID` with your Sheet ID
3. Replace `YOUR_GEMINI_API_KEY` with your key from [Google AI Studio](https://aistudio.google.com/app/apikey)
4. Connect your Google Sheets, Drive, and Gmail OAuth2 credentials
5. Activate the workflow

## Part of
[Myvan Automation Lab](https://github.com/moomoo9172) — AI-powered workflow automation for SMEs
