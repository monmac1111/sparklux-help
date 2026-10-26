# Privacy Policy — Sparklux Go (iPhone / iPad)

**Last updated: 2026-10-26**

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
| Imported LUT (.cube) files and your choice | App storage on the device | To apply them to the picture. Only a copy of the file you chose; nothing is written to its original location |
| Counts used for the rating request (videos watched to the end, first-launch date, date of the last request) | App storage on the device | To decide when to show the App Store rating request. Never sent anywhere |
| Subtitle, Picture in Picture, sort and display settings | App storage on the device | To keep your settings |
| Paired Sparklux Library on your Mac (display name, key fingerprint, addresses to connect to) | App storage on the device | To reconnect quickly |
| This device's key for the link | **Secure Enclave** (the device keychain on devices without one) | To prove to the paired Mac that it is this device. Never leaves the device |
| Values used to open a library you chose to “Remember with Face ID” | **The device keychain** (protected by Face ID / Touch ID; this device only) | To open it without typing the password each time. The password itself is not stored |
| Temporary copies of videos chosen from Photos (up to 20, 10GB total) | App storage on the device (excluded from backups; the oldest are removed automatically) | To play them |

This is removed when you delete the app (keychain items may remain, as the system decides).

For a **password-protected library** in Sparklux Library on your Mac, its contents (titles, thumbnails, playback positions, tags and so on) are kept in memory only while it is open and are never saved on the device. They are discarded when you close the app or it goes to the background.

## 3. Photos and camera

The app reads **only the video you choose**. It does not ask for access to your whole photo library.

The camera is used only to scan the QR code shown by Sparklux Library on your Mac. No photos or videos are taken or saved.

## 4. Scope of network traffic

The app connects only to **servers you register yourself** (SMB, WebDAV, Jellyfin, DLNA/UPnP), to **Sparklux Library on your own Mac, paired with a QR code**, and to **URLs you type in**. It never sends anything to a server run by the developer.

- You can connect not only to servers on your home network but also to servers outside it, over HTTPS (WebDAV, Jellyfin, URLs)
- Unencrypted traffic: SMB (when you connect to a server that does not require encryption), http WebDAV/Jellyfin/DLNA-UPnP, and http URLs. These only mean the traffic itself is not encrypted — the destination is still the one you chose
- Local network access is used to find these servers and Sparklux Library on your Mac on the same Wi-Fi
- The app talks directly to Sparklux Library on your Mac, encrypted with the keys of the paired devices. From outside your home it connects only if you turn on “Allow access from outside your home” on the Mac, or through a VPN you use yourself (such as Tailscale). The app does not include a VPN

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
| Browsing and playing Sparklux Library on your Mac | Reading the library list, thumbnails and videos; recording playback positions on the Mac; the password for a password-protected library when you open it (not kept on the device after sending) | Your own Mac, paired with a QR code |
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
