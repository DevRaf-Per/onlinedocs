# Troubleshooting Guide

This guide helps you resolve common issues in the OWPG Admin Portal.

## General Issues

### Can't Access the Portal

**Error**: Browser shows "Page not found" or "Connection refused"

**Solutions**:

1. **Check URL**: Verify you're using the correct portal URL
   - Ask your administrator for the exact URL
   - Check if URL is bookmarked correctly

2. **Check Internet Connection**:
   - Try opening another website to test connectivity
   - If internet is down, wait for connection to restore
   - Try from a different network if available

3. **Firewall/Network Issues**:
   - Your organization may block the portal
   - Contact your IT department
   - Try accessing from a different network (personal hot-spot, home)

4. **Browser Cache**:
   - Clear browser cache (Ctrl+Shift+Delete on Windows)
   - Try a different browser
   - Try "private" or "incognito" mode

### Page Loads Slowly

**Issue**: Portal takes a long time to open pages or tables

**Solutions**:

1. **Refresh the page**:
   - Press F5 or Ctrl+R
   - Wait 10-15 seconds for it to fully load

2. **Clear cache**:
   - Windows: Ctrl+Shift+Delete
   - Mac: Cmd+Shift+Delete
   - Select "All time" and clear

3. **Close other tabs**:
   - Having many browser tabs open slows everything
   - Close unnecessary tabs and try again

4. **Check internet speed**:
   - Run a speed test at speedtest.net
   - If slow, try later or change networks

5. **Try different browser**:
   - Chrome, Firefox, Safari, and Edge all work
   - If slow in one, try another

### Page Looks Wrong (Formatting Issues)

**Issue**: Text is misaligned, buttons are in wrong place, colors are off

**Solutions**:

1. **Refresh and clear cache**:
   - Ctrl+Shift+Delete (Windows) or Cmd+Shift+Delete (Mac)
   - Select "All time"
   - Click "Clear data"
   - Refresh the page (F5)

2. **Try a different browser**: The portal works best with:
   - Google Chrome
   - Mozilla Firefox
   - Microsoft Edge
   - Apple Safari

3. **Check browser zoom**:
   - If zoom is very high/low, page formatting breaks
   - Set zoom to 100% (Ctrl+0 on Windows, Cmd+0 on Mac)

4. **Update your browser**:
   - Old browser versions have compatibility issues
   - Go to browser settings and update

---

## Login Issues

### Can't Log In - "Invalid Credentials"

**Error**: After entering username/password, error says credentials are wrong

**Solutions**:

1. **Verify username and password**:
   - Username is case-sensitive
   - Password is case-sensitive
   - Check for extra spaces before/after text
   - Ensure CAPS LOCK is off

2. **Forgot your password?**:
   - The portal doesn't have a "forgot password" button
   - Contact your administrator to reset
   - They may need to create a new account for you

3. **Account locked?**:
   - After multiple failed login attempts, account may lock
   - Wait 15 minutes and try again
   - Or contact administrator to unlock

4. **Check login spelling**:
   - Example correct format: `john.doe` or `jdoe`
   - Confirm format with your administrator
   - User ID (like `JD001`) is NOT the login username

### Session Expired - "Please Log In Again"

**Error**: After being logged in, portal redirects you to login page

**Solutions**:

1. **Normal behavior**:
   - Sessions expire for security (usually after 1-2 hours of inactivity)
   - Just log in again — this is normal

2. **If it keeps happening frequently**:
   - You might have opened multiple tabs/windows
   - Try logging out completely: Sign Out button in sidebar
   - Close the browser entirely
   - Reopen browser and log in once

3. **Clear cookies**:
   - Ctrl+Shift+Delete (Windows) or Cmd+Shift+Delete (Mac)
   - Select "Cookies and other site data"
   - Try logging in again

---

## Vehicle (Vehicles Page) Issues

### "Cannot activate this tag because it is not on the premises"

**Error**: When trying to activate a tag, system says it's not on the premises

**Solutions**:

1. **Physical tag location**:
   - Ensure the BLE tag is physically at your facility location
   - The tag may need to power on and communicate location
   - Wait 5-10 minutes for the tag to report location

2. **Location mismatch**:
   - Check if tag location matches your facility
   - Tags created with different location codes can't be activated at your location
   - Contact administrator if location is incorrect

3. **Try again later**:
   - Give the tag more time to sync its location
   - Try again in 15 minutes
   - If it still fails, tag might be offline or broken

### Tag Battery Won't Update

**Issue**: Battery life shows "—" or old percentage that hasn't changed

**Solutions**:

1. **Wait for sync**:
   - Battery data syncs every 24 hours
   - If you just activated the tag, wait a full day
   - Check back tomorrow

2. **Tag connectivity**:
   - Ensure tag has power
   - Ensure tag can communicate with system
   - Try moving tag to a different location with better signal
   - If problem persists, replace the tag

3. **Refresh page**:
   - Press F5 to refresh
   - Close and reopen the Vehicles page

### Can't Delete a Tag

**Error**: Delete button doesn't work or shows error

**Solutions**:

1. **Select exactly what you want to delete**:
   - Uncheck all boxes except the tag you want to delete
   - Click Delete button
   - Confirm in dialog

2. **Refresh and try again**:
   - Refresh page (F5)
   - Try selecting and deleting again

3. **Contact administrator**:
   - If button is completely missing or grayed out
   - You might not have permission to delete
   - Ask administrator for help

### Can't Find a Specific Tag

**Issue**: You know the tag exists but can't find it in the table

**Solutions**:

1. **Use browser Find**:
   - Ctrl+F (Windows) or Cmd+F (Mac)
   - Search for the Tag ID
   - Press Enter to find it

2. **Scroll the table**:
   - Table might be wide, scroll right to see all columns
   - Table might have many rows, scroll down to find your tag

3. **Check if it's deleted**:
   - If you deleted it recently, it won't appear
   - Deletion is permanent

4. **Check status**:
   - Is it ACTIVE or INACTIVE?
   - Might be at bottom of table after inactive tags

---

## Employee (Person Management) Issues

### "This user already exists"

**Error**: When trying to create new employee, system says user already exists

**Solutions**:

1. **Check if account already exists**:
   - Look in the table for that employee
   - If they're already there, you don't need to create them again

2. **Use different email**:
   - The system checks both User ID and email
   - If using same name/email, system thinks it's a duplicate
   - Use a different email address if you want to create again

3. **Delete old account first**:
   - If old account is no longer needed
   - Select the old employee in table
   - Click Delete to remove them
   - Then create the new account

### Email Validation Error

**Error**: "Not a valid email address"

**Solutions**:

1. **Email format**:
   - Email must have @ symbol: `john.doe@company.com`
   - Cannot have spaces: `john doe@company.com` ❌
   - Should be lowercase: `john.doe@company.com` ✅

2. **Examples of valid emails**:
   - <john.doe@company.com> ✅
   - <j.smith@domain.co.uk> ✅
   - <mary_johnson@email.org> ✅

3. **Examples of invalid emails**:
   - john.doe (no @ or domain) ❌
   - @company.com (no name part) ❌
   - john <doe@company.com> (space) ❌
   - <john.doe@.com> (missing domain) ❌

### Password Requirements Error

**Error**: "Password must contain..." with various requirements

**Solutions**:

Password must meet ALL requirements:

- **6-16 characters**: Count the letters and numbers
  - Too short: `Pwd1` ❌
  - Good: `SecurePass1` ✅
  - Too long: `ThisIsAVeryLongPasswordThatIsTooLong1` ❌

- **At least one number (0-9)**:
  - Bad: `SecurePass` (no number) ❌
  - Good: `SecurePass1` ✅

- **At least one uppercase letter (A-Z)**:
  - Bad: `securepass1` (all lowercase) ❌
  - Good: `SecurePass1` ✅

- **At least one lowercase letter (a-z)**:
  - Bad: `SECUREPASS1` (all uppercase) ❌
  - Good: `SecurePass1` ✅

**Valid password examples**:

- `Employee1` ✅ 9 letters, has number, has upper/lower
- `WorkPass2023` ✅ 12 letters, has number, has upper/lower
- `Admin123` ✅ 8 letters, has number, has upper/lower

### Employee Trip Data Won't Load

**Issue**: Click View Details but trip table is empty or shows no data

**Solutions**:

1. **Wait for data to sync**:
   - If employee just created their account
   - They need to take at least one trip first
   - Data syncs every 24 hours
   - Check back tomorrow

2. **Refresh the page**:
   - Close the Details panel
   - Go back to main Vehicles page
   - Return to Person Management
   - Try View Details again

3. **Employee hasn't taken trips yet**:
   - New employee accounts won't have trip data
   - They need to use the mobile app to record trips
   - Check back after they've taken a few trips

### Can't Find Employee in Table

**Issue**: You know employee exists but can't see them in the table

**Solutions**:

1. **Use browser Find**:
   - Ctrl+F (Windows) or Cmd+F (Mac)
   - Search by name or email
   - Press Enter to locate

2. **Scroll the table**:
   - There may be many employees
   - Scroll down to find yours
   - Table might be wide, scroll right to see more columns

3. **Refresh the page**:
   - Press F5 to reload employee list
   - Maybe they were just added

4. **Check if deleted**:
   - If you deleted an employee recently
   - They won't appear in table
   - Deletion is permanent

---

## Message (Messaging Management) Issues

### Can't Send a Message

**Error**: Send button doesn't work or message won't appear

**Solutions**:

1. **Check message content**:
   - Message field cannot be blank
   - Type something in the message box
   - Try again

2. **Select priority level**:
   - You must select a priority (High, Medium, or Low)
   - If dropdown shows "—", select an actual priority
   - Then try sending

3. **Refresh and try again**:
   - Press F5 to refresh the page
   - Fill out form again
   - Click Send

### Message Priority Won't Change

**Issue**: Clicking the Priority cell doesn't let you edit

**Solutions**:

1. **Try double-clicking the cell**:
   - Single click should open a dropdown
   - If not, double-click the Priority cell

2. **Refresh page**:
   - Press F5
   - Try clicking the cell again

3. **Select from dropdown**:
   - When Priority cell is active
   - A dropdown appears with options
   - Click the option you want
   - Click elsewhere to confirm

### Message Active Status Won't Toggle

**Issue**: Clicking Active checkbox doesn't change it

**Solutions**:

1. **Check that it's actually changing**:
   - Sometimes the change is instant but not obvious
   - Look for any visual change (checkbox appearance)
   - Refresh page (F5) to confirm

2. **Try clicking directly on checkbox**:
   - Not just the row, but the checkbox itself
   - The checkbox should toggle

3. **Refresh and try again**:
   - Press F5
   - Try clicking the checkbox again

### Can't Delete a Message

**Error**: Delete button doesn't work or shows error

**Solutions**:

1. **Select the message(s)**:
   - Check the box(es) next to the message(s) to delete
   - Confirm at least one is selected
   - Click Delete button

2. **Confirm deletion**:
   - Dialog appears asking you to confirm
   - Click "Yes" to confirm
   - Click outside to cancel

3. **Refresh and try again**:
   - Press F5 to refresh
   - Try selecting and deleting again

### Employees Didn't See My Message

**Issue**: You sent a message but employees say they didn't see it

**Solutions**:

1. **Check if message is Active**:
   - Look in the table
   - If Active checkbox is unchecked, employees can't see it
   - Check the box to make it visible

2. **Activate the message**:
   - If Active is unchecked, click checkbox to check it
   - Message now appears to employees
   - May take a few minutes to sync to mobile apps

3. **Verify message exists**:
   - Can you see it in the table?
   - If not, it may have been deleted
   - Create a new message

4. **Check employee app version**:
   - They might have an old version of mobile app
   - Ask them to update the app
   - Then try viewing message again

---

## Data & Display Issues

### Table Shows Wrong or Missing Data

**Issue**: Table displays outdated information or items are missing

**Solutions**:

1. **Refresh the page**:
   - Press F5 to refresh
   - This loads the latest data from server
   - Wait 5 seconds for table to fully load

2. **Clear browser cache**:
   - Ctrl+Shift+Delete (Windows)
   - Cmd+Shift+Delete (Mac)
   - Select "All time" and clear

3. **Close other browser tabs**:
   - Having many tabs open causes stale data
   - Close other tabs
   - Refresh and check again

4. **Try a different browser**:
   - Chrome, Firefox, Safari, Edge all work
   - If one browser shows wrong data, try another

### Dates/Times Display Incorrectly

**Issue**: Dates show wrong format or time is incorrect

**Solutions**:

1. **Check system time**:
   - Portal uses your computer's time
   - Ensure your computer time is correct
   - Set correct timezone

2. **Correct format is YYYY-MM-DD HH:MM:SS**:
   - Year-Month-Day Hour:Minute:Second
   - Example: `2024-03-15 14:30:00` is March 15, 2024 at 2:30 PM
   - Not `03/15/2024` or `15-03-2024`

3. **24-hour time format**:
   - Time shows in 24-hour format
   - 1:00 PM = 13:00
   - 6:30 PM = 18:30
   - Midnight = 00:00
   - Noon = 12:00

---

## When to Contact Your Administrator

Contact your system administrator if:

- You still can't log in after trying all solutions
- Portal is completely down or not responding
- You see database errors or system errors
- You need password reset
- You're locked out of your account
- You don't have permission to perform an action
- Data appears to be missing or corrupted
- You need new features or changes
- There are recurring technical problems

**Information to provide administrator:**

- Exact error message you see
- What you were trying to do
- Your username/email
- Browser you're using
- Your operating system (Windows, Mac, etc.)
- Screenshots if helpful

---

## Browser Compatibility

The OWPG Admin Portal works best with:

| Browser | Version | Status |
| --- | --- | --- |
| Google Chrome | Latest | ✅ Fully supported |
| Mozilla Firefox | Latest | ✅ Fully supported |
| Microsoft Edge | Latest | ✅ Fully supported |
| Apple Safari | Latest | ✅ Fully supported |

**Older versions** (2+ years old) may have issues.
**Update your browser** regularly for best performance.

---

## Quick Checklist

Before contacting support, try these:

- [ ] Refresh page (F5)
- [ ] Clear browser cache (Ctrl+Shift+Delete)
- [ ] Try a different browser
- [ ] Check your internet connection
- [ ] Log out and log back in
- [ ] Restart your computer
- [ ] Try again in 5 minutes
- [ ] Reread the error message carefully

---

## Related Documentation

- [Getting Started Guide](../../GETTING_STARTED.md) — First-time setup
- [Vehicle Management](VEHICLES.md) — Vehicles guide
- [Employee Management](PEOPLE.md) — Employees guide
- [Message Management](MESSAGES.md) — Messages guide
- [Main README](../../README.md) — System overview

---

For additional help, contact your system administrator with the information listed above.
