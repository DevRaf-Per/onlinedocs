# Barcode Scanning Guide

Complete guide to scanning vehicle barcodes and beacon IDs using the OWPG Inventory Application.

## Understanding Vehicle Barcodes

### What is a Vehicle Barcode?

Your vehicle's barcode (also called "Vehicle Beacon ID" or "Barcode") is a unique identifier assigned to each vehicle in your inventory. This barcode links all checkout activities to the specific vehicle, ensuring proper tracking and accountability.

### Barcode Format

- **Type:** Linear barcode (1D barcode like Code 128)
- **Length:** Typically 16+ characters
- **Content:** Company prefix + vehicle number + checksum
- **Example:** `[PREFIX]001234567890[CS]`

**What the App Extracts:**
- If barcode is longer than 16 characters, the app extracts characters 4-16 (12-character code)
- If barcode is shorter than 16 characters, the entire barcode is used
- The extracted code is what's stored in the system

### Where is the Barcode?

Vehicle barcodes are typically located on:
- **Dashboard:** Mounted on passenger side of windshield
- **Door Jamb:** On the driver's side door
- **Bumper Sticker:** Front or rear bumper
- **VIN Plate:** Sometimes near the VIN number

Contact your administrator if you cannot locate a barcode on a vehicle.

## Methods of Entering a Barcode

### Method 1: Camera Scanner (RECOMMENDED)

The camera scanner provides fast, accurate barcode reading without manual typing.

#### Prerequisites

- Device with camera (smartphone, tablet, or Windows laptop with webcam)
- Camera permissions enabled for the OWPG app
- Good lighting (natural or bright artificial light)
- Barcode not damaged or obstructed

#### Step-by-Step Camera Scanning

1. **Prepare Your Device**
   - Ensure good lighting
   - Clean camera lens with soft cloth
   - Remove protective case if it blocks camera
   - Unlock device

2. **Navigate to Vehicle Beacon ID Field**
   - Complete the form up to "Vehicle Beacon ID" field
   - Locate the **Camera Icon** button next to the text field
   - (On some screens, you may need to scroll to find it)

3. **Open Camera Scanner**
   - Tap the **Camera Icon** button
   - App will request camera permission (grant if prompted)
   - Camera view will open with:
     - Live preview of what the camera sees
     - A scanning frame or crosshair in the center
     - Instructions or countdown (varies by device)

4. **Position the Barcode**
   - Slowly move your device toward the barcode
   - Center the barcode in the scanning frame
   - Keep the device steady and level
   - Optimal distance: 6-12 inches from barcode
   - Angle: Perpendicular to barcode (not at an extreme angle)

5. **Wait for Detection**
   - App automatically scans continuously
   - When barcode is detected, the app will:
     - Highlight the barcode in yellow
     - Play a beep sound (if enabled)
     - Display the barcode value in the scanner
   - Do not move device after detection - let app process

6. **Confirm the Scan**
   - Barcode value will appear at bottom of scanner view
   - Review that the value is correct
   - The scanner will auto-close after ~1 second
   - You'll return to the main form with barcode filled in

7. **Verify the Entry**
   - Check that the barcode value in the field matches what you scanned
   - If incorrect, clear field and try scanning again
   - If scanner failed, use manual entry method

#### Camera Scanning Tips for Success

**Lighting Conditions:**
- ✓ **Ideal:** Natural daylight or bright indoor lighting
- ✗ **Avoid:** Direct shadows, backlighting, low light
- ✗ **Problem:** Very shiny or reflective barcode surfaces
- **Solution:** Angle your device to reduce glare

**Barcode Positioning:**
- ✓ **Ideal:** Barcode straight and level in camera view
- ✓ **Ideal:** Entire barcode visible in frame
- ✗ **Avoid:** Scanning at extreme angles
- ✗ **Avoid:** Partially off-screen barcodes
- **Solution:** Move closer or farther to frame entire barcode

**Device Stability:**
- ✓ **Ideal:** Steady hand or device on surface
- ✗ **Avoid:** Shaky or moving camera
- **Solution:** 
  - Lean device against stable object
  - Use both hands to stabilize
  - Rest wrist on vehicle or table

**Barcode Condition:**
- ✓ **Ideal:** Clear, undamaged barcode
- ✗ **Problem:** Faded, damaged, or dirty barcode
- ✗ **Problem:** Barcode partially covered
- **Solution:**
  - Clean barcode carefully with soft cloth
  - Use flashlight to illuminate
  - Try scanning from different angle
  - If still unreadable, use manual entry

**Distance and Focus:**
- **Too Close:** Barcode is blurry or only part visible
  - Solution: Move device 3-4 inches away
- **Too Far:** Barcode is too small to read
  - Solution: Move device closer
- **Out of Focus:** App is not focusing on barcode
  - Solution: Tap barcode area on screen (on some devices)

### Method 2: Manual Text Entry

Use manual entry when camera scanning is unavailable or unsuccessful.

#### Step-by-Step Manual Entry

1. **Access the Field**
   - Locate the "Vehicle Beacon ID" text field
   - Tap directly on the text field (not the camera button)

2. **Enter the Barcode**
   - Type the barcode value
   - Or paste from clipboard if you have it copied:
     - On Windows: Ctrl+V
     - On iOS: Long-press > Paste
     - On Android: Long-press > Paste
   - Barcode should be 12+ characters

3. **Verify Entry**
   - Check that value matches the barcode you're referring to
   - Look for typos or missing digits
   - Compare to barcode on vehicle if possible

4. **Continue**
   - Proceed with rest of form
   - Submit as normal

#### Transcribing a Barcode Accurately

If you need to type the barcode:

1. **Read Carefully**
   - Examine barcode closely
   - Some characters look similar (e.g., 0 vs O, 1 vs I, 5 vs S)
   - Use the barcode itself as reference, not memory

2. **Split Into Chunks**
   - Break 12-character code into 3-character chunks: ABC-DEF-GHI-JKL
   - Easier to verify and less prone to error
   - Enter each chunk, then combine

3. **Double-Check**
   - After typing, compare to original barcode
   - Verify:
     - First 3 characters
     - Middle 6 characters
     - Last 3 characters
   - Correct any errors before submitting

4. **When Unsure**
   - Take a photo of barcode and reference it
   - Ask coworker to verify
   - Check vehicle documentation for barcode

### Method 3: Barcode Database Lookup

Some organizations may provide a searchable database of barcodes.

#### Using Barcode Lookup

1. **Access Lookup Tool** (if available)
   - Within app: Tap the lookup icon (varies by version)
   - Or check your organization's intranet

2. **Search by Vehicle**
   - Search by license plate
   - Search by VIN
   - Search by vehicle name/model
   - View associated barcode

3. **Copy and Use**
   - Select the barcode from results
   - Automatically copies to clipboard
   - Return to form and paste

## Troubleshooting Scanner Problems

### Camera Won't Open

**Symptoms:** Tap camera button, nothing happens or error appears

**Solutions:**
1. **Check Permissions:**
   - iOS: Settings > OWPG > Camera > Enable
   - Android: Settings > Apps > OWPG > Permissions > Camera > Allow
   - Windows: Settings > Privacy > Camera > Ensure OWPG is allowed

2. **Restart App:**
   - Close the app completely
   - Wait 5 seconds
   - Reopen and try again

3. **Restart Device:**
   - Power device off and on
   - This refreshes permission system

4. **Clear App Cache:**
   - Settings > Apps > OWPG > Storage > Clear Cache
   - Try again

5. **Reinstall App:**
   - Uninstall OWPG
   - Download and install latest version
   - Re-grant all permissions

**If Still Not Working:**
- Use manual entry method instead
- Contact your IT administrator

### Scanner Opens But Won't Detect Barcode

**Symptoms:** Camera view works but barcode is not detected/highlighted

**Solutions:**

1. **Check Lighting:**
   - Move to brighter location
   - Use flashlight to illuminate barcode
   - Avoid shadows
   - Try different angle to reduce glare

2. **Check Barcode Condition:**
   - Clean barcode with soft cloth
   - Ensure barcode is not torn or faded
   - Check if barcode is fully visible (not partially covered)

3. **Adjust Distance:**
   - Barcode may be too close (blurry)
   - Barcode may be too far (too small)
   - Try 6-12 inch range
   - Adjust slowly until it detects

4. **Check Camera Focus:**
   - Tap the barcode area on screen (some devices)
   - Let camera auto-focus for 2-3 seconds
   - Keep steady while waiting

5. **Try Different Angle:**
   - Scan barcode straight (perpendicular to surface)
   - Avoid scanning at extreme angles
   - Rotate slightly if detection fails

6. **Different Device:**
   - Try scanning with different phone/tablet
   - Different camera sensors may work better
   - Compare results to troubleshoot

7. **If Barcode is Unreadable:**
   - Use manual entry method
   - Note in comments that barcode was unreadable
   - Contact administrator to update barcode

### Scanner Keeps Beeping/Vibrating

**Symptoms:** Multiple detections or continuous alerts

**Cause:** Scanner detected barcode multiple times or sensitivity is too high

**Solution:**
1. Move away from barcode after first detection
2. Do not move device back over barcode
3. Let app auto-close (happens automatically)
4. If app doesn't close automatically, tap back button
5. Scanner is functioning normally - this is expected behavior

### Scanner Closed/Closed Too Soon

**Symptoms:** Scanner closed before getting good reading

**Cause:** Accidental tap or unstable detection

**Solution:**
1. Tap camera button again
2. Hold device steady
3. Keep barcode in view longer (2-3 seconds)
4. Use manual entry as backup

## Best Practices for Barcode Scanning

### Everyday Scanning Tips

- ✓ **Clean regularly:** Wipe camera lens daily with soft cloth
- ✓ **Check lighting:** Ensure adequate light before attempting scan
- ✓ **Verify result:** Always check that scanned value is correct
- ✓ **Know location:** Learn where each vehicle's barcode is positioned
- ✓ **Document issues:** Note if barcode is damaged or hard to read

### Efficient Workflow

- **Scan immediately:** Scan barcode right after selecting action, before other fields
- **Have backup:** Keep manual entry ready if scanner fails
- **Batch checkouts:** Group multiple same-vehicle checkouts to reuse barcode (copy from history)
- **Use clipboard:** Copy barcode for similar vehicles to speed entry

### Maintaining Barcodes

- Report damaged barcodes to your administrator
- Request replacement barcodes for faded or illegible ones
- Clean barcodes monthly to maintain readability
- Protect barcodes from harsh sun exposure (UV can fade)

## Barcode Format Variations

Different organizations may use different barcode formats. Common formats include:

### Code 128 (Most Common)
- Alphanumeric barcode (letters and numbers)
- Efficient encoding
- Works with standard scanners

### Code 39
- Alphanumeric format
- Thicker bars than Code 128
- Good durability

### EAN-13 / UPC-A
- 13-digit numeric (EAN) or 12-digit (UPC)
- Commonly used in retail
- May require special scanning

### QR Codes (Modern Alternative)
- 2D barcode (square with patterns)
- Can encode more data
- More resistant to damage
- Requires smartphone camera
- Better in poor lighting

**Your App:** The OWPG app supports 1D linear barcodes (Code 128, Code 39, etc.). For other formats, contact your administrator.

## Advanced Scanning Scenarios

### Multiple Barcodes on Same Vehicle

**Situation:** Vehicle has multiple barcodes (windshield, door, bumper)

**Solution:**
- Use any visible barcode (all point to same vehicle)
- Choose most accessible one for efficiency
- If barcodes differ, contact administrator (possible data issue)

### Barcode Not Found on Vehicle

**Situation:** Vehicle has no visible barcode or barcode is missing

**Action Items:**
1. Check common locations:
   - Windshield
   - Door jamb
   - Bumper
   - Dashboard
2. Contact your supervisor
3. Use VIN as temporary identifier (if allowed)
4. Note the issue for administrator to investigate
5. Request new barcode if original is lost

### Reading Faded Barcode

**Situation:** Barcode is faded or worn and hard to read

**Solutions:**
1. **Try camera scanner first:**
   - Cameras sometimes detect faded barcodes better
   - Use good lighting and try multiple angles

2. **If Scanner Fails:**
   - Look carefully at barcode
   - Identify each digit/character
   - Use manual entry method carefully
   - Have coworker verify

3. **Report Issue:**
   - Document that barcode is faded
   - Take photo and send to administrator
   - Request barcode replacement

## FAQ - Barcode Scanning

**Q: Is camera scanner faster than manual entry?**
A: Yes, typically 3-5 times faster for experienced users. In good conditions, scanning takes 5-10 seconds vs. 20-30 seconds for manual typing.

**Q: What if I scan the wrong barcode?**
A: Clear the field and scan again, or manually correct the value. Always verify the scanned value before submitting.

**Q: Can I save frequently-used barcodes?**
A: Some versions of the app may have a favorites feature. Check your app's settings or contact your administrator.

**Q: What if barcode is laminated and reflective?**
A: Angle your device to reduce glare. Try scanning from slightly different positions. If still problematic, use manual entry.

**Q: Can I use barcode scanner hardware with the app?**
A: Some devices support Bluetooth barcode scanners. Check with your administrator. The app will treat hardware scanner input as text entry.

**Q: Is there a minimum/maximum barcode length?**
A: The app extracts 12 characters from barcodes. Minimum 12 characters recommended. Very long barcodes (20+ characters) have the middle characters extracted.

**Q: What if I have vision issues and can't read small barcode?**
A: Use device magnification (zoom) to enlarge barcode before scanning. Or use manual entry if barcode data is available elsewhere.

---

**Last Updated:** February 2026  
**Document Version:** 1.0
