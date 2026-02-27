# Installation & Setup Guide

Complete instructions for downloading, installing, and setting up the OWPG Inventory Application on your device.

## Table of Contents

- [Before You Start](#before-you-start)
- [Windows Installation](#windows-installation)
- [iOS Installation](#ios-installation)
- [Android Installation](#android-installation)
- [macOS Installation](#macos-installation)
- [First Time Setup](#first-time-setup)
- [Verify Installation](#verify-installation)
- [Troubleshooting Installation](#troubleshooting-installation)

## Before You Start

### What You'll Need

1. **Device Requirements** (see below for your platform)
2. **Credentials:**
   - Username (provided by your administrator)
   - Password (provided by your administrator)
3. **Network Information:**
   - Server IP address or hostname (from administrator)
   - Internet/WiFi connection
4. **Permissions:**
   - Administrator rights on computer (for Windows desktop app)
   - Ability to grant app permissions on mobile devices

### Getting Information From Your Administrator

Before installing, contact your administrator to get:

```
Server Configuration:
  IP Address: ___________________
  Server Port: ___________________
  Hostname: ___________________
  
Credentials:
  Username: ___________________
  Initial Password: ___________________
  
Support Contact:
  Phone: ___________________
  Email: ___________________
```

---

## Windows Installation

### System Requirements

**Minimum:**
- Windows 10 (version 17763.0) or later
- Windows 11 recommended
- 100 MB free disk space
- 2 GB RAM minimum (4 GB recommended)
- Internet connection

**Supported Versions:**
- Windows 10 (all current versions)
- Windows 11 (all current versions)

### Step-by-Step Installation

#### Option 1: Windows Store (Easiest)

1. **Open Microsoft Store**
   - Click Windows Start menu
   - Search for "Microsoft Store"
   - Click to open

2. **Search for OWPG**
   - In Store, click search bar (magnifying glass)
   - Type "OWPG" or "Inventory App"
   - Press Enter

3. **Install Application**
   - Click the app in results
   - Click "Get" button (or "Install")
   - Microsoft Store downloads and installs

4. **Wait for Completion**
   - Installation shows progress
   - When done, says "Launch"
   - Click "Launch" to start

5. **First Launch**
   - App opens to IP Lookup page
   - Enter server IP (from administrator)
   - Click Connect
   - See [First Time Setup](#first-time-setup) below

#### Option 2: Direct Download

If your company provides a direct download link:

1. **Download Installer**
   - Click link from company email
   - Or download from company portal
   - Save to Downloads folder
   - File name is usually: `OWPGSetup.exe` or similar

2. **Run Installer**
   - Double-click the `.exe` file
   - You may see: "Do you want to allow this app to make changes?"
   - Click "Yes" to allow

3. **Follow Installation Wizard**
   - Click "Next" at each screen
   - Accept license agreement
   - Choose installation folder (default is fine)
   - Click "Install"
   - Wait for files to copy

4. **Complete Installation**
   - Click "Finish"
   - Option to launch app immediately
   - Check "Launch OWPG" and click Finish
   - App opens

5. **Grant Permissions**
   - Windows may ask for firewall permission
   - Click "Allow" to let app access network
   - Check both "Private" and "Public" boxes
   - Click "Allow"

6. **First Launch**
   - See [First Time Setup](#first-time-setup) below

### Windows Installation Issues

**"User Account Control" prompt appears**
- Click "Yes" to allow installation
- This is normal and required

**"Smartscreen" warning appears**
- Click "More info"
- Click "Run anyway"
- App is safe but Windows warns about new apps

**Installation path issues**
- Use default path: `C:\Program Files\...`
- Don't install to network drives or removable media
- Ensure folder has at least 100 MB free

### After Installation on Windows

**Create Shortcut (Optional)**
1. After installation, find shortcut on Desktop
2. Right-click > Pin to taskbar
3. App appears in taskbar for quick access

**Auto-Update**
- App will check for updates automatically
- You'll be notified when updates are available
- Updates install automatically or on restart

---

## iOS Installation

### System Requirements

**Minimum:**
- iPhone or iPad
- iOS 15.0 or later
- iOS 17+ recommended
- 150 MB free space
- WiFi or cellular data

**Supported Devices:**
- iPhone 8 and later
- iPad (5th generation) and later
- iPad Air 2 and later
- iPad mini 4 and later
- iPad Pro (all)

### Step-by-Step Installation

1. **Open App Store**
   - On home screen, find blue "App Store" icon
   - Tap to open

2. **Search for App**
   - Tap "Search" tab at bottom
   - Tap search bar at top
   - Type "OWPG" or "Inventory App"
   - Tap "Search"

3. **Find and Install**
   - Look for app with OWPG icon
   - Tap the app name to open its page
   - Tap "Get" (cloud with arrow)
   - You may need to:
     - Authenticate with Face ID, Touch ID, or Apple ID password
     - Agree to App Store terms

4. **Wait for Installation**
   - "Get" changes to "Installing"
   - When done, shows "Open"
   - Don't force close - let installation complete

5. **Launch App**
   - Tap "Open" to start
   - Or find app on home screen and tap it

6. **Grant Permissions**
   - First time, app asks for permission to:
     - **Camera:** For barcode scanning
       - Tap "Allow"
     - **Location:** For GPS tracking
       - Tap "Allow While Using App" (recommended)
       - Or "Allow Always" for background tracking
     - **Photo Library:** For accessing/saving images
       - Tap "Allow"
   - Each permission can be changed later in Settings

7. **First Launch**
   - App opens to IP Lookup page
   - See [First Time Setup](#first-time-setup) below

### iOS Installation Issues

**"Cannot Download at This Time"**
- Check WiFi or cellular connection
- Restart iPhone: Settings > Power Off > slide
- Try again in a few minutes
- Check storage space: Settings > General > iPhone Storage

**App Crashes on Launch**
- Force close: Swipe up from bottom of screen (old iPhone: double tap home)
- Delete and reinstall from App Store
- Restart iPhone

**Very Slow Installation**
- Check WiFi signal strength
- Download on faster network if available
- Close other apps to free memory

### After Installation on iOS

**Add to Home Screen Shortcut**
1. Long-press the app icon
2. Select "Add to Home Screen"
3. App icon appears where you place it

**Enable Background App Refresh (Optional)**
1. Settings > General > Background App Refresh
2. Find OWPG and enable
3. Allows location tracking in background

---

## Android Installation

### System Requirements

**Minimum:**
- Android 8.0 (API level 26) or later
- Android 10+ recommended
- 150 MB free space
- 2 GB RAM minimum (4 GB recommended)
- WiFi or cellular data

**Supported Devices:**
- Most Android smartphones from 2017 onwards
- Most Android tablets from 2016 onwards

### Step-by-Step Installation

1. **Open Google Play Store**
   - Find app with colorful Google Play icon
   - Tap to open
   - (May need to sign in with Google account)

2. **Search for App**
   - Tap search icon (magnifying glass) at top
   - Type "OWPG" or "Inventory App"
   - Tap search

3. **Find and Install**
   - Look for app with OWPG icon
   - Tap app name to open its page
   - Tap "Install" button
   - You may need to:
     - Authenticate with fingerprint or Google account
     - Review permissions (see [Permissions](#android-permissions-overview) section)

4. **Review App Permissions**
   - Before installing, screen shows:
     - Camera
     - Location
     - Storage
     - Network
   - Tap "Install" to accept all

5. **Wait for Installation**
   - "Install" button changes to "Installing..."
   - Progress bar shows installation progress
   - When done, shows "Open"

6. **Launch App**
   - Tap "Open" button
   - Or find app in app drawer and tap it

7. **Grant Runtime Permissions**
   - When you try to use camera:
     - Dialog: "Allow [App] to access camera?"
     - Tap "Allow"
   - When you try to access location:
     - Dialog: "Allow [App] to access location?"
     - Choose:
       - "While using the app" (recommended)
       - "Only this time"
       - "Don't allow"
   - For storage/photos:
     - Tap "Allow" to enable photo saving

8. **First Launch**
   - App opens to IP Lookup page
   - See [First Time Setup](#first-time-setup) below

### Android Installation Issues

**"Cannot download"**
- Check WiFi connection
- Ensure sufficient storage (Settings > Storage)
- Restart phone: Power off and on
- Try again

**Installation hangs at "Installing..."**
- Wait 5 minutes minimum (can be slow)
- Check WiFi is still connected
- If still frozen after 10 min: restart phone and try again

**"Not compatible with your device"**
- Device may not meet Android version requirement
- Check Android version: Settings > About Phone
- Upgrade Android if available
- Contact administrator for alternative versions

**Play Store won't open**
- Restart phone
- Clear Play Store cache: Settings > Apps > Play Store > Storage > Clear Cache
- Sign in to Google account

### After Installation on Android

**Add Shortcut to Home Screen**
1. Long-press app icon
2. Select "Add to Home"
3. Choose where to place
4. Shortcut appears on home screen

**Battery Optimization Exceptions**
1. Settings > Battery (or Device Care)
2. Find "Battery Optimization" or "Battery Saver"
3. Add OWPG to exceptions
4. Allows background location tracking

---

## macOS Installation

### System Requirements

**Minimum:**
- Mac with Apple Silicon (M1) or Intel processor
- macOS 12 (Monterey) or later
- macOS 13+ recommended
- 150 MB free space
- 2 GB RAM minimum
- WiFi or internet connection

**Compatible Macs:**
- MacBook Air (2018+)
- MacBook Pro (2015+)
- Mac Mini (2014+)
- iMac (2015+)
- Mac Studio
- Anything with macOS 12+

### Step-by-Step Installation

#### Option 1: App Store (If Available)

1. **Open App Store**
   - Click blue "App Store" icon in Dock
   - Or open Launchpad > App Store

2. **Search for OWPG**
   - Click search icon
   - Type "OWPG" or "Inventory App"
   - Press Enter

3. **Install App**
   - Click app result
   - Click "Get" button
   - You may need to authenticate with Touch ID or Apple ID password

4. **Wait for Installation**
   - "Get" changes to "Install"
   - When done, shows "Open"

5. **Launch**
   - Click "Open"
   - Or find app in Applications folder and double-click

#### Option 2: Direct Download

1. **Download App**
   - Click link from company email
   - Or download from company portal
   - File is usually `.zip` or `.dmg`

2. **Mount DMG (if .dmg file)**
   - Double-click the `.dmg` file
   - Disk mounts on desktop
   - Shows install window with app icon

3. **Install Application**
   - Drag OWPG app icon to "Applications" folder
   - Or double-click the app directly to run

4. **Grant Permission**
   - First launch, macOS asks:
     - "Are you sure you want to open 'OWPG'?"
     - Click "Open"
   - App may ask for:
     - Camera permission: Click "Allow"
     - Location permission: Click "Allow"
     - File access: Click "Allow"

5. **First Launch**
   - App opens to IP Lookup page
   - See [First Time Setup](#first-time-setup) below

### macOS Installation Issues

**"App is damaged and can't be opened"**
- Right-click app in Applications
- Select "Open"
- Click "Open" in dialog
- This is a security check

**"App is not signed"**
- App may be from unknown developer
- Settings > Security & Privacy > Open Anyway
- Find app and click "Open"
- Only appears first time

**App won't launch**
- Try removing and reinstalling
- Restart Mac: Apple menu > Restart
- Check macOS is up to date: Apple menu > About This Mac > Software Update

**Very slow startup**
- Check available storage: Apple menu > About This Mac > Storage
- Free up space if less than 1 GB available
- Restart Mac

### After Installation on macOS

**Add to Dock (Quick Access)**
1. Open Applications folder
2. Find OWPG app
3. Right-click > Add to Dock
4. App icon now in Dock for quick access

**Create Alias for Easy Access**
1. Right-click app in Applications
2. Select "Make Alias"
3. Drag alias to Desktop or Documents
4. Double-click alias to launch

---

## First Time Setup

### Part 1: Server Configuration

When you open the app for the first time, you'll see the **IP Lookup Page**:

**What You'll See:**
- "Server Configuration" title
- Text field asking for server IP address
- "Connect" button

**What You Do:**

1. **Get IP Address from Administrator**
   - Your administrator provides this
   - Format: `192.168.1.100` or `server.company.com`
   - Write it down so you have it ready

2. **Enter IP Address**
   - Tap the text field
   - Type the IP address carefully
   - No spaces, check for typos

3. **Connect**
   - Tap "Connect" button
   - App connects to server
   - Wait 5-10 seconds

4. **Connection Successful**
   - If successful, app moves to Sign In page
   - If unsuccessful, see troubleshooting below

**If Connection Fails:**
- Check IP address is correct
- Verify internet connection (WiFi on, signal strong)
- Ask administrator to verify server is running
- Check if network access is restricted (firewall)

### Part 2: Sign In

After server setup, you'll see the **Sign In Page**:

**What You'll See:**
- Username field
- Password field
- "Sign In" button
- Possibly a "Remember me" checkbox

**What You Do:**

1. **Get Your Credentials**
   - Your administrator provided these
   - Write them down so you have them ready
   - Passwords are case-sensitive!

2. **Enter Username**
   - Tap username field
   - Type your username
   - Ensure caps lock is OFF

3. **Enter Password**
   - Tap password field
   - Type your password
   - Characters will appear as dots (•) for security
   - Ensure caps lock is OFF

4. **Remember Me (Optional)**
   - Check "Remember me" to stay signed in
   - Uncheck for more security
   - Recommended: Leave unchecked on shared devices

5. **Sign In**
   - Tap "Sign In" button
   - Wait 5-10 seconds while app authenticates
   - You should see loading indicator

6. **Successful Sign In**
   - App opens to Main Page (Vehicle Checkout page)
   - You're now ready to use the app

**If Sign In Fails:**

| Error | Solution |
|-------|----------|
| "Invalid username or password" | Check spelling, password case, caps lock off, try again |
| "Username not found" | Contact administrator to verify username |
| "Connection failed" | Check internet connection, verify server IP |
| "Too many failed attempts" | Wait 5 minutes, then try again |
| "Session expired" | Sign out and sign back in |

### Part 3: Automatic Setup

The app automatically:

1. **Creates Device ID** (unique to your device)
2. **Creates User ID** (unique to your user account)
3. **Requests Permissions:**
   - Camera (for barcode scanning)
   - Location (for GPS tracking)
   - Storage/Photos (for image saving)
4. **Initializes Database** (for local record storage)
5. **Sets Theme** (dark theme by default)

**Just Grant Permissions When Asked:**
- Allow camera access
- Allow location access
- Allow photo/storage access
- You can change these later in Settings

---

## Verify Installation

### After Installation, Verify Everything Works

#### Test 1: App Launches
- Close app if running
- Reopen app
- Should open without errors
- Should show IP Lookup page if not configured, or Main page if already signed in

#### Test 2: Sign In
- Close app completely
- Open app
- Should show Sign In page (if auto-sign-in not enabled)
- Enter credentials
- Click Sign In
- Should reach Main page in 5-10 seconds
- No error messages

#### Test 3: Camera Access
- On Main page, select any action from dropdown
- Tap Camera icon next to Vehicle Beacon ID
- Camera view should open
- You should see live camera feed
- Close scanner by tapping back or X

#### Test 4: Location Services (if enabled)
- On Main page
- If location permission granted, location should be tracking
- Check location permission in device settings
- Should show permission as "Allowed" or "While Using App"

#### Test 5: Network Connectivity
- On Main page
- Try submitting a test checkout (fill in required fields)
- Should send successfully (you can clear it after)
- If submit fails, check internet connection
- Check if server IP is correct

#### Test 6: Storage Access
- If camera test was successful
- Try taking and saving a photo
- Photo should save without errors
- Check if storage has sufficient space

### System Health Check

**Run these checks to ensure everything is set up properly:**

1. **Device has internet connection** ✓
2. **Server IP is configured correctly** ✓
3. **You're signed in successfully** ✓
4. **Camera permission is granted** ✓
5. **Location permission is granted** ✓
6. **App doesn't crash on main page** ✓
7. **You can scan a barcode** ✓
8. **You can take and save photos** ✓
9. **Form can submit successfully** ✓
10. **You can sign out and back in** ✓

If all checks pass, installation is complete! ✓

---

## Troubleshooting Installation

### General Installation Issues

#### App Won't Download
- ✓ Check WiFi/internet connection
- ✓ Ensure device storage has space (minimum 150 MB free)
- ✓ Restart device
- ✓ Try again

#### App Won't Launch After Installation
- ✓ Force close app (swipe up from bottom, or close in task manager)
- ✓ Restart device
- ✓ Uninstall and reinstall fresh
- ✓ Check app is compatible with your OS version

#### Installation is Very Slow
- ✓ Check you have WiFi connected (not cellular)
- ✓ Close other apps using internet
- ✓ Move closer to WiFi router
- ✓ Restart modem/router

#### Cannot Accept License Agreement
- ✓ Scroll down to see full agreement
- ✓ Check "I agree" checkbox
- ✓ Click "Accept" or "Next"
- ✓ If checkbox is grayed out, restart installer

### Platform-Specific Issues

#### Windows Issues
- **"Admin rights required"** → Right-click installer, "Run as Administrator"
- **"File in use" error** → Restart computer and try again
- **Firewall blocks app** → Click "Allow" when prompted, check both boxes
- **Won't uninstall** → Restart Windows, try again from Settings > Apps

#### iOS Issues
- **"Verification failed"** → Restart iPhone, try again, check internet
- **Stuck on "Installing"** → Wait 10 minutes, restart iPhone, try again
- **Not in App Store search** → App may not be available in your region
- **"Requires iOS X.X"** → Update iOS: Settings > General > Software Update

#### Android Issues
- **"Not compatible"** → Check Android version: Settings > About > Android version
- **"Insufficient space"** → Delete files/apps, free up 200 MB
- **Play Store crashes** → Clear cache: Settings > Apps > Play Store > Storage > Clear Cache
- **Stuck downloading** → Restart phone, check internet, try again

#### Mac Issues
- **"App is damaged"** → Right-click > Open, then Open in dialog
- **"Unsigned developer"** → Settings > Security & Privacy > Open Anyway
- **App doesn't appear after installation** → Check Applications folder, try again
- **Very slow startup** → Mac may be busy, try again later, restart if needed

### First Time Setup Issues

#### Can't Connect to Server
**Problem:** "Cannot connect to MQTT server" or "Connection failed"

**Solutions:**
1. **Check IP Address:**
   - Verify IP address is correct (ask administrator)
   - No spaces before/after
   - Correct format: 192.168.1.100 or hostname
   
2. **Check Internet:**
   - WiFi should show connected
   - Try browser: open any website to verify connection
   - If no internet, fix connection first

3. **Check Server Status:**
   - Ask administrator if server is running
   - Check if there's maintenance window
   - Verify server hasn't moved

4. **Check Network Restrictions:**
   - Some networks block certain ports
   - Ask IT if MQTT port 1883 is open
   - Try on different network if available

#### Can't Sign In
**Problem:** "Invalid credentials" or "Sign in failed"

**Solutions:**
1. **Check Credentials:**
   - Verify username spelling (case-sensitive)
   - Verify password spelling (case-sensitive)
   - Turn off caps lock
   - No spaces at start/end
   
2. **Contact Administrator:**
   - Account may not be created yet
   - Password may be temporary and need changing
   - Username format may be different (email vs username)

3. **Reset Password:**
   - Ask administrator for password reset
   - They should send you new temporary password
   - Try signing in with new password

#### Permissions Dialog Won't Appear
**Problem:** Camera or location permission not requested

**Solutions:**
1. **Manually Enable Permissions:**
   - Settings > Apps > OWPG > Permissions
   - Find Camera, Location, Storage
   - Enable each one

2. **Reset App Permissions:**
   - Uninstall and reinstall app
   - This triggers permission requests again

3. **Device Has Restrictions:**
   - Check if device is managed (work device)
   - Contact administrator if permissions grayed out

#### Can't Scan Barcode
**Problem:** Camera opens but won't scan, or won't open at all

**Solutions:**
1. **Check Camera Permission:**
   - Settings > Apps > OWPG > Permissions > Camera
   - Must be "Allow"

2. **Check Camera Hardware:**
   - Close app, open phone camera app
   - If camera doesn't work there, hardware issue
   - Try different device

3. **Try Manual Entry:**
   - Type barcode manually if scanning fails
   - This is acceptable backup method

4. **Restart Camera:**
   - Close scanner, wait 5 seconds, reopen
   - Restart app if still problematic
   - Restart device if issue persists

### Getting Help

If you still have issues after following this guide:

1. **Check these resources:**
   - README.md for full documentation
   - QUICKSTART.md for 5-minute tutorial
   - TROUBLESHOOTING sections in various guides

2. **Contact your administrator with:**
   - What you were trying to do
   - What error message appeared (if any)
   - Steps you've already tried
   - Device model and OS version
   - App version (usually in Settings > About)

3. **They can help with:**
   - Verifying server configuration
   - Resetting your account
   - Updating your password
   - Troubleshooting network issues

---

**Last Updated:** February 2026  
**Version:** 1.0
