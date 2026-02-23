# Vehicle Management Guide

This guide provides detailed instructions for managing your fleet's BLE tags through the **Vehicles** page.

## Overview

The **Vehicles** page is your central hub for managing all BLE tags in your fleet. A BLE tag is a tracking device attached to each vehicle that records its location, trip data, and operational status.

## Accessing the Vehicles Page

1. Log in to the OWPG Admin Portal
2. Click **Vehicles** in the left sidebar
3. You'll see a table listing all your tags with their current status and information

## Understanding the Vehicles Table

The table displays the following information for each tag:

| Column | Description |
| --- | --- |
| **Tag ID** | Unique identifier for the BLE tag (DMAC address) |
| **Location** | Where the vehicle is currently located |
| **Vehicle Description** | Name/description of the vehicle (e.g., "Blue F-150 Truck") |
| **Activation Date** | When the tag was activated |
| **Deactivation Date** | When the tag was deactivated (blank if currently active) |
| **Days in Service** | Total number of days the tag has been active |
| **Battery Life** | Remaining battery percentage with color indicator |
| **Status** | ACTIVE or INACTIVE |

### Battery Life Indicator

The battery life column shows a visual progress bar with color coding:

- 🟢 **Green** (80-100%): Good condition
- 🟡 **Yellow** (60-80%): Acceptable, monitor
- 🟠 **Orange** (40-60%): Replace soon
- 🔴 **Red** (0-40%): Replace immediately

## Selecting Tags

To select one or more tags:

1. Check the box(es) next to the tag(s) you want to work with
2. Check the header box to select/deselect all tags
3. Selected tags are highlighted in blue
4. Buttons appear based on your selection:
   - **View Details** (requires exactly 1 tag selected)
   - **Activate** (for inactive tags)
   - **Deactivate** (for active tags)
   - **Delete** (for any selected tags)

## Core Actions

### 1. View Details

View comprehensive information about a specific vehicle and its usage history.

**How to:**

1. Select exactly one tag by clicking its checkbox
2. Click the **View Details** button
3. A panel opens showing:
   - Vehicle and tag information
   - Current status (ACTIVE/INACTIVE)
   - Days in service
   - **Test Drives** table with trip history

**Trip Information Displayed:**

- **Trip ID**: Unique identifier for the test drive
- **Vehicle Taken**: Which vehicle was used
- **Taken By**: Which employee has taken the vehicle
- **Reason**: Purpose of the trip
- **Customer Name**: Who used the vehicle
- **Start Time**: When the trip began
- **End Time**: When the trip ended
- **Trip File**: Reference to detailed trip data

**Viewing Trip Maps (if available):**

1. Click on a row in the Test Drives table
2. If available, a map shows the vehicle's route during that trip
3. The map displays all waypoints and the path taken

### 2. Add a New Tag

Register a new BLE tag in the system to track a new vehicle.

**How to:**

1. Scroll to the **"Add a New Tag"** section at the bottom
2. Enter the **New Tag ID** (click the QR code camera if your browser supports it, or enter manually)
3. Location is auto-filled with your facility's location code
4. Enter **Vehicle Description** (e.g., "Red Honda Civic - Sales")
5. Click **Add Tag** button

**Tag ID Format:**

- The Tag ID is typically a DMAC address (e.g., `00:1A:2B:3C:4D:5E`)
- System automatically converts to uppercase
- Must be unique — you can't add the same tag twice

**Important Notes:**

- The location is determined by your current facility code

### 3. Activate Tags

🚩🚩Activate a tag to start tracking a vehicle.

**When to activate:**

- After initially adding a tag to a vehicle
- When restarting service for a previously inactive vehicle
- When replacing a tag on an active vehicle

**How to:**

1. Select one or more **INACTIVE** tags (show Status: INACTIVE)
2. Click the **Activate** button
3. A confirmation dialog appears asking to confirm
4. Click **"Yes"** to proceed or click outside the dialog to cancel
5. The tag status changes to **ACTIVE** immediately

**What happens when activated:**

- 🚩🚩Tag starts recording GPS location data
- 🚩🚩Trip information begins being logged
- 🚩🚩Battery usage starts
- Activation date is recorded

### 4. Deactivate Tags

Deactivate a tag to stop tracking a vehicle temporarily.

**When to deactivate:**

- When a vehicle is taken out of service for maintenance
- When a vehicle is sold or transferred
- When storage tracking is not needed
- Before removing a tag from a vehicle

**How to:**

1. Select one or more **ACTIVE** tags (show Status: ACTIVE)
2. Click the **Deactivate** button
3. A confirmation dialog appears asking to confirm
4. Click **"Yes"** to proceed or click outside the dialog to cancel
5. The tag status changes to **INACTIVE** immediately

**What happens when deactivated:**

- Tag stops recording new trip data
- Deactivation date is recorded in the system
- 🚩🚩Battery consumption stops
- Tag can be reactivated later (use Activate button)

### 5. Delete Tags

Permanently remove a tag from the system.

⚠️ **Warning**: Deleting is permanent and cannot be undone. Only delete if you're certain the tag is no longer needed.

**When to delete:**

- When a tag is broken or lost
- When a tag is permanently removed from a vehicle
- When pruning old test/dummy tags from the system

**How to:**

1. Select one or more tags to delete
2. Click the **Delete** button (shown in red/primary color)
3. Confirm your selection is correct
4. The deletion is immediate and permanent

**Before deleting, consider:**

- 🚩🚩Do you need the trip history for records/audit?
- Is the tag still in use elsewhere?
- Have you made a backup of the data if needed?

## Advanced Features

### Bulk Operations

You can select multiple tags to perform actions on them all at once:

1. Click the header checkbox to select all tags, or individually select specific tags
2. Click **Activate**, **Deactivate**, or **Delete** buttons
3. Confirm the action for all selected tags

### Upload Multiple Tags

If you have many tags to add at once, use the **"Or Add Several Tags"** section:

1. Scroll to the bottom of the page
2. Prepare a file with tag information (ask your admin for format)
3. Click **"Drag and/or click to upload a file"**
4. Select your file
5. Click **Add Tags** button

### Monitoring Tag Health

Keep your fleet in good condition:

1. **Check battery levels regularly** — Replace tags showing red (0-40%)
2. **Review days in service** — Track how long each tag has been active
3. **Monitor locations** — Ensure tags are where expected
4. **Verify status** — Confirm tags are active/inactive as intended

## Common Tasks

### Task: Replace a Tag's Battery

1. Locate the tag in the table with low battery (red indicator)
2. Deactivate the tag by selecting it and clicking **Deactivate**
3. Confirm deactivation
4. Physically replace the tag's battery
5. Reactivate by selecting and clicking **Activate**
6. Confirm activation

### Task: Move a Tag to a Different Vehicle

1. Deactivate the tag on its current vehicle
2. Select the tag and click **Deactivate**
3. Physically move the tag to the new vehicle
4. Reactivate the tag by selecting and clicking **Activate**
5. Confirm activation (trip history continues from this point)

### Task: Generate a Report on Vehicle Usage

1. Click **View Details** for each vehicle of interest
2. Review the test drives/trip data
3. Note start times, end times, and customer names
4. Export or print as needed (browser print feature: Ctrl+P)

### Task: Find a Specific Tag

1. Use your browser's Find feature (Ctrl+F on Windows, Cmd+F on Mac)
2. Search for the tag ID you're looking for
3. The table will highlight the matching row

## Tips & Best Practices

✅ **Do:**  

- Check battery levels weekly
- Activate tags before deploying vehicles
- Use descriptive vehicle descriptions
- Confirm all actions before deleting
- Keep tag assignments up-to-date

❌ **Don't:**

- Delete tags without verifying necessity
- Leave batteries below 20% for extended periods
- Ignore red (critical) battery indicators
- Share tag IDs between multiple vehicles
- Deactivate tags without documenting why

## Troubleshooting

### "Cannot activate this tag because it is not on the premises"

**What it means:** The tag needs to be physically present at your facility to be activated.

**Solution:**

1. Ensure the tag is physically at your location
2. Wait a moment for the system to sync with the tag
3. Try again

### "Tag with this ID already exists"

**What it means:** You're trying to add a tag ID that's already in the system.

**Solution:**

1. Check if the tag is already in your table
2. If it shouldn't be, delete the old entry first
3. Use a different tag ID if this is a new tag

### Battery Life Shows "—" or No Value

**What it means:** The tag hasn't reported battery data yet, or the battery sensor is malfunctioning.

**Solution:**

1. Wait 24 hours for data to sync
2. Check if the tag is receiving power
3. If problem persists, replace the tag

### 🚩🚩Can't Find View Details Button

**What it means:** You need to select exactly one tag for View Details to appear.

**Solution:**

1. Uncheck all other checkboxes
2. Check only one tag
3. The View Details button should appear

## Data Retention

- **Vehicle information**: 🚩🚩Stored permanently until tag is deleted
- **Trip data**: Stored for analysis and auditing purposes
- **Battery history**: Tracked over time for maintenance planning
- **Activation/deactivation dates**: Recorded for all status changes

## Related Documentation

- [Getting Started Guide](../../GETTING_STARTED.md) — First-time setup
- [Employee Management](PEOPLE.md) — Managing users who drive vehicles
- [Main README](../../README.md) — System overview

---

For additional help, contact your system administrator.
