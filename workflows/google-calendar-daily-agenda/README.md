# Google Calendar Daily Agenda Email

Automatically sends a clean, professional HTML email every morning summarizing tomorrow's Google Calendar events.

---

## Overview

Many professionals forget to check their calendar until it's too late.

This workflow automatically retrieves tomorrow's events from Google Calendar, formats them into a responsive HTML email, and sends the agenda to your inbox every day.

It supports:

- ✅ Timed events
- ✅ All-day events
- ✅ Multiple events
- ✅ No-event days
- ✅ Missing locations
- ✅ Missing descriptions
- ✅ Automatic chronological sorting

---

## Workflow

![Workflow](workflow.png)

---

## Email Preview

![Email Preview](email-preview.png)

---

## Requirements

- n8n
- Google Calendar OAuth2 credential
- Gmail OAuth2 credential

---

## Features

- Retrieves tomorrow's calendar events
- Formats events into clean HTML cards
- Sorts events by time
- Handles all-day events
- Handles empty calendars
- Includes Google Calendar links
- Responsive email layout
- Beginner-friendly and fully customizable

---

## Nodes Used

1. Schedule Trigger
2. Google Calendar
3. Code (Build Event Objects)
4. Code (Generate HTML)
5. Set
6. Gmail

---

## Installation

See **install.md** for step-by-step setup instructions.

---

## Example Use Cases

- Daily personal agenda
- Executive assistants
- Sales professionals
- Project managers
- Small business owners
- Virtual assistants

---

## License

MIT
