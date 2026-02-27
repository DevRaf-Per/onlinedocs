
InventoryApp — End-user Guide

Overview

InventoryApp is a mobile app for Android and iOS that lets staff check out and return inventory items, capture customer details for test drives, scan item IDs, and track trips while items are checked out.
> **This file has been superseded.**  The primary user guide is now located at `docs/UserGuide.md`.

> Please open that document for the most up-to-date instructions.

Before you start

- Device running Android or iOS.
- Network access (Wi‑Fi or cellular) for communicating with the backend.
- Camera permission (to scan tags and take photos) and location permission (for trip tracking) when using those features.

Install and first run

- Install the app from your organization’s distribution channel or have IT install it.
- On first launch grant requested permissions (camera, location, storage) so scanning, trip tracking, and file export work correctly.
- Sign in with the credentials provided by your organization if prompted.

Main tasks (quick start)

1. Sign in if required.
2. Scan an item or type its ID into the Item field.
3. Choose an action (for example: Test Drive, Maintenance, Relocation, Transfer, Service Test, Other).
4. If you choose Test Drive, enter the customer's name and contact details when prompted.
5. Tap Submit to check the item out. Wait for the confirmation message before leaving the app or driving away.
6. While the item is checked out, the app may track the trip in the background (if you allowed location access).
7. When the item is returned, tap Return. Wait for the confirmation message before closing the app.

Scanning

- Use the Scan button to open the scanner and scan barcodes/QR codes. The app will request camera permission if needed.
- If the camera permission is denied, follow the prompt to open app settings and enable the camera permission.

Test drive flow

- Selecting Test Drive opens a popup asking for customer name, phone number, number of passengers, and whether license/insurance were provided.
- You can optionally capture customer license and insurance photos if the app prompts for it.
- If photos are taken and the organization requires them, the app may send them to the appropriate contact when you submit.

Submitting and returning items

- Submit: publishes a checkout request and waits for a confirmation. If confirmation is received, the app disables checkout controls and shows the return view.
- Return: publishes a checkin request and waits for a confirmation. If confirmation is received, the app clears the checkout state and may send recorded trip data.

Permissions and privacy

- Camera: required for scanning and taking photos.
- Location: required if the app needs to track trips while an item is checked out.
- Storage: used for saving trip logs and photos.
- Customer details and photos are stored on-device. Do not export or share sensitive customer data unless authorized by your organization.

Viewing messages and status

- The app displays incoming messages and status updates in the message area or carousel on the main screen.
- Pay attention to success or error popups after submitting or returning items.

Troubleshooting

- Cannot sign in or stay authenticated: sign out and sign back in. If the problem persists, contact IT with your User ID and the app version.
- Cannot connect or actions fail: verify network connectivity and try again. If the issue continues, contact IT.
- Scanner does not open: check camera permission in your device settings and grant it if necessary.
- Location tracking not working: check location permission and that location services are enabled on your device.

Best practices

- Always wait for a success confirmation before leaving the item or ending a session.
- If prompted for customer photos, confirm you have permission to collect and share those images.
- Sign out when finished if your device is shared.

Getting help

- If you need assistance, contact your organization's support team and provide:
  - A short description of the problem
  - Device type and OS version (Android/iOS)
  - App version (if shown in the app)

Privacy

- The app stores customer names, phone numbers, photos, and trip logs locally on the device. Treat this data in accordance with your organization’s privacy and data-handling policies.

This guide focuses on the day-to-day use of the app. For further assistance, contact your IT or support team.

