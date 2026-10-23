# Watching videos on a Synology NAS (Sparklux Go)

DSM 7.2.2 no longer includes Video Station. You can still open the videos on your NAS over SMB, directly on iPhone and iPad.

## 1. Turn on SMB on the NAS

1. In DSM, open Control Panel, File Services, then the SMB tab.
2. Check "Enable SMB service" and apply.
3. Make sure the folder with your videos is a shared folder and that your user has read permission.

## 2. Add the server in the app

1. Connect the iPhone and the NAS to the same Wi-Fi.
2. In Sparklux Go, tap "Add server" on the home screen and choose SMB.
3. Enter the NAS name (for example `diskstation.local`) or IP address, then your DSM user name and password.

## 3. Tap to play

Browse the shared folder and tap a video. MKV, MP4, MOV and AVI play as they are, with subtitles and multiple audio tracks.

## If it does not connect

| Symptom | What to check |
|---|---|
| Name not found | Try the IP address. Check both devices are on the same Wi-Fi |
| Authentication fails | DSM user name and password, and that user's permission on the shared folder |
| "Require SMB3 encryption" is on | Not supported right now. Turn it off for that share or use another share |
| Away from home | You need a way into your home network (such as a VPN) |

More in the [Sparklux Go help](help.md).
