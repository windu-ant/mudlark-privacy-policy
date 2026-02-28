# MUDlark Privacy Policy

**Last Updated:** February 28, 2026

**App Name:** MUDlark  
**Bundle ID:** dbi.MUDlark  
**Developer:** Tony Mace

---

## Overview

MUDlark is a MUD (Multi-User Dungeon) client for iOS that connects to third-party MUD game servers. We are committed to protecting your privacy. This policy explains what data the app collects, how it is used, and your rights regarding that data.

---

## Data Collection & Usage

### Data Stored on Your Device Only

The following data is stored locally on your device and is **never transmitted** to us:

- **World/Server Configurations** — Saved MUD server addresses, ports, and connection preferences (stored in UserDefaults).
- **Triggers, Aliases, and Timers** — Automation rules you create, stored per-world in UserDefaults.
- **App Settings** — Preferences such as font size, font family, input options, joystick configuration, and display settings (stored in UserDefaults).
- **Session Logs** — If you enable auto-logging, session transcripts are saved as text files on your device. These logs never leave your device unless you explicitly share or export them.
- **Command History** — Recent commands you have entered during a session, stored locally.
- **Scrollback Buffer** — Text received from MUD servers is held in memory during your session and is not persisted after the app is closed (unless logging is enabled).

### Data Stored in the iOS Keychain

- **Cryptographic Signing Key** — An Ed25519 private key used for authentication with the optional MUDlark proxy server. This key is generated on your device and stored securely in the iOS Keychain. It is never transmitted; only the corresponding public key is shared with the proxy server during registration.

### Data Associated with Your Identity

- **User ID** — A randomly generated UUID created on first launch. This ID is used solely to identify your device when connecting to the optional MUDlark proxy server. It is not linked to your name, email, Apple ID, or any other personally identifiable information.

---

## Optional Proxy Server

MUDlark offers an optional proxy relay server that maintains your MUD connection when the app is backgrounded or suspended by iOS. If you choose to use this feature:

### Data the Proxy Server Processes

- **MUD Traffic** — Text sent between you and the MUD server is relayed through the proxy. This data exists **only in memory** and is buffered temporarily until delivered to your device. It is **not logged or stored persistently** on the server.
- **Connection Metadata** — The server records your User ID and timestamps for connection and disconnection events for operational purposes (e.g., debugging connection issues).

### Data the Proxy Server Does NOT Collect

- No message content or MUD session data is logged or stored on disk.
- No IP address logging beyond standard server access patterns.
- No analytics, tracking, or profiling of user behavior.
- No advertising identifiers or third-party tracking SDKs.

---

## Third-Party MUD Servers

When you connect to a MUD game server (directly or via the proxy), your data is transmitted to that third-party server. Each MUD server has its own privacy practices, which are outside our control. We recommend reviewing the privacy policy of any MUD server you connect to. MUDlark does not control, monitor, or log your interactions with third-party MUD servers.

---

## Data Sharing

We do **not** sell, share, rent, or trade your personal data with any third parties. No data is shared with advertising networks, analytics providers, or data brokers.

---

## Analytics & Tracking

MUDlark does **not** include any analytics frameworks, crash reporting services, or third-party tracking SDKs. We do not collect usage statistics, device information, or behavioral data.

---

## Notifications

MUDlark may request permission to send local notifications. These notifications are generated entirely on your device (e.g., trigger-based alerts, connection timeout warnings) and do not involve any external notification service beyond Apple Push Notification service (APNs) when used with the optional proxy server for push notifications.

---

## Data Retention

- **On-device data** (settings, triggers, logs) persists until you delete the app or manually clear the data.
- **Proxy server connection metadata** (User ID, connect/disconnect timestamps) is retained for operational purposes.
- **Proxy server MUD traffic buffer** is held in memory only and is discarded once delivered or when the session ends.

---

## Data Deletion

- **On-device data:** Uninstalling MUDlark removes all locally stored data, including UserDefaults, Keychain entries, and session logs.
- **Proxy server data:** You may request deletion of your User ID and associated connection metadata by contacting us at the email below. You can also reset your proxy identity within the app, which generates a new User ID and cryptographic key.

---

## Security

- Cryptographic keys are stored in the iOS Keychain with `kSecAttrAccessibleAfterFirstUnlock` protection.
- Proxy server connections use WebSocket over TLS (WSS) with JWT-based authentication using Ed25519 challenge/response signing.
- Direct MUD connections use TCP; TLS is available on a per-world basis where supported by the MUD server.

---

## Children's Privacy

MUDlark is not directed at children under the age of 13. We do not knowingly collect personal information from children. If you believe a child has provided data through the app, please contact us so we can take appropriate action.

---

## Changes to This Policy

We may update this privacy policy from time to time. Changes will be reflected by the "Last Updated" date at the top of this document. Continued use of the app after changes constitutes acceptance of the updated policy.

---

## Your Rights

Depending on your jurisdiction, you may have the right to:

- Access the personal data we hold about you.
- Request deletion of your data.
- Opt out of any data processing (though MUDlark processes minimal data by design).

---

## Contact

If you have questions or concerns about this privacy policy or your data, please contact:

**Email:** [mudlarkmudclient@gmail.com]

---

*This privacy policy applies to the MUDlark iOS application (bundle ID: dbi.MUDlark) available on the Apple App Store.*
