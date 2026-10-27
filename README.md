# AI Voice Booking Automation

An AI-powered appointment-booking system built with Vapi and n8n.

## What it does

1. A customer speaks with the Vapi voice assistant.
2. The assistant checks Google Calendar availability.
3. It creates a confirmed appointment.
4. Vapi extracts booking information after the call.
5. Vapi sends the end-of-call report to n8n.
6. n8n adds the booking information to Google Sheets.

## Workflow overview

![n8n workflow overview](workflow-overview.png)



## Extracted fields

- Customer name
- Email address
- Appointment type
- Appointment date and time
- Call summary

## Technologies used

- Vapi
- n8n
- Google Calendar
- Google Sheets
- GitHub

## Setup

1. Import the workflow JSON into n8n.
2. Connect Google Calendar and Google Sheets credentials.
3. Configure the spreadsheet and webhook values.
4. Add the production n8n webhook URL to Vapi.
5. Enable the `end-of-call-report` server message.
6. Activate the n8n workflow.

## Security

This repository contains a sanitized version of the workflow. Credentials,
customer information, production webhook URLs, and private resource IDs are
not included.
