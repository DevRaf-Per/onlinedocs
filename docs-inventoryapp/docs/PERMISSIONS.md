# Device Permissions & Settings Guide

Complete guide to app permissions and device settings for the OWPG Inventory Application.

## Overview

The OWPG app requires certain permissions to function properly. These permissions give the app access to your device's features (camera, location, storage, etc.). This guide explains what each permission does and how to manage them.

## Why Permissions Are Required

**Permissions protect your privacy** by:
- Making you aware of what app features can access
- Letting you control which apps can use which features
- Preventing unauthorized access to sensitive data
- Allowing you to revoke permissions any time

Each permission request in this app serves a specific function:

| Permission | Purpose | Can Work Without It? |
|-----------|---------|-------------------|
| Camera | Barcode scanning, photo capture | Limited (manual entry only) |
| Location | Vehicle tracking, GPS data | Partial (no location data) |
| Storage | Save photos, access files | Partial (no photo storage) |
| Network | Connect to server | No (core functionality) |
| Contacts | (Not requested) | N/A |

## Platform-Specific Permission Management

### Windows Desktop

Windows uses a different permission system than mobile devices. Most features work without explicit permission prompts.

#### Camera Permission

1. **Open Settings:**
   - Windows Settings > Privacy & Security > Camera
   
2. **Allow Camera Access:**
   - Toggle "Camera access" to **On**
   - Toggle "OWPG" to **Allow**

3. **Testing:**
   - Open OWPG app
   - Select Test Drive or other action
   - Tap Camera button
   - Camera should open and scan barcodes

#### Location Permission

1. **Open Settings:**
   - Windows Settings > Privacy & Security > Location
   
2. **Allow Location Access:**
   - Toggle "Location" to **On**
   - Scroll down and toggle "OWPG" to **Allow**

3. **Note:** Desktop location may use IP-based location (not GPS)

#### File Storage

- OWPG automatically uses its application directory
- No special permission required
- Photos stored in: `C:\Users\[YourName]\AppData\Local\OWPG\`

### iOS (iPhone/iPad)

iOS requests permissions with on-screen prompts when app needs them.

#### Camera Permission

**When First Requested:**
1. App opens, or you try to scan barcode
2. Popup appears: "OWPG Would Like to Access Your Camera"
3. Options:
   - **"Allow"** - Allow camera access
   - **"Allow Once"** - Allow only this time
   - **"Don't Allow"** - Deny camera access

**If You Selected "Don't Allow":**
1. Open **Settings** app
2. Scroll down and find **OWPG**
3. Tap **Camera**
4. Change to **Allow**
5. Return to OWPG app - camera now works

**Test Camera:**
1. Open OWPG
2. Select action
3. Tap Camera icon
4. Permission prompt appears
5. Select "Allow"
6. Camera view opens

#### Location Permission

**When First Requested:**
1. A dialog appears: "OWPG Requests Permission to Access Your Location"
2. Options:
   - **"Allow Once"** - Allow one time only
   - **"Allow While Using App"** - Allow while app is open (recommended)
   - **"Allow Always"** - Allow in background too
   - **"Don't Allow"** - Deny location access

**Recommended Setting:** "Allow While Using App"
- Balances privacy and functionality
- Location tracked during active use
- Stops tracking when you minimize app

**For Background Tracking (advanced):**
- Select "Allow Always" (uses more battery)
- Useful for long test drives

**If You Need to Change:**
1. Open **Settings** app
2. Scroll to **OWPG**
3. Tap **Location**
4. Select desired option:
   - Never
   - While Using App
   - Always
5. Return to app

#### Storage Permission

iOS automatically manages storage for app files.
- No explicit permission needed
- Photos stored in: Settings > OWPG > Local Storage

**If You Can't Save Photos:**
1. Settings > OWPG > Photos > Allow

#### Reset All Permissions

To reset all app permissions on iOS:
1. Settings > General > iPhone Storage
2. Find "OWPG"
3. Tap "Offload App" (keeps data)
4. Or "Delete App" (removes everything)
5. Reinstall from App Store

### Android (Phone/Tablet)

Android requests permissions during first use and in app settings.

#### Camera Permission

**During First Use:**
1. Tap Camera button
2. Permission dialog: "OWPG wants access to Camera"
3. Options:
   - **"Allow"** - Grant permission
   - **"Allow only this time"** - One-time use
   - **"Don't allow"** - Deny

**If You Selected "Don't Allow":**
1. Open **Settings**
2. Tap **Apps** or **Application Manager**
3. Find and tap **OWPG**
4. Tap **Permissions**
5. Tap **Camera**
6. Select **Allow**

**Test Camera:**
1. Open OWPG app
2. Try barcode scanner
3. Should work after permission granted

#### Location Permission

**During First Use:**
1. App requests location permission
2. Two options appear:
   - **"While using the app"** - Location only during active use (recommended)
   - **"All the time"** - Allow background location tracking
   - **"Only this time"** - One-time permission
   - **"Don't allow"** - Deny

**Recommended:** "While using the app"

**For Continuous Tracking (advanced):**
- Select "All the time" (requires Android 10+)
- Uses more battery and data
- Enables background location service

**If You Need to Change:**
1. Open **Settings**
2. Tap **Apps** > **OWPG** (or **Permissions** > **Location**)
3. Tap **Permissions** > **Location**
4. Select desired setting
5. Return to app

#### File Storage Permission

**During First Use:**
1. Dialog asks for storage/file access
2. Select **"Allow"** to enable photo storage

**If Already Denied:**
1. Settings > Apps > OWPG > Permissions
2. Tap **Files and Media**
3. Select **Allow**

#### Foreground Service Permission (Android 12+)

**What It Is:** Permission for location service to run while app is visible

**When Requested:**
1. Notification prompt appears
2. Select **"Allow"**
3. This enables background location tracking

#### Battery Optimization (Android)

Some Android devices have aggressive battery management that might stop the app's background location service.

**To Prevent:**
1. Settings > Battery > Battery Optimization (varies by device)
2. Find **OWPG** in list
3. Select **"Don't optimize"** or **"Excluded"**
4. This allows background location to continue

**Device-Specific Steps:**
- **Samsung:** Settings > Device Care > Battery > App Power Management > Excluded
- **Google Pixel:** Settings > Battery > Battery Saver > Manage Battery Saver > Excluded
- **Other:** Settings > Battery > Battery Optimization > OWPG > Don't Optimize

#### Manage All Permissions

**Quick Method:**
1. Open **Settings**
2. Tap **Apps & notifications**
3. Find **OWPG**
4. Tap **Permissions**
5. View and change any permission:
   - Camera
   - Location
   - Microphone
   - Storage/Files
   - Phone

**Reset Permissions:**
1. Settings > Apps > OWPG
2. Tap three dots (⋮) or menu
3. Select **Uninstall** or **Disable**
4. Reinstall from Play Store

### macOS (Mac)

macOS handles permissions through System Preferences.

#### Camera Permission

1. Open **System Preferences**
2. Go to **Privacy & Security** > **Camera**
3. Find **OWPG** in the list
4. Ensure it has a checkmark (✓)
5. If not in list:
   - Restart OWPG app
   - Grant permission when prompted
   - Permission will be added automatically

**Test Camera:**
1. Open OWPG
2. Try camera/barcode scanner
3. Camera view should open

#### Location Permission

1. **System Preferences** > **Privacy & Security** > **Location Services**
2. Find **OWPG** in list
3. Ensure checkmark (✓) is present
4. For continuous tracking, look for related system services

#### Reset Permissions

To reset all OWPG permissions on macOS:
1. Open **Terminal**
2. Command: `tccutil reset All com.companyname.inventoryapp`
3. Restart OWPG
4. Grant permissions when prompted

## Common Permission Scenarios

### "Permission Denied" Error When Opening Camera

**Problem:** Error appears when trying to scan barcode

**Solution:**
1. Go to device Settings
2. Find app permissions section
3. Locate **Camera** permission for OWPG
4. Change from "Deny" or "Never" to "Allow"
5. Return to app and try again

### Camera Opens But Very Slow

**Problem:** Camera takes 5+ seconds to open or is laggy

**Cause:** Camera permission may be restricted or other apps using camera

**Solutions:**
1. Close other apps using camera
2. Ensure camera permission is fully enabled
3. Restart the OWPG app
4. Restart device if issue persists

### Location Not Working/Tracking

**Problem:** App won't track location or shows no location data

**Solutions:**

1. **Check Permission:**
   - Verify Location permission is set to "Allow" or "Always"
   - Not set to "Never" or "Deny"

2. **Check Location Services:**
   - Settings > Location Services (or GPS)
   - Ensure **On** or **Enabled**

3. **Check Battery Saver:**
   - Disable battery saver mode (uses more battery)
   - Or whitelist OWPG app in battery saver exceptions

4. **Check Internet:**
   - Location requires internet connection
   - Ensure WiFi or cellular data is connected

5. **Check Accuracy:**
   - Indoor locations are less accurate
   - Move outside for better GPS signal
   - Give GPS 30-60 seconds to acquire signal

6. **For Android:**
   - Ensure "High Accuracy" location mode is enabled
   - Not set to "Battery Saver" mode

### Can't Save Photos

**Problem:** Photos won't save or error appears

**Solutions:**

1. **Check Storage Permission:**
   - Verify storage/files permission is enabled
   - Grant permission if denied

2. **Check Device Storage:**
   - Device may be out of space
   - Delete unnecessary files to free space
   - Check Settings > Storage

3. **Check Location:**
   - Verify app is trying to save to valid location
   - On some devices, this location may be restricted

4. **Restart App:**
   - Close and reopen OWPG
   - Try saving photo again

### "App is Running in Background" Warnings

**What This Means:**
- OWPG is using location/resources in background
- This is normal during active operations

**To Control:**
1. **Reduce Battery Impact:**
   - Settings > Battery > Reduce Battery Usage
   - Or disable "Always" location permission
   - Use "While Using App" instead

2. **Stop Location Tracking:**
   - Sign out of app (stops background activity)
   - Or manually disable location permission

### Need All Permissions but Can't Grant Them

**Situation:** Some permissions won't grant (grayed out)

**Possible Causes:**
1. Device policy restrictions (work device)
2. Parental controls preventing permission changes
3. Device owner settings preventing camera/location

**Solutions:**
1. Contact your device administrator
2. Contact IT department (if work device)
3. Remove device restrictions if applicable
4. For personal device, check parental controls

## Permission Impact on Features

### Without Camera Permission
- ❌ Cannot scan barcodes with camera
- ❌ Cannot capture photos
- ✓ Can manually enter barcode
- ✓ Can still submit forms

**Impact:** Minor - camera is helpful but optional

### Without Location Permission
- ❌ Cannot track vehicle location
- ❌ No GPS data recorded
- ✓ Can still perform all other functions
- ✓ Can still submit checkouts

**Impact:** Medium - location tracking disabled, but core functions work

### Without Storage Permission
- ❌ Cannot save photos to device
- ❌ Photos not persistent
- ✓ Can view photos temporarily
- ✓ Can submit forms without photos

**Impact:** Low - affects documentation capability

### Without Network Permission
- ❌ Cannot connect to server
- ❌ Cannot sign in
- ❌ Cannot submit checkouts
- ✗ App is non-functional

**Impact:** Critical - app will not work

## Best Practices for Permissions

### Recommended Settings

| Permission | Setting | Reason |
|-----------|---------|--------|
| Camera | **Allow** | Needed for barcode scanning |
| Location | **While Using App** | Balances functionality and battery |
| Storage | **Allow** | Needed to save photos |
| Network | **Allow** | Required for basic function |

### Privacy Tips

1. **Review Permissions Regularly:**
   - Check Settings monthly
   - Remove permissions you don't need
   - Revoke for unused apps

2. **Disable When Not Needed:**
   - Disable location after work hours
   - Turn off camera if only doing manual entry
   - Disable if device is loaned to others

3. **Use "While Using App" for Location:**
   - Saves battery
   - Provides privacy when app is closed
   - Still allows tracking during checkout

4. **Be Aware of Background Activity:**
   - Location tracking uses battery
   - "Always Allow" consumes more power
   - Monitor battery impact in settings

## Troubleshooting Permission Issues

### Permission Already Granted But Not Working

**Solutions:**

1. **Restart App:**
   - Close OWPG completely
   - Wait 5 seconds
   - Reopen

2. **Restart Device:**
   - Power off device
   - Power on after 10 seconds
   - Reopen OWPG

3. **Clear App Cache:**
   - Settings > Apps > OWPG > Storage > Clear Cache
   - (Doesn't delete your data)

4. **Reinstall App:**
   - Uninstall OWPG
   - Restart device
   - Reinstall from app store
   - Grant permissions fresh

5. **Check Device Date/Time:**
   - Settings > Date & Time > Auto
   - Incorrect time can cause permission issues

### Permission Prompt Won't Appear

**Possible Causes:**
- Permission already granted (check settings)
- Permission previously denied and set to "Don't ask again"
- Device type doesn't support that permission

**Solutions:**
1. Go to app Settings > Permissions
2. Manually enable the permission
3. Return to app - it should now work

### "Device Administrator" Blocking Permissions

**What This Means:**
- Device is managed by your organization
- IT has restrictions in place
- Cannot change certain permissions

**What To Do:**
1. Contact your IT administrator
2. Request permission to be enabled
3. Provide reason (e.g., "Need camera for barcode scanning")
4. Administrator may grant temporarily or permanently

## Permission Settings by Device Type

### Work Devices

**Common Restrictions:**
- Camera may be disabled
- Location may be monitored centrally
- Storage may be restricted
- Some permissions may be grayed out

**What To Do:**
- Contact IT for any permission changes
- Ask IT to enable camera/location if needed
- Follow your organization's device policies

### Personal Devices

**Full Control:**
- You control all permissions
- No restrictions on enabling/disabling
- IT cannot see your permissions
- You responsible for protecting device

**Recommendation:**
- Enable only permissions you need
- Regularly review and revoke unused permissions
- Keep software updated for security

### Shared Devices

**Best Practice:**
- Sign out when finished
- Don't grant sensitive permissions permanently
- Consider "Allow Only This Time" option
- Reset app permissions between users

## FAQ - Permissions

**Q: Why does the app need camera permission?**
A: Camera is used for barcode scanning. Without it, you must manually enter barcodes.

**Q: Why does the app need location permission?**
A: Location is used to track vehicle position during test drives and operations. This is a core feature.

**Q: Can I revoke permissions after allowing them?**
A: Yes, anytime. Go to Settings > Apps > OWPG > Permissions and change any setting.

**Q: Does the app use location in background?**
A: Only if you grant "Always Allow" permission. Default is "While Using App" which stops when app closes.

**Q: Will location tracking drain my battery?**
A: Moderate impact. GPS uses more battery than WiFi location. If battery is a concern, use WiFi location or disable when not in use.

**Q: Can my employer see my location data?**
A: Only the location data from official checkouts (submitted through app). Your personal movement is not tracked.

**Q: What if I accidentally denied a permission?**
A: Go to Settings > Apps > OWPG > Permissions and re-enable it. Some devices may ask for permission again next time you use that feature.

**Q: Can I use the app without granting any permissions?**
A: Mostly. You can manually enter data, but camera for barcodes and location tracking won't work.

---

**Last Updated:** February 2026  
**Document Version:** 1.0
