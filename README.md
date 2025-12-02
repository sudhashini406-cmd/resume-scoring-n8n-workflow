Resume Scoring n8n Workflow

This repository contains an n8n workflow that:

Accepts a resume file (PDF)

Extracts the text

Sends the text to an AI model for scoring (OpenAI or n8n AI)

Saves the results in a Google Sheet

Workflow Steps
1. Extract Resume Text

Parses the PDF and converts it to plain text.

2. AI Resume Analyzer

Analyzes the text and returns:

Summary

Score (1–10)

Note: AI scoring requires n8n AI credits or an OpenAI API key.

3. Format Output

Prepares fields for saving:

candidateName

extractedSummary

aiScore

timestamp

4. Store in Google Sheets

Appends the data into a sheet called Resume Scores.

Files

workflow.json → n8n workflow export

Usage

Import the JSON file into n8n

Add your Google Sheets credentials

Add n8n AI or OpenAI credentials

Run the workflow
