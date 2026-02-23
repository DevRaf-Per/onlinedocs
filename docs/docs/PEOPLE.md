# Employee Management Guide

This guide provides detailed instructions for managing employee accounts on the **Person Management** page.

## Overview

The **Person Management** page lets you create and manage user accounts for your sales team and other employees who use the mobile app. Each employee gets a unique User ID and password for accessing the system.

## Accessing the Person Management Page

1. Log in to the OWPG Admin Portal
2. Click **Person Management** in the left sidebar
3. You'll see a table with all employee accounts
4. Action buttons and the add employee form are below the table

## Understanding the Employees Table

The table displays the following information for each employee:

| Column | Description |
| --- | --- |
| **User ID** | Unique identifier generated for the employee (e.g., JD001) |
| **Email** | Employee's email address |
| **First** | Employee's first name |
| **Last** | Employee's last name |

### Table Features

- **Sorting**: Click column headers to sort by that field
- **Selection**: Use checkboxes to select employees for actions
- **Scrolling**: Scroll right if you can't see all columns
- **Search**: Use browser Find (Ctrl+F) to locate an employee

## Selecting Employees

To select one or more employees:

1. Check the box(es) next to the employee(s) you want to work with
2. Check the header box to select/deselect all employees
3. Selected rows are highlighted in blue
4. Action buttons appear based on your selection:
   - **View Details** (requires exactly 1 employee selected)
   - **Delete** (for any selected employees)

## Core Actions

### 1. Create a New Employee Account

Add a new employee to the system so they can use the mobile app.

**Requirements for valid account:**

- **Email**: Must be a valid email address (e.g., `john.doe@company.com`)
- **Password**: Must meet complexity requirements (see below)
- **First Name**: Cannot be blank
- **Last Name**: Cannot be blank

**Password Requirements:**

- At least 6 characters, no more than 16 characters
- Must include at least one number (0-9)
- Must include at least one uppercase letter (A-Z)
- Must include at least one lowercase letter (a-z)

**Example valid passwords:**

- `SecurePass1`
- `Emp123Pass`
- `WorkPw456`

**Example invalid passwords:**

- `Pass123` — too short (7 characters, but let's say it's rejected for other reasons)
- `password123` — no uppercase letter
- `PASSWORD123` — no lowercase letter
- `EmployeeP` — no number

**How to add an employee:**

1. Scroll to the **"Add New User"** form at the bottom
2. Fill in the required fields (marked with *):
   - Email address
   - Password (save this securely!)
   - First name
   - Last name
3. Click **Add new user** button
4. A confirmation dialog appears showing the details
5. Review the information, especially the User ID and password
6. Click **OK** to confirm

**After creation:**

- A unique **User ID** is automatically generated
- Write down both the User ID and temporary password
- Provide these credentials securely to the employee
- They will use these to log in to the mobile app
- Ask them to change their password after first login

**What information appears in the confirmation:**

```plaintext
About to add [First] [Last] with the user ID [USER_ID] and password [PASSWORD].
This is the ID and password they'll be using to sign in to the mobile app. 
Be sure to write down the password.
```

### 2. View Employee Details and Trip History

View detailed information about an employee's trip history and vehicle usage.

**How to:**

1. Select exactly one employee by clicking their checkbox
2. Click the **View Details** button
3. A panel opens showing:
   - Employee name
   - **Trip History** table with all trips they've taken

**Trip Information Displayed:**

| Column | Description |
| --- | --- |
| **Trip ID** | Unique identifier for the trip |
| **Vehicle Taken** | Description of the vehicle used |
| **Reason** | Purpose of the trip (delivery, inspection, etc.) |
| **Customer Name** | Client or customer name for that trip |
| **Start Time** | Date and time trip began (YYYY-MM-DD HH:MM:SS) |
| **End Time** | Date and time trip ended (YYYY-MM-DD HH:MM:SS) |
| **Trip File** | Reference to detailed GPS tracking data |

**Viewing Trip Route on Map:**

If trip mapping is available:

1. Click on one trip in the Trip History table
2. If available, a map will display showing:
   - The vehicle's route during that trip
   - Start and end points
   - All waypoints along the path
3. Use map zoom and pan controls to explore the route

**Common Uses:**

- Verify employee was at expected locations
- Monitor driving efficiency
- Audit trip information for billing/invoicing
- Track customer visits
- Investigate discrepancies in vehicle usage

### 3. Delete an Employee Account

Permanently remove an employee account from the system.

⚠️ **Warning**: Deleting is permanent. The employee will no longer be able to log in to the mobile app.

**When to delete:**

- When an employee leaves the company
- When an employee no longer needs system access
- When removing a test or demo account

**How to:**

1. Select one or more employees to delete
2. Click the **Delete** button (shown in red)
3. A confirmation dialog appears asking:
   - "Are you sure you want to delete these users? This action cannot be undone."
4. Click **Yes** to confirm or click outside to cancel
5. The employee account(s) are immediately removed

**Before deleting:**

- Ensure you have the correct employee selected
- Consider if you need to preserve their trip history
- Confirm the employee no longer needs access
- For security, remove access immediately if employee leaves

**What happens after deletion:**

- Employee can no longer log in to mobile app
- Trip history is preserved in the system
- Account cannot be recovered
- To re-enable, you must create a new account with new credentials

## Advanced Features

### Bulk Operations

You can delete multiple employee accounts at once:

1. Click the header checkbox to select all employees, or individually select specific employees
2. Click **Delete** button
3. Confirm the deletion for all selected employees

### Finding an Employee

**Using the table:**

1. Use browser Find feature:
   - Windows: Ctrl+F
   - Mac: Cmd+F
2. Search by name, email, or User ID
3. The table will highlight matching results

### Reviewing Trip History

Get insights into employee activity:

1. Click **Person Management** in sidebar
2. For each employee, click **View Details**
3. Review their trips:
   - Frequency of trips
   - Locations visited
   - Duration of trips
   - Vehicles used

## Common Tasks

### Task: Onboard a New Salesperson

1. **Create Account**: Use the "Add New User" form with their information
2. **Generate Credentials**: Note the User ID and temporary password
3. **Provide Access**: Securely share the credentials with the employee
4. **Train**: Show them how to log in and use the mobile app
5. **Verify**: Wait for them to take their first trip and confirm they can use the system

### Task: Audit Employee Activity

1. Go to **Person Management**
2. Select the employee(s) to audit
3. Click **View Details**
4. Review their trip history:
   - What vehicles did they use?
   - Where did they go?
   - How long were the trips?
   - Who were the customers?
5. Export or print data as needed (Ctrl+P)

### Task: Offboard Departing Employee

1. **Immediate Action**: Delete their account to prevent login
2. **Preserve Records**: Before deleting, optionally export/screenshot trip data
3. **Communicate**: Inform them their access is revoked
4. **Verify**: Confirm they're locked out of the system
5. **Records**: Keep trip history for compliance/audit

### Task: Verify Employee Location

1. Go to **Person Management**
2. Find and select the employee
3. Click **View Details**
4. Find recent trips
5. Click on a trip to view the route map
6. Check if route matches expected customer locations

### Task: Generate Employee Report

1. Select the employee(s) to include
2. Click **View Details**
3. Use browser Print (Ctrl+P) to save/print the trip information
4. Select "Save as PDF" option for archiving

## Password Management

### Employee Changes Password

Employees change their password within the mobile app. Admin password reset is not available in this interface — employees must use the app's password reset feature.

### Initial Password Requirements

When you create an account, ensure the password meets all requirements:

- ✅ At least 6 characters
- ✅ At most 16 characters
- ✅ At least one number
- ✅ At least one uppercase letter
- ✅ At least one lowercase letter

### Sharing Passwords Securely

- ❌ **Never** email passwords in plain text
- ✅ **Do** write it on paper and hand to employee in person
- ✅ **Do** read it aloud and have employee verify
- ✅ **Do** have employee immediately change it after first login

## Data & Privacy

### What Data is Stored

- Employee name, email, User ID
- All trip history and locations
- Vehicle usage records
- Timestamps of all activity

### Data Retention

- **Account information**: Stored permanently until deleted
- **Trip data**: Retained for operational and audit purposes
- **Login history**: Tracked for security

### Privacy Considerations

- Employees can see their own trip data in the mobile app
- Managers can audit any employee's trips through this system
- Trip data includes precise locations and times
- Comply with employment laws regarding employee monitoring

## Troubleshooting

### "This user already exists"

**What it means:** An account with that User ID or email already exists in the system.

**Solution:**

1. Check if the employee already has an account
2. If it's an old account they no longer use, delete it first
3. Use a different email address if the person has multiple accounts

### "Email cannot be left blank"

**What it means:** Email field is empty.

**Solution:** Enter a valid email address (must contain @ symbol)

### "Password must contain..." (various requirements)

**What it means:** Your password doesn't meet complexity requirements.

**Solution:** Ensure password has:

- At least 6 characters
- At most 16 characters
- At least one number
- At least one uppercase letter
- At least one lowercase letter

### Employee Says They Can't Log In

**Possible causes:**

1. **Wrong credentials**: Verify User ID and password (case-sensitive)
2. **Needs password reset**: Employee must use password reset in mobile app
3. **Account deleted**: Check if account still exists in table
4. **Server issue**: Try again in a few minutes

**What you can do:**

- Confirm the account appears in the employees table
- Have employee attempt login 2-3 more times
- Suggest they check caps lock is off
- As last resort, delete account and create new one with new credentials

### Can't Find View Details Button

**What it means:** You need to select exactly one employee for View Details to appear.

**Solution:**

1. Uncheck all other checkboxes
2. Check only one employee
3. The View Details button should now be visible

### Trip Data Shows No Information

**Possible causes:**

1. Employee hasn't taken any trips yet
2. Trip data hasn't synced to the system
3. Trip data was purged for data retention

**Solution:**

1. Wait 24 hours after employee's first trip for data to sync
2. Try again later
3. Contact your administrator if data is missing

## Related Documentation

- [Getting Started Guide](../../GETTING_STARTED.md) — First-time setup
- [Vehicle Management](VEHICLES.md) — Managing BLE tags and vehicles
- [Main README](../../README.md) — System overview

---

For additional help, contact your system administrator.
