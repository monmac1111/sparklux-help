# Help — Sparklux Go (iPhone / iPad)

**SDR video, at HDR brightness.** Browse the folders on your Mac or NAS and play videos directly.

## Requirements

- iOS / iPadOS 26 or later
- **An HDR-capable screen** (iPhone 12 or later, iPad Pro, etc.). Videos still play on other screens, but SDR-to-HDR conversion does not run (the app tells you so)

## Open a shared folder on your Mac

1. **On the Mac**: System Settings › General › Sharing › turn on **File Sharing** and add the folders you want to share
2. **In the app**: tap your Mac under **Network** (if it does not appear, use **Add Server** and type its host name or IP address)
3. Enter your Mac user name and password, then **Connect**

!!! note "If you are asked about Local Network the first time"
    Tap **Allow**. The first attempt right after allowing may fail once — just tap **Connect** again.
    If you declined, turn on Sparklux Go in Settings › Privacy & Security › Local Network.

NAS devices (Synology, QNAP, etc.) work over SMB too. **Shares that require SMB3 encryption are not supported yet.**

## Other ways to open videos

| Source | How |
|---|---|
| A folder in the Files app | **Add Folder** — browse it again next time |
| A single file | **Open File** |
| Photos | **Choose from Photos** (HDR recordings stay as they are) |
| URL | **Open URL** — direct links to video files (.mp4 / .mov / .m3u8) |

!!! warning "Streaming services such as YouTube cannot be opened"
    Their video pages are not video files, so they cannot be played.

## Supported formats

MP4 / MOV / M4V / HLS (.m3u8) / **MKV**. H.264 and HEVC video (including 10-bit, HDR10, HLG and Dolby Vision 8.1).

- For MKV, only the default audio track plays. MKV embedded subtitles are planned for a future update
- Dolby Vision Profile 5 cannot be shown in correct colours (the app tells you so)

## Controls while playing

The screen is split into left, middle and right thirds. What happens depends on where you tap.

![Screen controls: left, middle and right thirds, and swipe down](../../assets/ios-gestures-en.svg)

| Gesture | Action |
|---|---|
| Tap the middle | Play / pause. While paused, the controls stay on screen |
| Tap the left or right | Show / hide the controls |
| Double-tap the left | Back 10 seconds (keep tapping for 20, 30…) |
| Double-tap the right | Forward 10 seconds (keep tapping for 20, 30…) |
| Touch and hold (anywhere) | 2× speed while you hold. Back to normal when you let go (while playing) |
| Swipe down | Closes the player. Pull about a fifth of the screen, or flick quickly. If not far enough, it springs back (does not start on the controls or near the A/B divider) |

The **controls** have a seek bar, back / forward 10 seconds, play / pause, ✨ (Picture) and × (close).

## Picture settings

Tap ✨ to open the picture settings.

| Setting | What it does |
|---|---|
| **Natural** (default) | Natural brightness. Hard to break |
| Vivid | Keeps colour strong in bright areas |
| Brighter, as is | Same contrast, lifted to the screen's full brightness |
| No conversion | Shows the source as it is |
| A/B compare | Left: current preset, right: no conversion. Drag the divider |
| Upscale to screen resolution | When the video is smaller than the screen, scales it to the screen's native resolution |
| Frame interpolation | Smooths motion (videos up to 30 fps). When active, "Smooth ×2" appears on screen. If unavailable, the reason is shown |
| Audio & subtitles | Choose the audio track and subtitles |
| Now | Headroom (how many times brighter than normal white, e.g. ×8.0), source resolution and output resolution |

**Which videos can use frame interpolation**

- **720p or smaller, 8-bit**: a lightweight method, works on every supported device
- **1080p, 10-bit**: the app first measures the speed on your device. On iPhone 17 Pro Max it works **up to 1080p at 24 fps**
- **Over 30 fps, or 1440p and larger**: not available (1080p at 30 fps is also too slow). The reason is shown

When the device gets hot or Low Power Mode is on, frame interpolation and super resolution pause automatically (the app tells you so). Colour conversion never pauses.

## Free trial and purchase

- On first launch you will see the **3-day** free trial. Tap **Start Free Trial** to begin
- When the trial ends, **playback stops** (you can still browse folders)
- To keep using the app, make a one-time purchase. **You are never charged automatically**
- After changing devices or reinstalling, tap **Restore Purchase**

## Troubleshooting

| Symptom | What to check |
|---|---|
| The server does not appear | Mac and iPhone on the same Wi-Fi? File Sharing on? Use **Add Server** with the host name (e.g. `name.local`) or IP address |
| "Loading… the disk may be spinning up" | An external HDD can take a few seconds to spin up |
| Playback stopped and **Try Again** appeared | The connection dropped. **Try Again** reopens from the same position |
| "This video needs more than the network provides…" | The video's data rate exceeds your Wi-Fi speed. Move closer to the router, or serve from a wired Mac |
| The picture does not get brighter | At maximum brightness some devices leave no HDR headroom. Lower it slightly |

## Contact

<hello@monneural.dev>
