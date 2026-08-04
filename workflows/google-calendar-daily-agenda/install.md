# Installation Guide

This guide walks you through connecting the workflow to your own Google Calendar and Gmail accounts.

---

# Requirements

Before importing the workflow, you'll need:

- n8n (Cloud or Self-Hosted)
- A Google account
- Google Calendar
- Gmail
- Google OAuth2 credentials

---

# Step 1 — Import the Workflow

1. Download the workflow JSON.
2. Open n8n.
3. Click **Import from File**.
4. Select:

```
google-calendar-daily-agenda.json
```

The workflow will import with all nodes already configured.

---

# Step 2 — Create Google Calendar Credentials

Open the **Get Tomorrow's Events** node.

Under **Credentials**:

Click

**Create New Credential**

Select

**Google Calendar OAuth2 API**

Complete the Google OAuth connection.

After connecting, save the credential.

---

# Step 3 — Create Gmail Credentials

Open the **Send Daily Agenda Email** node.

Under **Credentials**

Click

**Create New Credential**

Select

**Gmail OAuth2 API**

Complete the OAuth login.

Save the credential.

---

# Step 4 — Select Your Calendar

Inside the **Get Tomorrow's Events** node:

Choose the Google Calendar you want to monitor.

Most users should simply choose:

```
Primary
```

---

# Step 5 — Choose the Recipient

Open the **Workflow Settings** node.

Replace the sample email address with your own.

Example:

```
you@example.com
```

---

# Step 6 — Set the Schedule

Open the **Schedule Trigger** node.

Choose when you'd like to receive your agenda.

Example:

**Every day at 9:00 AM**

---

# Step 7 — Test the Workflow

Click

**Execute Workflow**

You should receive a formatted HTML email showing tomorrow's calendar events.

If there are no events scheduled, you'll receive a friendly "No events scheduled" email instead.

---

# Customization

You can easily customize:

- Email colors
- Branding
- Logo
- Button color
- Subject line
- Time format
- Date format
- Footer text

These settings are located inside the **Create Email Content** code node.

---

# Troubleshooting

### No email received

- Verify Gmail credentials are connected.
- Confirm the recipient email is correct.
- Execute the workflow manually.

---

### No events appear

Verify:

- The correct calendar is selected.
- Tomorrow contains events.
- The workflow timezone matches your calendar timezone.

---

### Times appear incorrect

Update the workflow timezone inside:

```
Workflow Settings
```

and ensure your Google Calendar uses the same timezone.

---

# Included Features

- Daily automatic schedule
- Responsive HTML email
- Timed events
- All-day events
- Multiple events
- Empty calendar handling
- Event sorting
- Google Calendar links
- Clean modern design

---

# Support

If you customize this workflow for clients, consider duplicating it before making changes so you always keep a clean master template.
