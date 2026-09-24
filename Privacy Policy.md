Privacy Policy

This Privacy Policy explains how the Sasori application collects, processes, and protects your data, as well as the developer’s stance on permissions and user transparency.
1. Data Processing and Storage
Sasori is an automation and remote-control tool designed strictly for personal use on a device you own or are authorized to manage.

No Cloud / No Developer Access: The developer does not operate any background servers, analytics engines, or telemetry systems. Your SMS messages, call logs, contacts, photos, location data, files, notifications, and configuration settings are not transmitted to the developer or to any unauthorized third-party servers.
Storage: All configuration (Telegram Bot Token, Chat ID, feature toggles, SIM preferences, etc.) is stored locally on the device using Android shared preferences. Data stays on the device unless you explicitly enable a feature that sends it to a destination you configure.
User-Directed Routing: Data is transmitted only to the destination you configure — primarily your personal Telegram bot and Chat ID. The app does not forward data until you enter valid credentials, grant the required permissions, and enable the service.

2. Transparency and Application Behavior
Sasori is designed to be transparent:

No Stealth Mode: The application cannot be hidden from the device. Its icon remains visible in the system launcher.
Background Operation: The app uses standard Android components (broadcast receivers, content observers, foreground service) to process SMS, calls, notifications, and other events according to the features you enable.
Foreground Service: When the service is enabled, Android may show a persistent notification indicating that Sasori is running. This is intentional so you remain aware that the app is active.
Telegram Control: Remote commands (e.g. /sms, /camera, /location, /ls) work only for the Chat ID you configure. Unauthorized users cannot control the device through the bot unless they have access to that chat.

3. Required Permissions and Justification
Permissions are requested so that specific features can work. They are used only for the purposes described below:
PermissionPurpose RECEIVE_SMS / READ_SMSDetect and read incoming SMS to forward them to Telegram and to show SMS history via bot commands.SEND_SMSSend SMS from the device when you reply from Telegram or use related commands. Carrier charges may apply.READ_CALL_LOGRead call history so it can be shown or forwarded via Telegram (/calls).READ_PHONE_STATE / CALL_PHONEDetect SIM state, place outgoing calls on request (/call), and support multi-SIM selection.READ_CONTACTSResolve phone numbers to contact names and support contact-related commands (/contacts).CAMERATake a photo on demand (/camera) and send it to your Telegram chat.ACCESS_FINE_LOCATION / ACCESS_COARSE_LOCATION / ACCESS_BACKGROUND_LOCATIONProvide device location via /location, including when the app is not in the foreground (if you grant “Allow all the time”).READ_EXTERNAL_STORAGE / READ_MEDIA_IMAGES / MANAGE_EXTERNAL_STORAGEBrowse gallery albums (/photos, /album), list files (/ls), and download/upload/delete files (/get_file, /upload, /del) as requested from Telegram.BIND_NOTIFICATION_LISTENER_SERVICE (Notification access)Forward app notifications to Telegram when you enable /forward_notify.INTERNETCommunicate with the Telegram Bot API to send and receive messages and media.RECEIVE_BOOT_COMPLETEDRestart the forwarding service after the device reboots, if it was enabled.FOREGROUND_SERVICE / POST_NOTIFICATIONSKeep the service running reliably and show the status notification required by Android.WAKE_LOCKBriefly keep the device awake while processing events or commands.
The app does not use these permissions for advertising, tracking, or sharing data with third parties other than the Telegram endpoint you configure.

4. What Is Sent to Telegram
Depending on which features you enable and which commands you use, the following may be sent only to your configured Chat ID:

Incoming/outgoing SMS content and metadata
Call log entries and outgoing call requests
Photos from the camera or gallery
Device location coordinates
File listings and file contents you request
App notifications (if notification forwarding is enabled)
Battery level, system info, installed apps list, and similar status data

Nothing is sent to the developer’s servers.
5. Security Notice
Because Sasori handles sensitive data (SMS, calls, location, files, notifications) and communicates over the network with Telegram, some antivirus or Play Protect heuristics may flag similar behavioral patterns. The application is intended for legitimate personal use, does not include hidden tracking or adware, and only transmits data according to the settings and commands you control.
Protect your Bot Token and Chat ID. Anyone with access to that Telegram chat can send commands to the device while the service is enabled.

6. Children’s Privacy
Sasori is not directed at children under 13 (or the equivalent minimum age in your jurisdiction). Do not use the app to collect data from children.

7. Changes to This Policy
This Privacy Policy may be updated from time to time. The latest version will be published on the project page or website. Continued use of the app after changes means you accept the updated policy.

8. Contact

GitHub: https://github.com/mirodilov/sasori
Website: https://sasori.xops.uz
Telegram: https://t.me/the_hikiman


Disclaimer: Sasori is intended for use on your own device or a device you are legally authorized to manage. Using it to monitor another person’s device without their knowledge and consent may be illegal in your country.
