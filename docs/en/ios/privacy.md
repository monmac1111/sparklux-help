# Privacy Policy — Sparklux Go (iPhone / iPad)

**Last updated: 2026-10-01**

This policy describes how Sparklux Go for iPhone / iPad ("the app") handles information.

## 1. Information we do not collect

**The app never collects or sends:**

- the **content** of videos you play
- video **file names, folder names or locations**
- **viewing history**
- contact details such as your name, email address or phone number
- **location**
- identifiers that track you across devices

The app contains no analytics, no advertising SDK and no crash-report upload. The developer runs no server.

## 2. Information stored only on your device

The following stays **on your iPhone / iPad only** and is never sent anywhere.

| Information | Where | Why |
|---|---|---|
| Servers you add (name, host name, user name, last share and folder) | App storage on the device | To reconnect quickly |
| **Passwords** for SMB and WebDAV | **The device keychain** (this device only; not synced to iCloud Keychain) | To reconnect quickly. You can choose not to save it |
| Jellyfin **sign-in token** (no password is stored) | **The device keychain** (this device only) | To reconnect quickly |
| References to folders you add from the Files app | App storage on the device | To reopen the same folder |
| Resume positions and watched marks (up to 1000 combined) | App storage on the device | To resume playback and show what you've watched |
| Favorites | App storage on the device | To show them on the home screen |
| Thumbnails (small previews of videos) | Device cache | To show them quickly in lists |
| Subtitle, Picture in Picture, sort and display settings | App storage on the device | To keep your settings |
| Temporary copies of videos chosen from Photos (up to 20, 10GB total) | App storage on the device (excluded from backups; the oldest are removed automatically) | To play them |

This is removed when you delete the app (keychain items may remain, as the system decides).

## 3. Photos

The app reads **only the video you choose**. It does not ask for access to your whole photo library.

## 4. Scope of network traffic

The app connects only to **servers you register yourself** (SMB, WebDAV, Jellyfin, DLNA/UPnP) and to **URLs you type in**. It never sends anything to a server run by the developer.

- You can connect not only to servers on your home network but also to servers outside it, over HTTPS (WebDAV, Jellyfin, URLs)
- Unencrypted traffic: SMB (when you connect to a server that does not require encryption), http WebDAV/Jellyfin/DLNA-UPnP, and http URLs. These only mean the traffic itself is not encrypted — the destination is still the one you chose
- Local network access is used to find these servers on the same Wi-Fi

## 5. Purchases

Purchases and the free trial are handled by **Apple (App Store)**. The app never receives or stores payment details.

- The 3-day free trial is a zero-price App Store item; **Apple records the start date**
- Whether you have purchased, and how much of the trial is left, is decided on the device from Apple-signed transactions
- You are never charged automatically

## 6. Network traffic

The app connects only in these cases.

| Traffic | What | To |
|---|---|---|
| Opening a shared folder / playing | Sign-in and reading the video | The server you registered (SMB, WebDAV, Jellyfin, DLNA/UPnP) |
| Opening a URL | A request to the URL you entered | Where you pointed it |
| Purchase, trial, restore | Processing and verifying the transaction | Apple |

## 7. Children's privacy

The app does not knowingly collect information from children under 13 (it collects personal information from no one).

## 8. Changes

If this policy changes, this page and the "Last updated" date will be updated. Significant changes will also be noted in the app's release notes.

## 9. Contact

<hello@monneural.dev>

---

Operator: mon neural (Fumiaki Monma)
