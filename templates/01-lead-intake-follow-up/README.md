# Template 001: Google Calendar → Daily Agenda Email

## Problem

Busy professionals and business owners often forget appointments, meetings, and deadlines because they don't have a simple daily overview of what's scheduled for the next day.

## Solution

This n8n workflow will:

1. Run automatically once per day
2. Retrieve all events scheduled for tomorrow from Google Calendar
3. Filter out cancelled events
4. Normalize and organize event details
5. Sort events chronologically
6. Generate a responsive HTML email
7. Send a daily agenda email through Gmail

If no events are scheduled, the workflow sends a clean "No events scheduled" reminder instead.

## Initial Tools

- n8n
- Google Calendar
- Gmail
- JavaScript
- HTML Email Template

## Workflow Status

✅ Version 1 Complete

## Features

- Daily automated email
- Responsive HTML email design
- Supports all-day events
- Supports timed events
- Chronological event sorting
- Handles missing titles gracefully
- Handles missing times gracefully
- Handles missing locations and descriptions
- Filters cancelled events
- "No events scheduled" fallback email
- One-click "Open in Google Calendar" buttons

## Planned Improvements

```text
Google Calendar
        │
        ▼
Scheduled Trigger (Daily)
        │
        ▼
Retrieve Tomorrow's Events
        │
        ▼
Filter & Normalize Events
        │
        ▼
Generate HTML Email
        │
        ▼
Send Daily Agenda Email
```
Form Submission
      ↓
Validate Required Fields
      ↓
Clean Lead Data
      ↓
Check for Existing Email
      ↓
Add or Update Google Sheets
      ↓
Send Lead Confirmation
      ↓
Notify Business Owner
