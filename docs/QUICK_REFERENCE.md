# Quick Reference Guide

A quick lookup for common tasks and keyboard shortcuts in the OWPG Admin Portal.

## Keyboard Shortcuts

| Action | Windows | Mac |
| --- | --- | --- |
| Find text on page | Ctrl+F | Cmd+F |
| Refresh page | F5 or Ctrl+R | Cmd+R |
| Zoom in | Ctrl++ | Cmd++ |
| Zoom out | Ctrl+- | Cmd+- |
| Reset zoom to 100% | Ctrl+0 | Cmd+0 |
| Clear browser cache | Ctrl+Shift+Delete | Cmd+Shift+Delete |
| Print page | Ctrl+P | Cmd+P |
| Open browser developer tools | F12 | F12 |

## Navigation Shortcuts

| Feature | Click | Then |
| --- | --- | --- |
| Go to Vehicles | Sidebar → Vehicles | Add/manage tags |
| Go to Messages | Sidebar → Messaging Management | Send/manage messages |
| Go to Employees | Sidebar → Person Management | Create/manage users |
| Go to Home | Sidebar → Home | View features overview |
| Sign Out | Sidebar → Sign Out | Click "Yes" in dialog |

## Common Tasks - Quick Steps

### Add a Vehicle Tag

1. Vehicles page → Scroll to "Add a New Tag"
2. Enter Tag ID
3. Enter Vehicle Description
4. Click **Add Tag**
5. Select tag, click **Activate**

### Add an Employee

1. Person Management page → Scroll to "Add New User" form
2. Email, Password, First Name, Last Name
3. Click **Add new user**
4. Write down User ID and Password
5. Share credentials with employee

### Send a Message

1. Messaging Management page → "Write a New Message" section
2. Type message
3. Select Priority (High/Medium/Low)
4. Check "Active" if immediate visibility needed
5. Click **Send**

### View Employee Trips

1. Person Management page
2. Select one employee
3. Click **View Details**
4. Click on a trip to view route map

### Activate a Tag

1. Vehicles page
2. Select one or more INACTIVE tags
3. Click **Activate**
4. Confirm in dialog

### Deactivate a Tag

1. Vehicles page
2. Select one or more ACTIVE tags
3. Click **Deactivate**
4. Confirm in dialog

### Delete Items (Irreversible)

1. Check checkbox(es) for item(s)
2. Click **Delete** button
3. Click **Yes** to confirm
4. Item permanently removed

## Table Selection Patterns

| Goal | Action |
| --- | --- |
| Select all items | Click header checkbox |
| Deselect all items | Click header checkbox again |
| Select one item | Click that item's checkbox |
| Select multiple items | Click each item's checkbox |
| Select a range | Click first, hold Shift, click last |

## Field Validation Rules

### Tag ID

- Required: Yes
- Format: Any format (typically DMAC address)
- Must be unique: Yes (can't duplicate)
- Case: Auto-converted to uppercase

### User Email

- Required: Yes
- Format: Must include @ and domain (e.g., <user@company.com>)
- Must be unique: Yes (one email per account)
- Case: Auto-converted to lowercase

### Password (New Employees)

- Length: 6-16 characters
- Must contain: Number, Uppercase, Lowercase
- Example: `SecurePass1` ✅

### Message Text

- Required: Yes
- Length: Can be any length (keep brief for mobile)
- Format: Any text
- Recommended: Under 280 characters

### First Name / Last Name

- Required: Yes
- Length: Any length
- Format: Any text
- Case: Preserved as entered

## Status & Color Indicators

### Vehicle Tag Status

- **ACTIVE**: Tag is tracking (green indicator)
- **INACTIVE**: Tag not in use (gray indicator)

### Battery Life Colors

- 🟢 **Green**: 80-100% (Good)
- 🟡 **Yellow**: 60-80% (OK, monitor)
- 🟠 **Orange**: 40-60% (Replace soon)
- 🔴 **Red**: 0-40% (Replace now)

### Message Status

- **Active (checked)**: Visible to employees
- **Inactive (unchecked)**: Hidden from employees

### Priority Levels

- **High**: Urgent/time-sensitive
- **Medium**: Important but not urgent
- **Low**: Informational

## Page Load Wait Times

| Action | Typical Wait Time |
| --- | --- |
| Log in | 2-5 seconds |
| Load Vehicles page | 3-10 seconds |
| Load Messaging page | 2-5 seconds |
| Load Person Management page | 3-10 seconds |
| View employee details | 2-5 seconds |

If page takes longer, try refreshing (F5).

## Buttons & What They Do

### Vehicles Page

- **View Details**: Show vehicle info and trip history (select 1)
- **Activate**: Start tracking a tag (select INACTIVE tags)
- **Deactivate**: Stop tracking a tag (select ACTIVE tags)
- **Delete**: Remove tag permanently (select any)

### Person Management Page

- **View Details**: Show employee trips (select 1)
- **Delete**: Remove employee account (select any)

### Messaging Page

- **Send**: Create and send new message (in form)
- **Delete**: Remove message permanently (select any)

## Data Sync Times

| Data | Typical Sync Time |
| --- | --- |
| New employee account | Instant (2-5 sec) |
| New message | Instant (2-5 sec) |
| New vehicle tag | Instant (2-5 sec) |
| Employee trip data | 24 hours |
| Tag battery data | 24 hours |
| Tag location update | 5-15 minutes |

## Browser & System Requirements

**Minimum Requirements:**

- Modern browser (Chrome, Firefox, Safari, Edge)
- Internet connection
- Display: 1024x768 or larger
- JavaScript: Enabled

**Recommended:**

- Latest browser version
- Broadband internet
- Display: 1366x768 or larger
- Mobile: Works with responsive design

## Common Error Messages & Quick Fixes

| Error | Quick Fix |
| --- | --- |
| "Invalid credentials" | Check username/password, verify CAPS LOCK off |
| "Please log in again" | Session expired, log in again (normal) |
| "User already exists" | Email/ID already in system, use different one |
| "Not a valid email" | Email must have @ and domain |
| "Password must contain..." | Add uppercase, lowercase, number, 6-16 chars |
| "Cannot activate tag" | Tag must be physically at facility, wait 5 min |
| "Cannot delete" | Select item first, try refreshing (F5) |
| "Page not found" | Check URL is correct, contact admin |

## Getting Help

### Quick Reference

- Keep this guide open in another browser tab
- Use Ctrl+F to search this document

### Full Documentation

- [README.md](README.md) — System overview
- [GETTING_STARTED.md](GETTING_STARTED.md) — Setup guide
- [VEHICLES.md](docs/VEHICLES.md) — Complete vehicles guide
- [PEOPLE.md](docs/PEOPLE.md) — Complete employee guide
- [MESSAGES.md](docs/MESSAGES.md) — Complete messaging guide
- [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md) — Problem solving

### Contact Support

1. Check this Quick Reference
2. Check full documentation for your feature
3. Try refreshing page (F5) and retrying
4. Contact your system administrator with:
   - Error message
   - What you were doing
   - Your browser type
   - Screenshots if helpful

## Tips & Tricks

### Pro Tips

✅ Select with checkbox header for all/none  
✅ Use Ctrl+F to find items in large tables  
✅ Write down passwords on paper for new employees  
✅ Check battery levels weekly  
✅ Deactivate messages instead of deleting if unsure  
✅ Use High priority sparingly so it stands out  
✅ Set message to Active immediately to ensure delivery  

### Avoid These Mistakes

❌ Don't delete unless you're certain (irreversible)
❌ Don't set all messages to High priority
❌ Don't share passwords via email
❌ Don't forget to activate new tags
❌ Don't rely on password resets (not available)
❌ Don't close portal during important work
❌ Don't ignore battery warnings

## Offline Capabilities

**Note:** Portal requires internet connection. Features that require connection:

- Logging in
- Viewing/adding data
- Sending messages
- Managing tags and employees

**What can't be done offline:**

- Cannot work without internet
- Cannot view or edit data
- Cannot send messages

**If internet goes out:**

- Wait for connection to restore
- Refresh page when back online
- Data is automatically saved on server

---

**Last Updated:** 2026
**Version:** 1.0
**For Help:** Contact your system administrator

---

[Back to Main README](../README.md)
