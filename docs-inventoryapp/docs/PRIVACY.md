# Privacy & Data Security

Information about how the OWPG Inventory Application handles your personal data and maintains security.

## Privacy Overview

The OWPG Inventory Application collects, processes, and stores information necessary for vehicle inventory management, test drive tracking, and location monitoring. This document explains what data is collected, how it's used, and how it's protected.

## Data Collected

### User Information

**During Sign-In:**
- Username and password (verified against secure authentication server)
- Email address (if provided)
- User ID (unique identifier created on first use)
- Device ID (unique identifier of your device)
- Session token (authentication credential for your session)

**During Checkout Operations:**
- Selected action type (Test Drive, Maintenance, Relocation, etc.)
- Customer information (name, phone number) for test drives
- Vehicle beacon ID / barcode number
- Forms submitted (time, date, content)
- Any photos or videos captured
- Notes and descriptions entered

### Device Information

**Automatically Collected:**
- Device model (e.g., iPhone 14, Samsung Galaxy)
- Operating system and version
- Application version
- Device identifier (IMEI, Android ID, or equivalent)
- Network type (WiFi or cellular)

**When Location Services Enabled:**
- GPS coordinates (latitude, longitude)
- Altitude
- Speed
- Accuracy (estimated error margin)
- Timestamp of location reading
- Frequency: While using app and location is enabled

### Session Information

**Tracking Data:**
- Login timestamp and duration
- Actions taken and timestamps
- Pages visited and time spent
- Errors encountered
- Network connection status

### Photos and Videos

**When Captured:**
- Full-resolution images/videos
- Metadata (timestamp, GPS location if available)
- File size and format
- Camera settings used

## How Data is Used

### Primary Uses

1. **Vehicle Tracking**
   - Maintain accurate inventory of vehicle location and status
   - Track which vehicle is assigned to which user/customer
   - Document vehicle condition (photos)
   - Record maintenance and service history

2. **Test Drive Management**
   - Document customer information for test drives
   - Capture pre/post-drive vehicle condition
   - Track location during test drive
   - Verify licensing and insurance compliance

3. **Location Monitoring**
   - Track vehicle location in real-time
   - Maintain historical location data
   - Generate location reports
   - Assist in vehicle recovery if needed

4. **Authentication & Security**
   - Verify your identity
   - Maintain your session
   - Prevent unauthorized access
   - Audit account access

5. **System Operations**
   - Monitor app performance
   - Troubleshoot technical issues
   - Analyze usage patterns
   - Improve functionality

### Secondary Uses

- Quality assurance and training
- Dispute resolution and auditing
- Compliance with company policies
- Statistical analysis (anonymized)

## Data Retention

### Session Information

- **Duration:** Until you sign out
- **Location:** Device memory and server
- **After Sign-Out:** Retained on server for audit purposes (typically 90 days)

### Checkout Records

- **Duration:** Indefinitely (permanent record)
- **Location:** Company database and backup systems
- **Availability:** Accessible to authorized personnel

### Location Data

- **Duration:** Active during checkout operations
- **On Device:** Kept in app storage (varies by device settings)
- **On Server:** Retained per company policy (typically 6-12 months)
- **Deletion:** Can be permanently deleted per company data retention policy

### Photos/Videos

- **On Device:** Stored in app data directory, subject to device storage limits
- **On Server:** Retained as part of checkout records
- **Deletion:** Deleted when checkout records are purged

### Customer Information

- **Duration:** Stored for reference on future test drives
- **On Device:** Can be manually deleted from app settings
- **On Server:** Retained indefinitely for customer history

### User Credentials

- **Password:** Never stored in plain text
- **Stored as:** Cryptographic hash on authentication server
- **Transmission:** Always encrypted in transit

## Data Security

### Encryption

**In Transit:**
- All communication with server uses TLS 1.2+ encryption
- Barcode shown as lock icon 🔒 when secure
- Prevents eavesdropping on network
- Required even on private WiFi networks

**At Rest:**
- Passwords encrypted using industry-standard algorithms
- Session tokens are secure credentials
- Local database on device uses platform encryption
- Photos stored in encrypted app container

### Authentication

**Sign-In Process:**
1. Username and password sent via encrypted connection
2. Validated against secure authentication database
3. Session token generated and provided to app
4. Token used for subsequent requests
5. Token expires after period of inactivity (typically 8 hours)

**Session Token:**
- Unique credential per sign-in
- Automatically managed by app
- Cannot be used after sign-out
- More secure than password transmission

### Device Security

**Local Storage:**
- Data stored in app-specific directory
- OS prevents other apps from accessing
- Encrypted by device OS on modern phones
- Removed when app is uninstalled

**Permissions:**
- Camera: Required for barcode scanning and photos
- Location: Required for GPS tracking
- Storage: Required to save photos and videos
- Network: Required for server communication

### Account Security

**Best Practices:**
- ✓ Sign out when finished using app
- ✓ Do not share your password
- ✓ Do not share your device with other users
- ✓ Use strong password (8+ characters, mixed case, numbers)
- ✓ Report any suspicious activity to administrator

**Two-Factor Authentication (if available):**
- Contact administrator to enable
- Provides additional security layer
- Requires authentication device for sign-in

## Data Sharing

### Internal Sharing

**Within Your Organization:**
- Managers and supervisors: Full access to all your checkouts
- IT/Support staff: Technical access to troubleshoot issues
- Finance/Audit: Access to transaction records (anonymized)
- Authorized personnel only: Access restricted by role

**Data Shared:**
- Checkout records (action, vehicle, timestamp)
- Location data (during active checkouts)
- Photos/videos (associated with checkouts)
- Aggregated statistics (non-identifying)

### External Sharing

**Shared With Third Parties:**
- MQTT Server Provider: Vehicle and location data (configured by your organization)
- Cloud Backup Provider: Encrypted backups (if configured)
- Support Vendors: Only with explicit consent for technical support

**NOT Shared:**
- Personal contact information (without consent)
- Customer information for marketing
- Financial or payment data
- Any data with third parties not under company contract

## Your Privacy Rights

### Access Your Data

**You have the right to:**
- View your checkout history and associated data
- Request copies of your data
- See what information is stored about you
- Review your location history

**How to Request:**
- Contact your IT administrator
- Provide specific time period (if requesting subset)
- Allow 5-10 business days for response

### Correct Your Data

**You can:**
- Update your user profile information
- Correct customer data you entered (before submission)
- Request correction of errors (after submission contact administrator)

**Note:** Submitted checkouts cannot be edited but errors can be noted in follow-up records.

### Delete Your Data

**You cannot delete:**
- Submitted checkout records (legal retention required)
- Historical location data (may be required for disputes)
- System logs and audit trails

**You can delete:**
- Unsaved draft information
- Locally stored customer information
- App cache and temporary files

**How to Request Deletion:**
- Contact your IT administrator
- Specify what data to delete
- Understand retention requirements

### Opt-Out Options

**Location Tracking:**
- You can disable location services in device settings
- Disabling prevents GPS data collection
- Note: Some organizations require location tracking for vehicle management

**Photo/Video Capture:**
- You can decline permission for camera access
- Cannot perform certain operations without camera
- Use manual entry or other workarounds

**Data Collection:**
- Cannot opt-out of core data collection for inventory management
- Can limit optional data collection (detailed logging)
- Contact administrator for specific opt-out requests

## Compliance & Legal

### Data Protection Regulations

The application complies with:
- **GDPR** (General Data Protection Regulation) - If users in EU
- **CCPA** (California Consumer Privacy Act) - If users in California
- **State Privacy Laws** - As applicable
- **Company Privacy Policy** - Additional protections per organization

**If applicable to you:**
- Contact your administrator for GDPR/privacy rights
- Request Data Subject Access Request (DSAR) form
- Specify your location and applicable regulations

### Data Retention Requirements

**Legal Requirements:**
- Vehicle inventory records: Typically 7 years (tax/audit)
- Customer data: Duration of business relationship + 3 years
- Location/GPS data: 6-12 months (per company policy)
- System logs: 1-2 years (security/audit)

**Your Organization May:**
- Retain data longer for specific purposes
- Maintain backups of data (stored separately)
- Archive old data (accessible but not in active systems)

## Security Incidents

### If a Security Issue Occurs

**In Case of Data Breach:**

1. **You will be notified:**
   - Via email or app notification
   - Details of what data was affected
   - Steps you should take
   - Timeline (typically within 48-72 hours of discovery)

2. **Your organization will:**
   - Investigate the breach
   - Implement corrective measures
   - Notify relevant authorities (if required by law)
   - Provide guidance for protecting yourself

3. **You should:**
   - Change your password immediately
   - Monitor for suspicious activity
   - Report any suspicious access to administrator
   - Save any notifications for records

### Reporting Security Issues

**If you discover a security problem:**
1. Contact your IT administrator or security team immediately
2. Do not share details publicly
3. Do not test or exploit the vulnerability
4. Provide detailed information about the issue
5. Allow time for investigation and fixes

**Contact Information:**
- Administrator email: [Provided by your organization]
- IT Support: [Provided by your organization]
- Security hotline: [If available in your organization]

## Privacy Settings

### App Privacy Settings (if available)

**Location Services:**
- Settings > Location > [Vary by device]
- Options: Never, While Using, Always
- Recommended: "While Using" for app functionality

**Camera:**
- Settings > Privacy > Camera > OWPG
- Must be enabled for barcode scanning and photos
- Can be disabled if only doing manual entry

**Network Monitoring:**
- Settings > App Settings > Diagnostics
- Controls what activity is logged
- Disable to reduce data collection

**Ad Tracking (if available):**
- Settings > Ad Tracking > [Vary by device]
- OWPG app does not contain ads
- This is standard privacy control

### Device Privacy Settings

**Important Privacy Controls:**

1. **Limit Ad Tracking:**
   - iOS: Settings > Privacy > Tracking > Limit Ad Tracking
   - Android: Settings > Privacy > Ads > Opt out of Personalized Ads
   - Note: Does not affect OWPG app

2. **Location Privacy:**
   - Disable for non-essential apps
   - Allow OWPG only for inventory purposes

3. **Camera Privacy:**
   - Only OWPG uses camera in this app
   - Disable camera permission if not needed

4. **Storage Access:**
   - OWPG can access only its dedicated directory
   - Cannot see other apps' files

## Questions About Privacy

### FAQ - Privacy & Security

**Q: Is my password stored securely?**
A: Yes. Passwords are hashed (encrypted) and cannot be recovered by anyone, including administrators. To reset, you must go through authentication process.

**Q: Can my manager see my photos?**
A: Your manager can see photos associated with checkouts you submit. Unsaved photos on your device are private.

**Q: How long is location data kept?**
A: Typically 6-12 months. Check your company's specific retention policy with your administrator.

**Q: Can I delete submitted checkout records?**
A: No. Submitted checkouts become permanent records for accounting and audit purposes. Contact administrator if you need a correction noted.

**Q: Is my data backed up?**
A: Yes. Company maintains secure backups. If device is lost, you can sign in on another device and continue. Local backup retention varies.

**Q: Can I use the app offline?**
A: Limited offline capability exists (viewing local records). Submitted data requires internet to transmit. Data is stored locally until sent.

**Q: What happens to my data if I'm terminated?**
A: Your account access is disabled. Your data remains in company records per retention policies. Contact HR for specific details.

**Q: Is my data encrypted on my device?**
A: Yes. Device OS provides encryption. Data is also stored in app-specific encrypted container.

**Q: Can I request a copy of all my data?**
A: Yes. This is your right under many privacy laws. Contact your IT administrator to request Data Subject Access Request (DSAR).

**Q: Who can access my checkout history?**
A: Authorized personnel only (managers, supervisors, IT support). Access is logged and audited.

**Q: Is the app secure if I'm on public WiFi?**
A: Yes, because all data uses TLS encryption. However, avoid signing in on untrusted networks when possible.

### Contact Privacy Officer

**For Privacy Questions:**
- Contact your IT department
- Request to speak with Privacy Officer or Compliance team
- Email privacy@[your-company].com (if available)
- Allow 5-10 business days for response

## Glossary

- **Encryption:** Converting data into code to prevent unauthorized access
- **TLS:** Transport Layer Security, encryption standard for internet communication
- **Hash:** One-way encryption that cannot be reversed (used for passwords)
- **Metadata:** Information about data (timestamp, location, file type)
- **GDPR:** EU regulation on data protection and privacy
- **CCPA:** California law on data privacy
- **DSAR:** Data Subject Access Request, your right to see your data
- **Retention:** How long data is kept
- **Breach:** Unauthorized access to protected data

---

**Last Updated:** February 2026  
**Document Version:** 1.0  
**Review Recommended:** Annually or after policy changes
