# Application Flow & Navigation Guide

Visual guide to understanding how the OWPG Inventory Application flows and navigates between screens.

## Application Navigation Flow

```
START
  ↓
[IP Lookup Page]
  ├─ User enters server IP address
  └─ Click "Connect"
      ↓
[Sign In Page]
  ├─ User enters username and password
  └─ Click "Sign In"
      ↓
[Main Page - Vehicle Checkout]
  ├─ Select action (Test Drive, Maintenance, etc.)
  ├─ Fill in action-specific form fields
  ├─ Scan or enter vehicle barcode
  ├─ Complete required information
  └─ Click "Submit"
      ↓
  ┌─ Success ─────────────────────┐
  │ Form clears, ready for next   │
  │ checkout or can view messages  │
  └───────────────────────────────┘
```

---

## Page Overview

### 1. IP Lookup Page

**When You See It:** First time app is opened, or server not configured

**Purpose:** Configure the MQTT server address

**What's On It:**
```
┌──────────────────────────────────────┐
│  Server Configuration                │
│  Enter Server IP Address:            │
│  [___________________________]        │
│              [Connect]               │
└──────────────────────────────────────┘
```

**What You Do:**
1. Enter IP address (e.g., 192.168.1.100)
2. Click Connect
3. Wait 5-10 seconds
4. App moves to Sign In page

**Next:** Sign In Page

---

### 2. Sign In Page

**When You See It:** After server configuration, or after signing out

**Purpose:** Authenticate your account

**What's On It:**
```
┌────────────────────────────────────┐
│         OWPG Sign In              │
├────────────────────────────────────┤
│  Username:                         │
│  [_________________________]       │
│                                    │
│  Password:                         │
│  [_________________________]       │
│                                    │
│  ☐ Remember me                    │
│                                    │
│         [Sign In]                  │
└────────────────────────────────────┘
```

**What You Do:**
1. Enter username
2. Enter password
3. (Optional) Check "Remember me"
4. Click Sign In
5. Wait 5-10 seconds for authentication
6. App moves to Main Page

**Next:** Main Page

---

### 3. Main Page (Vehicle Checkout)

**When You See It:** After successful sign-in

**Purpose:** Perform vehicle checkouts (test drives, maintenance, etc.)

**Layout:**
```
┌─────────────────────────────────────┐
│  [OWPG Logo]    Vehicle Checkout    │
├─────────────────────────────────────┤
│                                     │
│  Select Reason For This Check Out:  │
│  [▼ Test Drive ____________________] │
│                                     │
│  Vehicle Beacon ID:                 │
│  [________________] [Camera Icon]   │
│                                     │
│  Customer Name:                     │
│  [________________] [* Edit Button]  │
│                                     │
│  Phone Number:                      │
│  [________________________________] │
│                                     │
│  Number of People: [+] 1 [-]       │
│                                     │
│  ☐ Valid Driver's License          │
│  ☐ Insurance Information           │
│  ☐ Picture/Video Access           │
│                                     │
│           [Submit]                  │
│                                     │
├─────────────────────────────────────┤
│  [Messages] [Settings] [Sign Out]   │
└─────────────────────────────────────┘
```

**Form Sections (varies by action selected):**

**Test Drive Form:**
- Action Selection
- Customer Name (editable)
- Phone Number
- Number of People
- Driver's License checkbox
- Insurance Information checkbox
- Picture/Video Access checkbox
- Vehicle Beacon ID (barcode)
- Submit button

**Maintenance Form:**
- Action Selection
- Service Type
- Duration
- Notes/Description
- Vehicle Beacon ID
- Submit button

**Relocation Form:**
- Action Selection
- From Location
- To Location
- Notes
- Vehicle Beacon ID
- Submit button

**Transfer Form:**
- Action Selection
- From Department/Person
- To Department/Person
- Reason
- Vehicle Beacon ID
- Submit button

**Service Test Form:**
- Action Selection
- Test Type
- Results
- Vehicle Beacon ID
- Submit button

**Other Form:**
- Action Selection
- Description
- Notes
- Vehicle Beacon ID
- Submit button

**Main Actions:**
1. Select action from dropdown
2. Fill in required fields
3. Scan or type vehicle barcode
4. Complete form
5. Click Submit
6. See success message
7. Form resets for next checkout

**Bottom Menu:**
- Messages (view history)
- Settings (app configuration)
- Sign Out (logout)

**Next:**
- Submit → Success message → Form resets
- Messages → Message history view
- Settings → App settings
- Sign Out → Sign In page

---

## Modal Windows (Popups)

### Edit Customer Name Modal

```
┌─────────────────────────────────────┐
│  Edit Customer Name                 │
├─────────────────────────────────────┤
│  First Name:                        │
│  [_____________________________]    │
│                                     │
│  Last Name:                         │
│  [_____________________________]    │
│                                     │
│  Or Search Existing Customers:      │
│  [_____________________________]    │
│  □ John Smith                       │
│  □ Jane Doe                         │
│  □ Bob Johnson                      │
│                                     │
│        [Save]      [Cancel]         │
└─────────────────────────────────────┘
```

### Camera Scanner Modal

```
┌─────────────────────────────────────┐
│  Barcode Scanner                    │
├─────────────────────────────────────┤
│                                     │
│  [      Live Camera Feed     ]      │
│  [                          ]      │
│  [      [Yellow Frame      ]       │
│  [       when barcode      ]       │
│  [      is detected]        ]      │
│  [                          ]      │
│                                     │
│  Detected: ███████████████          │
│                                     │
│        [Back]              [X]      │
└─────────────────────────────────────┘
```

### Photo Capture Modal

```
┌─────────────────────────────────────┐
│  Capture Vehicle Photo              │
├─────────────────────────────────────┤
│                                     │
│  [      Live Camera Preview   ]     │
│  [        (Portrait View)     ]     │
│  [                            ]     │
│  [                            ]     │
│  [                            ]     │
│                                     │
│  Caption: [____________________]   │
│                                     │
│  [Take Photo]  [Done]  [Delete]    │
│                                     │
│  Photos Captured: [####__]         │
│  1 of 4 photos                      │
└─────────────────────────────────────┘
```

### Success Modal

```
┌──────────────────────────────────────┐
│  ✓ Success                           │
├──────────────────────────────────────┤
│                                      │
│  Test Drive Checkout Successful      │
│                                      │
│  Vehicle: ABC123456789               │
│  Customer: John Smith                │
│  Time: 2026-02-25 14:30              │
│  Transaction ID: TXN-20260225-0001  │
│                                      │
│  Location tracking: Enabled          │
│  Photos: 4 captured                  │
│                                      │
│           [OK]                       │
│                                      │
└──────────────────────────────────────┘
```

### Error Modal

```
┌──────────────────────────────────────┐
│  ✗ Error                             │
├──────────────────────────────────────┤
│                                      │
│  Could not submit checkout           │
│                                      │
│  Error: Connection timeout           │
│                                      │
│  Please check:                       │
│  • Internet connection               │
│  • All required fields filled        │
│  • Try again in 10 seconds          │
│                                      │
│           [Retry]      [Cancel]      │
│                                      │
└──────────────────────────────────────┘
```

---

## Screen Transitions

### Happy Path (Successful Checkout)

```
IP Lookup → Sign In → Main Page → Fill Form → Submit
                                      ↓
                              Success Message
                                      ↓
                              Form Resets (Main Page)
```

### Message History Path

```
Main Page → Click Messages → Message List View
                                      ↓
                              Tap Message
                                      ↓
                              Message Details
                                      ↓
                              Back to Main Page
```

### Sign Out Path

```
Main Page → Click Sign Out → Confirm Dialog
                                    ↓
                              Sign In Page
```

### Error Path

```
Form → Submit → Error Message → Retry Options
                                    ↓
                        (Retry) → Submit Again
                            or
                        (Cancel) → Form Retained
```

---

## Feature Access Map

```
MAIN PAGE
├─ Vehicle Checkout (Primary Feature)
│  ├─ Action Selection Dropdown
│  ├─ Customer Info Management (edit/add)
│  ├─ Camera Scanner (barcode)
│  ├─ Manual Entry Fields
│  ├─ Photo Capture
│  └─ Form Submission
│
├─ Messages Button
│  ├─ Checkout History
│  ├─ Message Details
│  └─ Location History
│
├─ Settings (if available)
│  ├─ App Preferences
│  ├─ Permission Management
│  ├─ Server Configuration
│  └─ About App
│
└─ Sign Out Button
   ├─ Confirm Dialog
   └─ Return to Sign In
```

---

## Data Flow Through App

```
User Input → Form Fields → Validation → Local Storage → Submission
                                              ↓
                                        MQTT Server
                                              ↓
                                    Company Database
                                              ↓
                                        Location Tracking
                                        Photo Storage
                                        Message Logging
```

---

## Permission Requests Timeline

```
APP LAUNCH
├─ Camera Permission (immediately or on first scan)
├─ Location Permission (on first checkout or on app start)
├─ Storage Permission (on first photo attempt)
└─ Network Permission (on first data submission)
```

**Can happen at any time during use when feature accessed.**

---

## State Management

### Form States

**State: Empty**
- No fields filled
- Submit button available but may be disabled
- Edit buttons show "required" indicator

**State: Partial**
- Some required fields filled
- Some optional fields empty
- Submit button may be disabled if required fields missing

**State: Complete**
- All required fields filled
- Ready to submit
- Submit button enabled and highlighted

**State: Submitted**
- Form locked (read-only)
- Loading indicator shown
- Cannot make changes

**State: Success**
- Form clears
- Success message shown
- Returns to empty state

**State: Error**
- Form retained with user data
- Error message shown
- User can correct and retry

### Authentication States

```
NOT SIGNED IN → SIGNING IN → SIGNED IN → SIGNING OUT → NOT SIGNED IN
  (IP Lookup)   (loading)   (Main Page)  (logging out)  (Sign In Page)
     ↓
   ERROR
     ↓
 (Back to IP Lookup)
```

### Location Tracking States

```
START → REQUEST PERMISSION → ENABLED → TRACKING → STOP (or app close)
                                            ↓
                                    Background Service
                                    (if Always Allow)
```

---

## Navigation Shortcuts

### Quick Actions from Main Page

| Action | Button/Menu | Result |
|--------|------------|--------|
| New Checkout | Form fields | Create new checkout |
| View History | Messages button | See past checkouts |
| Re-scan Same Barcode | Copy from history | Faster next checkout |
| Switch User | Sign Out | Go to Sign In page |
| Change Server | Settings | Go to IP Lookup |
| Enable Camera | Permission dialog | Allow barcode scanning |
| Enable Location | Permission dialog | Allow GPS tracking |

---

## Accessibility Features

### For Users with Different Needs

**Vision:**
- Large text option (if available)
- High contrast mode (dark theme default)
- Screen reader compatible (standard)

**Motor:**
- Large touch targets
- Pinch to zoom support
- Keyboard navigation (on some platforms)

**Hearing:**
- Visual indicators for alerts
- Vibration feedback (if enabled)
- No required audio notifications

**Cognitive:**
- Clear language and instructions
- Consistent layout
- Minimal steps to complete tasks

---

## Performance Considerations

### Typical Screen Load Times

| Screen | Load Time | What It's Doing |
|--------|-----------|-----------------|
| IP Lookup | <1 second | Displaying form |
| Sign In | <1 second | Displaying form |
| Main Page | 1-2 seconds | Loading customer list, initializing location |
| Camera Scanner | 1-3 seconds | Initializing camera hardware |
| Message History | 2-5 seconds | Loading from local database |
| Submit Checkout | 5-15 seconds | Sending to server, receiving confirmation |

### Battery & Data Usage

**Location Tracking:**
- ~5-10% battery per 8 hours
- ~1-5 MB data per day (with hourly updates)

**Camera Scanning:**
- ~2-5% battery per 100 scans
- No data usage

**General App Use:**
- ~1-2% battery per hour
- ~1-10 MB data per hour (depends on activity)

---

## Customization Options (for Administrators)

Different organizations may customize:

- **Color scheme** (theme)
- **Logo and branding**
- **Available actions** (which checkout types)
- **Required fields** (what must be filled)
- **Permissions required** (camera, location)
- **Data retention** (how long records kept)
- **Server address** (where data goes)

**Users should check with their administrator for organization-specific customizations.**

---

## Common Workflows

### Standard Test Drive

```
1. Open app
2. See Main Page (already signed in)
3. Select "Test Drive" action
4. Edit/add customer name
5. Enter phone number
6. Set number of people
7. Check required boxes
8. Scan vehicle barcode (or type)
9. Take photos of vehicle
10. Click Submit
11. See success message
12. Form resets, ready for next
```

### Handling a Checkout Error

```
1. Fill form and click Submit
2. See error message
3. Check what went wrong
4. Fix the issue
5. Click "Retry" or "Submit" again
6. (Repeat if needed)
7. Eventually see success
```

### Switching Users

```
1. On Main Page, click "Sign Out"
2. Confirm logout
3. See Sign In page
4. Enter different username/password
5. Click Sign In
6. See Main Page with new account
```

### Changing Server

```
1. On Main Page, go to Settings
2. Find "Server Configuration"
3. Edit IP address
4. Click Save
5. App reconnects to new server
6. May need to sign in again
```

---

## Troubleshooting Navigation

**If you're stuck, try:**

1. **Look at current screen title** - Know where you are
2. **Find the button/field you need** - Check Main Page sections
3. **Use Back button if available** - Return to previous screen
4. **Sign out and sign back in** - Reset app state
5. **Restart app** - Clear temporary state
6. **Check Messages** - See history and past errors

---

## Tips for Efficient Navigation

- **Bookmark these pages** in your documents folder
- **Memorize server IP** so you don't need to reconfigure
- **Save customer names** to avoid re-entering
- **Keep camera accessible** for quick barcode scanning
- **Use "Remember me"** if on personal device to stay logged in
- **Keep phone charged** for location tracking during test drives

---

**Last Updated:** February 2026  
**Version:** 1.0
