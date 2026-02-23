# Message Management Guide

This guide provides detailed instructions for sending and managing messages through the **Messaging Management** page.

## Overview

The **Messaging Management** page lets you send messages and notifications to your sales team. Messages can be broadcast to all employees simultaneously and set to different priority levels to ensure important communications get noticed.

## Accessing the Messaging Management Page

1. Log in to the OWPG Admin Portal
2. Click **messages** in the left sidebar
3. You'll see a table with all active and inactive messages
4. Action buttons and message forms are below the table

## Understanding the Messages Table

The table displays the following information for each message:

| Column | Description |
| --- | --- |
| **Message ID** | Unique identifier for the message |
| **Message** | The text content of the message |
| **Start Date** | When the message was created (YYYY-MM-DD HH:MM:SS) |
| **Priority** | Importance level: High, Medium, or Low |
| **Active** | Whether the message is currently active/visible to employees |

### Understanding Message Status

- **Active (checked)**: Message is visible to employees on their mobile app
- **Inactive (unchecked)**: Message is archived but not shown to employees
- **Priority**: Indicates how important the message is

### Table Features

- **Sorting**: Click column headers to sort messages
- **Inline Editing**: 🚩🚩Click editable cells to change values directly
- **Live Updates**: Changes apply immediately without needing a save button
- **Selection**: Use checkboxes to select messages for deletion

## Message Priority Levels

Use priority levels to indicate urgency and importance:

### 🔴 High Priority

Use for urgent, time-sensitive information:

- "Important: All vehicles must return by 5 PM today"
- "Safety alert: Check tire pressure before any trip"
- "System maintenance: App will be unavailable 2-4 AM tonight"
- "Immediate action required"

High priority messages should:

- Be concise and actionable
- Require immediate attention
- Be used sparingly (not every message should be high priority)

### 🟡 Medium Priority

Use for standard operational information:

- "Reminder: Complete vehicle inspections"
- "Upcoming: Training session scheduled for Friday"
- "Update: New customer database is live"
- "Notice: Office will be closed next Monday"

Medium priority messages:

- Are important but not urgent
- Can wait a day or two for action
- Are routine operational notifications

### 🟢 Low Priority

Use for informational or optional messages:

- "Tip: Clean your vehicle inside before return"
- "Reminder: Submit time-sheets by Friday"
- "FYI: Break room has fresh coffee"
- "Optional: Webinar on sales techniques today"

Low priority messages:

- Are for information only
- Don't require immediate action
- Can be archived without impact

## Core Actions

### 1. Send a New Message

Create and broadcast a message to your team.

**How to:**

1. Scroll to the **"Write a New Message"** form (left side at bottom)
2. Fill in the required fields:
   - **Message**: Type your message text (keep it clear and concise)
   - **Priority Level**: Select from dropdown (High, Medium, or Low)
   - **Active**: Check the box if message should be visible immediately
3. Click **Send** button

**What happens:**

- Message appears in the table
- If "Active" is checked, employees see it immediately in their mobile app
- If "Active" is unchecked, message is stored but hidden (you can activate later)
- Form clears and is ready for a new message

**Message Composition Tips:**

✅ **Do:**  

- Be clear and specific about what action is needed
- Include relevant dates and times
- Use proper punctuation and capitalization
- Keep messages concise (under 280 characters recommended)
- Consider mobile screen size — shorter is better

❌ **Don't:**

- Use ALL CAPS (except for emphasis on specific words)
- Use excessive punctuation or emojis
- Assume recipients saw previous messages
- Make vague requests ("Call someone," "Let me know")
- Send duplicate messages in quick succession

**Example messages:**

| Bad | Good |
| --- | --- |
| "Check stuff" | "Vehicle inspections must be completed before each trip" |
| "URGENT URGENT URGENT" | "High Priority: Return all vehicles by 5 PM" |
| "Blah blah meeting" | "Training session: Friday 2 PM in Conference Room A" |

### 2. Modify Message Priority

Change the priority level of an existing message.

**How to:**

1. Locate the message in the table
2. Click the **Priority** cell for that message
3. A dropdown appears with options: High, Medium, Low
4. Select the new priority
5. Change applies immediately

**Example scenarios:**

- Message was set as Medium but it's now urgent → change to High
- Initial announcement completed → change from High to Medium or Low
- Routine reminder being archived → change to Low before deactivating

### 3. Activate or Deactivate Messages

Show or hide messages from employees.

**How to:**

1. Locate the message in the table
2. Click the **Active** checkbox column for that message
3. Checkbox toggles between checked (active) and unchecked (inactive)
4. Change applies immediately

**When to activate:**

- After creating a message that should be visible
- When reactivating a message that was temporarily hidden
- When posting urgent communications

**When to deactivate:**

- When message is outdated (training ended, deadline passed)
- When archiving a message but keeping it in records
- When you need to hide a message temporarily

**Important notes:**

- Deactivating does NOT delete the message — it's still in the table
- Re-activate anytime by clicking the checkbox again
- Employees won't see inactive messages in their mobile app
- Message data is preserved for record-keeping

### 4. Delete Messages

Permanently remove a message from the system.

⚠️ **Warning**: Deleting is permanent and cannot be undone.

**When to delete:**

- When clearing out old/obsolete messages
- When a message was sent in error
- When maintaining a clean, organized message list

**How to:**

1. Select one or more messages using the checkboxes
2. Click the **Delete** button (shown in red)
3. A confirmation dialog appears asking: "Are you sure you want to delete these messages? This action cannot be undone."
4. Click **Yes** to confirm or click outside to cancel
5. Messages are immediately removed

**Before deleting:**

- Ensure you have the correct message(s) selected
- Consider deactivating instead if you want to keep the record
- Check if the information needs to be preserved for compliance

**What happens after deletion:**

- Message is permanently removed from the table
- Employees no longer see it
- Cannot be recovered or restored
- Message history is lost

## Advanced Features

### Bulk Operations

Delete multiple messages at once:

1. Click the header checkbox to select all messages, or individually select specific messages
2. Click the **Delete** button
3. Confirm deletion for all selected messages

### Message Lifecycle Example

Here's a typical message lifecycle:

#### Day 1: Send Message

1. Write new message: "Training session Friday 2 PM"
2. Set priority to Medium
3. Check "Active" box
4. Click Send
5. Employees see message immediately

#### Day 3: Modify Priority

1. Locate the message in table
2. Click Priority cell
3. Change from Medium to Low (training is starting soon, less new info)
4. Change applies

#### Day 4: Deactivate

1. Click Active checkbox to uncheck
2. Message hides from employees (training happened)
3. Still visible to admin in table

#### Day 30: Delete

1. Select message checkbox
2. Click Delete
3. Confirm deletion
4. Message is gone

### Filtering & Finding Messages

**Find a specific message:**

1. Use browser Find (Ctrl+F on Windows, Cmd+F on Mac)
2. Search by message text, ID, or date
3. Matching results highlight in the table

**🚩🚩View only active messages:**

1. Look at table to see which messages have Active checkbox checked
2. Note that inactive messages still appear but are grayed out

## Common Tasks

### Task: Send a Time-Sensitive Announcement

1. Go to **messages**
2. Scroll to "Write a New Message" form
3. Type: "Important: All vehicles must return by 5 PM today for maintenance"
4. Select **Priority: High**
5. Check "Should this message be active right away?"
6. Click **Send**
7. Message appears immediately to all employees

### Task: Routine Daily Reminder

1. Go to **messages**
2. Type: "Daily reminder: Complete vehicle inspections before departing"
3. Select **Priority: Medium**
4. Leave "Active" checked or uncheck if sending for tomorrow
5. Click **Send**

### Task: Archive Old Messages

1. Review table of messages
2. Find messages that are outdated (date passed, event happened, etc.)
3. Select the message(s) you want to hide
4. Click Active checkbox to uncheck (deactivate)
5. Messages no longer appear to employees

### Task: Clean Up Message Clutter

1. Find all inactive/archived messages
2. Select multiple inactive messages
3. Click **Delete** button
4. Confirm deletion
5. System is cleaned up for new messages

### Task: Update Message Urgency

1. Find a message in table
2. Example: Emergency announcement initially marked High priority
3. Once situation resolves, click Priority cell
4. Change to Medium or Low
5. Or deactivate entirely if resolved

## Best Practices for Messaging

### ✅ Effective Messages

- **Be specific**: "Bring all vehicles back by 5 PM" vs. "Return vehicles"
- **Include dates/times**: Use complete date format when relevant
- **Consider recipients**: Are all employees the right audience?
- **Use appropriate priority**: Match urgency level to priority
- **Keep it brief**: Employees read on mobile phones
- **One topic per message**: Don't combine unrelated items

### ❌ Common Mistakes

- Creating duplicate messages
- Setting everything as High priority (dilutes urgency)
- Forgetting to deactivate outdated messages
- Vague or unclear instructions
- Typos and grammatical errors
- Sending too many messages too quickly

## Message Examples by Scenario

### Safety-Related (High Priority)

"⚠️ Safety Alert: Check tire pressure and fluid levels before each trip. Report any issues immediately."

### Operational (Medium Priority)

"Reminder: Vehicle inspections are due by end of week. Complete them before your next departure."

### Procedural Change (High Priority)

"Important: New customer database is live. Use the updated system for all customer information."

### General Information (Low Priority)

"Tip: Ensure vehicles are clean inside and out before returning to the lot."

### Event Notification (Medium Priority)

"Training session scheduled: Thursday 2 PM, Conference Room A. Sales techniques workshop."

### Urgent Action (High Priority)

"Action Required: All vehicles must return by 2 PM for emergency maintenance inspection."

## Troubleshooting

### Message Won't Save

**What it means:** The message may have content issues.

**Solution:**

- Check that message text is not blank
- Verify text isn't excessively long
- Try again or contact administrator

### Can't Change Priority Level

**What it means:** The message table might not be responding.

**Solution:**

1. Refresh the page (F5)
2. Try clicking the cell again
3. If it still doesn't work, contact administrator

### Message Appears to Disappear

**What it means:** You probably deactivated it by unchecking the Active box.

**Solution:**

1. Look at the table (it's still there but grayed out)
2. Check the Active box to reactivate
3. Message will be visible to employees again

### Employees Didn't See My Message

**Possible causes:**

1. Message might not be set to Active
2. Message was created but not marked Active initially
3. There might be a delay in synchronizing with mobile app
4. Employees might not have the latest app version

**Solution:**

1. Verify the Active checkbox is checked in the table
2. Create a new test message marked as Active
3. Wait a few minutes for sync
4. Contact administrator if issue persists

### Can't Delete a Message

**What it means:** You might not have permission or there's a system issue.

**Solution:**

1. Refresh the page (F5)
2. Try again
3. If it persists, contact your administrator

## Data & Message Retention

### Message Storage

- **Message content**: Stored permanently in database
- **Activation/deactivation history**: Not tracked (only current status)
- **When deleted**: Cannot be recovered
- **Archives**: Deactivate messages instead of deleting if you need records

### Employee View

- Employees only see **Active** messages in their mobile app
- They cannot see or delete messages themselves
- Message history may be available to them (depends on app version)

## Related Documentation

- [Getting Started Guide](../../GETTING_STARTED.md) — First-time setup
- [Vehicle Management](VEHICLES.md) — Managing BLE tags and vehicles
- [Employee Management](PEOPLE.md) — Managing user accounts
- [Main README](../../README.md) — System overview

---

For additional help, contact your system administrator.
