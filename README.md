# Autonomous HubSpot Lead Follow-up Agent

## Overview
An AI-powered lead evaluation and follow-up workflow built with n8n, HubSpot, and Google Gemini. It analyzes available contact information, assigns lead scores, prioritizes leads, and recommends suitable follow-up actions.

## Key Features
- Fetches and normalizes contacts from HubSpot CRM.
- Checks contact information and flags records that need review.
- Uses Google Gemini to evaluate leads and assign scores from 0–100.
- Categorizes leads as High, Medium, or Low priority.
- Recommends actions such as Send Follow-up, Request Information, No Action, or Review Contact.
- Generates personalized follow-up email drafts.
- Produces lead decision reports and summaries.
- Routes leads according to their recommended actions.

## Workflow
1. Retrieve contacts from HubSpot.
2. Normalize and verify contact information.
3. Evaluate leads using an AI Agent.
4. Score and classify leads.
5. Generate recommended actions and reports.
6. Route leads through the appropriate action branch.
7. Send follow-up emails through Gmail when the Send Follow-up branch is executed.

## Technologies Used
- n8n
- HubSpot CRM
- Google Gemini
- Gmail
- JavaScript
- AI Agents
- Structured Output Parser

## Setup
1. Import the workflow JSON into n8n.
2. Configure your own HubSpot, Google Gemini, and Gmail credentials.
3. Verify the HubSpot contact property mappings.
4. Test the workflow using safe test contacts before enabling real email sending.

## Important Note
The Gmail node sends real emails through the Send Follow-up branch. Review and test this step carefully before using the workflow with real contacts.

## Project Purpose
To demonstrate how AI agents can support lead evaluation, prioritization, decision-making, and follow-up automation within a CRM workflow.
