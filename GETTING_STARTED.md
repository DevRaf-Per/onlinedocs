# Getting Started with OWPG Admin Portal

This guide will walk you through the initial setup and first steps of using the OWPG Admin Portal.

## System Requirements

- Modern web browser (Chrome, Firefox, Safari, or Edge)
- Internet connection
- Administrator login credentials

## First Login

### Step 1: Access the Portal

1. Open your web browser
2. Navigate to the OWPG Admin Portal URL (provided by your administrator)
3. You should see the login page with the OWPG logo

### Step 2: Enter Your Credentials

1. **Username**: Enter the username provided to you
2. **Password**: Enter the password provided to you
3. Click the **Login** button

### Step 3: Successfully Logged In

Once logged in successfully, you'll see:

- The OWPG logo in the top left
- A welcome message at the center
- The main navigation in the left sidebar
- A **Sign Out** button in the sidebar (top right)

## Your First Actions

### Common First Tasks

#### 1. Add a New Vehicle Tag

- Click **Vehicles** in the sidebar
- Scroll to "Add a New Tag" section
- Enter the Tag ID and vehicle description
- Click **Add Tag**

#### 2. Create a New Employee Account

- Click **Person Management** in the sidebar
- Scroll to "Add New User" form
- Fill in email, password, first name, and last name
- Click **Add new user**
- **Important**: Write down the password — you'll need to provide it to the employee

#### 3. Send a Message to Your Team

- Click **Messaging Management** in the sidebar
- Scroll to "Write a New Message" section
- Type your message, select priority level
- Check "Should this message be active right away?" if needed
- Click **Send**

## Understanding the Dashboard

### Home Page

The home page shows:

- **Welcome message** with OWPG branding
- **Key features** available in the system
- **Documentation links** for each feature

### Sidebar Navigation

The left sidebar provides access to:

| Page | Purpose |
| --- | --- |
| Home | Overview and documentation |
| Vehicles | Manage BLE tags and fleet vehicles |
| Messaging Management | Send and manage team messages |
| Person Management | Create and manage employee accounts |

### Sign Out

Always click **Sign Out** in the sidebar when you're done. This keeps your account secure.

## Common Workflows

### Workflow 1: Onboarding a New Employee

1. **Create Account**
   - Go to **Person Management**
   - Fill out the "Add New User" form
   - Click **Add new user**
   - Note the generated User ID and password

2. **Provide Credentials**
   - Write down the User ID and temporary password
   - Share with the employee securely
   - Instruct them to change password in the mobile app

3. **Verify Account**
   - View the employee in the table
   - Confirm their information displays correctly

### Workflow 2: Adding a Vehicle to Your Fleet

1. **Register the Tag**
   - Go to **Vehicles**
   - Find "Add a New Tag" form
   - Enter: Tag ID and vehicle description
   - Click **Add Tag**

2. **Activate the Tag**
   - Tag appears in the table with "INACTIVE" status
   - Select the tag with the checkbox
   - Click **Activate** button
   - Confirm activation in the dialog

3. **Monitor the Tag**
   - Check battery life percentage
   - View test drive history by clicking **View Details**

### Workflow 3: Broadcasting a Message

1. **Compose Message**
   - Go to **Messaging Management**
   - Type your message (max 255 characters recommended)
   - Select priority: High, Medium, or Low

2. **Activate Message**
   - Check "Should this message be active right away?"
   - Click **Send**

3. **Manage Message**
   - View all messages in the table
   - Toggle Active status (on/off)
   - Edit priority level
   - Delete when no longer needed

## Important Tips

### ✅ Best Practices

- **Save Important Information**: Write down employee User IDs and initial passwords
- **Battery Monitoring**: Check battery life percentage on vehicle tags regularly
- **Message Priority**: Use "High" for urgent messages, "Low" for informational updates
- **Confirmation Dialogs**: Always review before confirming deletions or major changes
- **Regular Logouts**: Always sign out when finished, especially on shared computers

### ⚠️ Before You Delete

**Deleting is permanent.** Before you delete:

- Verify you have the correct item selected
- Consider if you need the data for records (especially for employees and vehicles)
- For employees, confirm they no longer need system access

### 🔒 Security Tips

- **Never share passwords** via email or chat
- **Change temporary passwords** immediately upon employee request
- **Sign out** when leaving your workstation
- **Report suspicious activity** to your administrator
- **Don't use the same password** for multiple accounts

## Understanding Common Terms

| Term | Definition |
| --- | --- |
| **Tag** | GPS device attached to a vehicle for tracking |
| **Tag ID / DMAC** | Unique identifier for each BLE tag |
| **Status** | Whether a tag is ACTIVE (in use) or INACTIVE (not in use) |
| **Battery Life** | Percentage of remaining battery on the BLE tag |
| **User ID** | Unique identifier for an employee account |
| **Trip** | Record of a vehicle's journey with start time, end time, and route |
| **Message Priority** | Importance level: High, Medium, or Low |

## Working with Tables

### Selecting Rows

Most tables have checkboxes on the left. To select:

- Click individual checkboxes to select specific rows
- Click the checkbox in the header to select/deselect all rows
- Selected rows are highlighted with a blue background

### Viewing Table Data

- **Scroll horizontally** if the table is wider than your screen
- **Column headers** show what data each column contains
- **Status indicators** may use color (e.g., battery life uses red/orange/yellow/green)

### Common Table Actions

1. **View Details**: Select one row and click "View Details"
2. **Edit**: Click directly on editable cells (messages table only)
3. **Activate/Deactivate**: Select rows and click appropriate button
4. **Delete**: Select rows and click "Delete" button

## Troubleshooting

### Can't Login

1. Check that you entered your **username** correctly (case-sensitive)
2. Verify you entered your **password** correctly
3. Ensure CAPS LOCK is off
4. Contact your administrator if you've forgotten your credentials

### Can't Find a Feature

1. Check the **sidebar navigation** on the left
2. Review the **home page** for documentation links
3. Look for form sections at the bottom of pages (add new items)

### Page Loads Slowly

1. Refresh the page using F5 or Ctrl+R
2. Clear your browser cache
3. Try a different browser
4. Check your internet connection

### Lost Your Work

- **Tables**: Changes are saved automatically when you edit
- **Forms**: Use the form buttons to submit (data is not saved until you click the action button)
- **No automatic save** on unsaved forms — always click the submit button

For additional help, see the [Troubleshooting Guide](docs/TROUBLESHOOTING.md).

## Next Steps

Now that you're set up, check out the detailed guides:

- [Vehicle Management Guide](docs/VEHICLES.md) — Learn all vehicle tag features
- [Employee Management Guide](docs/PEOPLE.md) — Complete employee management reference
- [Message Management Guide](docs/MESSAGES.md) — Full messaging system walkthrough

Happy administrating! 🚀
