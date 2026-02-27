# OWPG Inventory Application

A mobile and desktop application for managing vehicle checkouts, test drives, and inventory tracking with real-time location monitoring and barcode scanning capabilities.

## Table of Contents

- [Overview](#overview)
- [Getting Started](#getting-started)
- [Features](#features)
- [System Requirements](#system-requirements)
- [Installation](#installation)
- [First Time Setup](#first-time-setup)
- [Using the Application](#using-the-application)
- [Troubleshooting](#troubleshooting)
- [FAQ](#faq)
- [Support](#support)

## Overview

The OWPG Inventory Application is a comprehensive vehicle management system designed to streamline vehicle checkouts, test drives, and inventory tracking. The application runs on multiple platforms including Windows, iOS, Android, and macOS, allowing you to manage your inventory on the go or from your desktop.

**Key Capabilities:**
- Secure sign-in authentication
- Vehicle barcode scanning
- Real-time location tracking
- Test drive information management
- Maintenance and relocation tracking
- Photo and document capture
- Message logging and retrieval

## Getting Started

### What You'll Need

Before you begin, ensure you have:

1. **Network Connectivity** - The app requires a connection to the MQTT server (typically configured with an IP address like 192.168.x.x or a server hostname)
2. **Device** - Windows PC, iPhone, iPad, or Android device
3. **User Credentials** - Your sign-in username and password provided by your administrator
4. **Device ID** - A unique identifier created automatically on first use

## System Requirements

### Windows Desktop
- Windows 10 (version 17763) or later
- 100 MB free disk space
- Internet connection

### iOS
- iOS 15.0 or later
- 150 MB free space
- Camera permissions for barcode scanning

### Android
- Android 8.0 (API 26) or later
- 150 MB free space
- Camera and location permissions

### macOS
- macOS 15.0 or later
- 150 MB free space
- Camera permissions

## Installation

### Windows
1. Download the OWPG application installer
2. Run the installer and follow the on-screen instructions
3. Grant any permission requests (camera, location, file access)
4. Launch the application

### iOS
1. Install from the Apple App Store
2. Open the application
3. Grant camera and location permissions when prompted

### Android
1. Install from Google Play Store
2. Open the application
3. Grant camera, location, and file storage permissions when prompted

### macOS
1. Download the application from the designated source
2. Install to your Applications folder
3. Grant camera permissions when prompted
4. Launch the application

## First Time Setup

### Step 1: Server Configuration (IP Address)

When you launch the app for the first time, you'll be directed to the **IP Lookup Page**:

1. Enter the **Server IP Address** provided by your administrator (e.g., `192.168.1.100`)
2. This is the address of the MQTT server that the app will communicate with
3. Tap **Connect** to proceed
4. The app will save this setting for future use

### Step 2: Sign In

After configuring the server address, you'll see the **Sign In Page**:

1. Enter your **Username** (provided by your administrator)
2. Enter your **Password** (provided by your administrator)
3. Tap **Sign In**
4. Upon successful authentication, you'll be directed to the main page

### Automatic Device Registration

On first launch, the app automatically:
- Creates a unique **Device ID** (stored securely on your device)
- Creates a unique **User ID** (tied to your specific device)
- Stores your **Session Token** after sign-in (keeps you logged in)

These IDs are used for tracking and auditing purposes.

## Using the Application

### Main Page Overview

The main page is your central hub for all vehicle checkout operations. It consists of:

- **Logo & Title** - "Vehicle Checkout" header with application logo
- **Action Selection** - Dropdown menu to select the reason for checkout
- **Vehicle ID Input** - Barcode scanning or manual entry
- **Form Fields** - Context-specific fields based on your selected action
- **Submit Button** - Complete your checkout operation

### Selecting an Action

The app supports six types of operations:

#### 1. **Test Drive** ✓ (Most Common)
Used when a customer is taking a vehicle for a test drive.

**Required Information:**
- Customer Name (click the * button to edit)
- Phone Number
- Number of People
- Driver's License (checkbox confirmation)
- Insurance Information (checkbox confirmation)
- Picture/Video Access Permission (checkbox confirmation)
- Vehicle Beacon ID (barcode)

**Additional Options:**
- Capture photos of the vehicle (optional)
- Record video documentation
- Attach customer signature

#### 2. **Maintenance**
Used for scheduled maintenance or repairs.

**Required Information:**
- Service Type (e.g., Oil Change, Tire Rotation)
- Maintenance Duration
- Vehicle Beacon ID (barcode)
- Notes/Description

#### 3. **Relocation**
Used when moving vehicles between locations.

**Required Information:**
- From Location
- To Location
- Vehicle Beacon ID (barcode)
- Notes

#### 4. **Transfer**
Used for vehicle transfers between departments or personnel.

**Required Information:**
- From Department/Person
- To Department/Person
- Transfer Reason
- Vehicle Beacon ID (barcode)

#### 5. **Service Test**
Used for testing vehicle functionality.

**Required Information:**
- Test Type
- Test Results
- Vehicle Beacon ID (barcode)

#### 6. **Other**
For operations not covered by the above categories.

**Required Information:**
- Description
- Vehicle Beacon ID (barcode)
- Additional Notes

### Scanning a Vehicle Barcode

#### Using the Camera Scanner (Recommended)

1. Select your desired action from the dropdown
2. Tap the **Camera Icon** button next to the "Vehicle Beacon ID" field
3. Point your device's camera at the barcode
4. The app will automatically detect and read the barcode
5. The barcode value will be entered automatically
6. The scanner will close and return you to the form

#### Manual Entry

1. If scanning isn't available or doesn't work:
   - Tap the **Vehicle Beacon ID** text field
   - Type or paste the barcode value manually
   - Continue with form completion

**Barcode Format:** The app extracts a 12-character code from the barcode (characters 4-16 if the barcode is longer than 16 characters).

### Entering Customer Information (Test Drive)

For Test Drive operations:

1. Tap the **Edit Customer Name Button** (the * button)
2. A dialog will appear where you can:
   - Add the customer's first and last name
   - View previously saved customer names
   - Search for existing customers
3. Confirm your selection
4. The form will show a confirmation that customer information is set

**Note:** Customer names are saved locally for faster entry on future checkouts.

### Capturing Photos and Videos

When enabled for your action type:

1. Tap **Camera** button
2. Capture photos of the vehicle (exterior, interior, etc.)
3. You can:
   - Take multiple photos
   - Review before saving
   - Delete unwanted photos
   - Add captions to photos

4. Tap **Video** button to record video documentation
5. Return to the form to complete submission

### Location Tracking

The app automatically:
- Requests permission to access your device's location
- Records GPS location data (latitude, longitude, speed, timestamp)
- Stores location data in a local file
- Transmits location to the server when available

**Location Permission:** 
- On first use, you'll be prompted to allow location access
- Select "Allow While Using the App" or "Always Allow" depending on your preference
- On Android, the app runs a background location service

### Submitting Your Checkout

1. Complete all required fields (marked with *)
2. Review the information for accuracy
3. Tap the **Submit** button
4. You'll see a loading indicator while the data is transmitted
5. Upon success, you'll see a success message
6. The form will clear and you can perform another checkout

### Messages and History

The app maintains a local database of all messages and checkouts:

1. Tap the **Messages** icon (if available)
2. View a list of all recent checkouts and activities
3. Each message shows:
   - Timestamp
   - Action type
   - Vehicle information
   - Status (sent, pending, failed)
4. Tap a message to view full details

### Sign Out

To sign out and switch to a different user:

1. Tap the **Sign Out** button or menu option
2. Confirm that you want to sign out
3. You'll be returned to the sign-in page
4. You can now sign in with different credentials

## Troubleshooting

### "Cannot Connect to Server"

**Problem:** The app shows an error that it cannot connect to the MQTT server.

**Solutions:**
1. **Check IP Address:**
   - Verify the server IP address is correct
   - Contact your administrator for the correct IP
   - On Windows, go to Settings to reconfigure the IP address

2. **Check Network Connection:**
   - Ensure your device has WiFi or internet connectivity
   - Try connecting to a different network if available
   - Restart your device's network connection

3. **Check Server Status:**
   - Ask your administrator to verify the server is running
   - Check if there are any network maintenance windows

### "Sign In Failed"

**Problem:** Username or password is being rejected.

**Solutions:**
1. **Verify Credentials:**
   - Ensure CAPS LOCK is not enabled
   - Double-check username and password for typos
   - Contact your administrator to reset your password

2. **Clear App Data (Windows):**
   - Uninstall and reinstall the application
   - This clears any corrupted session tokens

3. **Verify Internet Connection:**
   - Ensure you're connected to the network

### Barcode Scanner Not Working

**Problem:** Camera opens but doesn't detect barcodes.

**Solutions:**
1. **Check Lighting:**
   - Ensure adequate lighting on the barcode
   - Avoid shadows and reflections
   - Hold the camera 6-12 inches from the barcode

2. **Check Permissions:**
   - Verify camera permissions are granted
   - Settings > App Permissions > Camera > Enable for OWPG

3. **Try Manual Entry:**
   - If scanning continues to fail, enter the barcode manually
   - Type or paste the barcode value in the text field

4. **Restart Scanner:**
   - Close the scanner and reopen
   - This often resolves temporary camera issues

### Application Crashes or Freezes

**Problem:** The app crashes or becomes unresponsive.

**Solutions:**
1. **Force Close and Restart:**
   - Close the application completely
   - Wait 10 seconds
   - Reopen the application

2. **Restart Your Device:**
   - Power off and power on your device
   - This clears memory and caches

3. **Clear App Cache (if available):**
   - Settings > Apps > OWPG > Storage > Clear Cache
   - This doesn't delete your data, just temporary files

4. **Reinstall Application:**
   - Uninstall the OWPG application
   - Download and install the latest version
   - Sign in again

### Missing or Duplicate Location Data

**Problem:** Location tracking seems inconsistent.

**Solutions:**
1. **Check Location Permissions:**
   - Settings > Location > Ensure OWPG has permission
   - On Android, ensure "Always Allow" is selected for background tracking

2. **Enable Location Services:**
   - Settings > Location > Toggle On
   - Ensure GPS is enabled

3. **Check Battery Saver:**
   - Some devices restrict background location in battery saver mode
   - Disable battery saver or whitelist OWPG

### Form Data Not Saving

**Problem:** Entered information is lost when navigating away.

**Solutions:**
1. **Check Network Connection:**
   - Ensure you're still connected
   - Form won't clear if submission fails

2. **Complete All Required Fields:**
   - Verify all fields marked with * are filled
   - Look for any validation error messages

3. **Try Again:**
   - Re-enter the information
   - Tap Submit again

## FAQ

### Q: Is my data secure?
**A:** Yes. The app uses industry-standard encryption (TLS) to communicate with the server. Your credentials are validated and sessions are protected with tokens. Local data is stored securely on your device.

### Q: What happens if I lose internet connection during checkout?
**A:** The app will attempt to save your data locally and sync when connection is restored. You'll see a notification about the connection status.

### Q: Can I use the app offline?
**A:** Limited functionality is available offline. You can view local message history and fill out forms, but you cannot submit new checkouts without an internet connection.

### Q: How do I change the server IP address?
**A:** 
- **Windows:** Settings > App Settings > Server Configuration
- **iOS/Android:** Settings > App Preferences > Network Settings
- Or contact your administrator to reset the app

### Q: Are test drive photos permanently stored?
**A:** Photos are stored on your device's local storage. The retention period depends on your device's storage availability and your organization's policies. Contact your IT department for backup procedures.

### Q: Can multiple users use the same device?
**A:** Yes, but each user must sign in separately. Each user gets their own session and Device/User ID for tracking purposes.

### Q: What's the difference between Device ID and User ID?
**A:**
- **Device ID:** A unique identifier for the physical device (created once, never changes)
- **User ID:** A unique identifier for each user account (changes when you sign out and sign in as different user)

### Q: How often is location data transmitted?
**A:** Location is tracked whenever you're using the app and have location permissions enabled. Data is batched and transmitted when network connectivity is available.

### Q: What if I see "Session Token Expired"?
**A:** Simply sign out and sign back in. Your session will be renewed.

### Q: Can I transfer data between devices?
**A:** No. Each device maintains its own local database. To access data from another device, sign in with your account credentials on that device.

## Support

If you encounter issues not covered in this documentation:

1. **Take a Screenshot** - Capture any error messages
2. **Note the Steps** - Write down what you were doing when the issue occurred
3. **Check System Info:**
   - **Windows:** Settings > System > About
   - **iOS:** Settings > General > About
   - **Android:** Settings > About Phone
4. **Contact Your Administrator or IT Support** with:
   - Device model and OS version
   - Application version
   - Error message (with screenshot)
   - Steps to reproduce the issue
   - Your Device ID (shown in app settings)

## Additional Resources

- [Getting Started with Test Drives](./TESTDRIVE_GUIDE.md)
- [Vehicle Barcode Scanning Tips](./BARCODE_GUIDE.md)
- [Privacy and Data Security](./PRIVACY.md)
- [Device Permissions and Settings](./PERMISSIONS.md)

---

**Application Name:** OWPG Inventory Application  
**Current Version:** 1.0  
**Last Updated:** February 2026  
**Support Contact:** Your Administrator or IT Department
