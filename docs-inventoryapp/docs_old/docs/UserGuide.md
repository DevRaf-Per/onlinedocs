# InventoryApp End-User Guide

This document is intended for the people who actually use the mobile application on a daily basis.  It explains how to install, sign in, and perform the most common tasks.

> **Note:** The file `INVENTORYAPP_USER_GUIDE.md` at the project root is kept for compatibility with older distributions.  Please consult this copy instead.

## Table of Contents

1. [Overview](#overview)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Quick Start](#quick-start)
5. [Scanning](#scanning)
6. [Test Drive Flow](#test-drive-flow)
7. [Submitting and Returning Items](#submitting-and-returning-items)
8. [Messages and Status](#messages-and-status)
9. [Permissions & Privacy](#permissions--privacy)
10. [Troubleshooting](#troubleshooting)
11. [Getting Help](#getting-help)
12. [Best Practices](#best-practices)

## Overview

InventoryApp is a cross‑platform mobile application (Android and iOS) used by field staff to check items in and out, record customer details for test drives, track trips, and communicate status messages with a backend system.

## Prerequisites

* A supported Android or iOS device.
* Network connectivity (Wi‑Fi or cellular) to communicate with the service.
* Permissions: camera (scanning/photos), location (trip tracking), and storage (saving logs/photos).

## Installation

The app is deployed by your organization via its chosen distribution mechanism (internal app store, deployment tool, or mobile device management).  Ask your IT department if you are unsure where to obtain the latest version.

1. Install the application on your device.
2. When launching for the first time, grant the requested permissions so the scanner, camera, and location tracking work correctly.
3. Sign in with the username/password supplied by your organisation, if prompted.

## Quick Start

1. **Sign in** (if required).
2. On the main screen enter or scan an item ID and select an action from the dropdown.
3. If the action is **Test Drive**, enter the customer’s name, phone number, passenger count and optionally capture license/insurance photos.
4. Tap **Submit** to check the item out; wait for the success message.
5. If the item remains checked out, the app may track the trip in the background (location permission required).
6. To return the item, tap **Return** and again wait for confirmation before closing or leaving the app.

## Scanning

* Tap the **Scan** button to open the barcode/QR scanner.  The camera permission is requested if not already granted.
* If permission is denied, the app will prompt you to open the system settings and enable the camera manually.

## Test Drive Flow

When you choose **Test Drive** as the action:

* A form appears asking for customer details and optional photo attachments.
* You may be required by your organisation to take pictures of the customer's license and insurance.
* Pictures are stored locally and submitted with the request if required.

## Submitting and Returning Items

* **Submit**:
  * Sends a checkout request to the backend.
  * The controls are disabled once a successful response is received and the view switches to the return mode.

* **Return**:
  * Sends a check‑in request and clears the checkout state on success.
  * Trip data (if collected) may be uploaded at this point.

## Messages and Status

Incoming messages or status updates from the server appear in the message area or the carousel on the main screen.  Always watch for success or error pop‑ups after submissions.

## Permissions & Privacy

* **Camera** – scanning and taking photos.
* **Location** – required for trip tracking.
* **Storage** – used to save trip logs and customer photos.

Customer information (names, phone numbers, photos, trip logs) is stored locally.  Do not export or share sensitive data unless authorised by your organisation.

## Troubleshooting

* **Sign‑in problems**: sign out and sign back in; contact IT with your user ID and app version.
* **Connectivity issues**: ensure the device has network access; restart the app if necessary.
* **Scanner does not start**: verify camera permission in system settings.
* **Location tracking inactive**: check location permission and that location services are enabled on the device.

## Getting Help

If you experience an issue that isn’t covered here, contact your organisation’s support team with the following information:

1. A brief description of the problem.
2. Device type and operating system.
3. App version (displayed in the app if available).

## Best Practices

* Wait for confirmation before leaving the item or closing the app.
* Capture and submit photos only if you have permission to do so.
* Sign out if you are using a shared device.
