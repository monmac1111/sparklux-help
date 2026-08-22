# Sparklux Help

## What Sparklux does

**It converts SDR video to HDR in real time.** Nothing is converted to a new file — the
processing happens as the picture is drawn. It also upscales the resolution.

HDR video (HDR10, HLG, Dolby Vision Profile 8) is shown **exactly as it is**, untouched.

## Requirements

| | |
|---|---|
| macOS | 14 or later |
| HDR output | An **HDR-capable display** is required (built-in XDR display, a supported external display, …) |
| Formats | MP4 / MOV / M4V, HLS (.m3u8), direct links, network shares |

⚠️ On a display that cannot show HDR, the conversion does not run. The app says so at the top of the window.

## Do this first — calibrate your display (⌘K)

**This makes the brightness correct.** Without it the app uses a conservative default.

1. Press ⌘K
2. **Step 1 of 2** — press Enter when the white panel on the left and the patch on the right
   look **equally bright**. You have it right when the edge between them disappears
3. **Step 2 of 2** — raise the value and press Enter when it **stops getting brighter**

The measurement is remembered per display.

## Presets (colour rendering)

Choose from the button at the right end of the control bar.

| | |
|---|---|
| **No conversion** | Show the source as it is |
| **Subtle** | Slightly brighter. Use when highlights clip |
| **Cinema** | Keeps midtones, lifts only the highlights |
| **Natural** | Natural brightness. The default; hard to break |
| **Vivid** | Keeps colour strong in bright areas |
| **Real** | Photographic tonality (uses a model) |

Use **A/B** to compare two presets.

## Resolution (upscaling)

In the lower half of the same menu.

| | |
|---|---|
| **No upscaling** | Keep the source resolution |
| **Sharper (MetalFX)** | Default. Uses what is in the source; it does not invent edges |
| **Sharper (Lanczos)** | Classic upscaling |
| **Sharper (strong)** | Stronger |

⚠️ **Upscaling does not run when the window is smaller than the source** (there is nothing to
gain). The status line says so. Go **full screen** or enlarge the window.

## Keyboard

| | |
|---|---|
| Space | Play / Pause |
| ← / → | Back / forward 5 seconds |
| ⌥⌘← / ⌥⌘→ | Previous / next chapter |
| ↑ / ↓ | Volume |
| ⌘K | Calibrate the display |
| ⌘⌃F | Full screen |
| ⌘O | Open a file |
| ⌘⇧L | Open a URL |

## Subtitles

- Embedded subtitles are read automatically
- **External subtitles** are picked up when they sit next to the video with the same name
  (`movie.mp4` → `movie.srt`). SRT and WebVTT; UTF-8, Shift_JIS, EUC and UTF-16 are handled

## Audio

- **5.1 and 7.1 are passed through** unchanged
- On a stereo output they are folded down **so that dialogue is not lost**
- Dolby Atmos titles play as the 5.1 or 7.1 bed underneath

## Playing a URL

Press ⌘⇧L.

- A **direct video link** (`https://…/movie.mp4`)
- **HLS** (`https://…/index.m3u8`)
- A **network share** address

### Streaming services (YouTube and similar)

⚠️ **Sparklux cannot play these on its own.** It can do so only if you have installed
`yt-dlp` yourself, in which case it invokes it.

```
brew install yt-dlp
```

- The app **neither bundles nor installs** yt-dlp
- **Netflix, Prime Video and Disney+ cannot be played** (they are protected)
- **A VPN may cause the request to be refused** (403). Turn it off and try again
- Services change their delivery from time to time. Update yt-dlp if playback stops working

## Power saving

Choose it from the menu. On **Automatic**, when the machine gets hot or runs on battery,
processing is paused in stages (model → sharpening → upscaling; the HDR conversion is kept
until last). The status line says what was paused.

## Pricing

**One-time purchase.** After a seven-day free trial, a single purchase lets you use the app
forever **on every Mac signed in to the same Apple ID**. There is no monthly fee.

- On another Mac, choose **“Restore Purchase”** from the menu
- iCloud is used to manage the free trial (the start date only → [Privacy Policy](privacy.md))

## Troubleshooting

| Symptom | What to check |
|---|---|
| **Colour does not change** | Is the display HDR-capable (is there a warning at the top)? Is the preset set to “No conversion”? |
| **Upscaling has no effect** | Is the window smaller than the source? Check the status line. Full screen makes it work |
| **Brightness looks wrong** | Calibrate with ⌘K |
| **A file will not open** | In System Settings → Privacy & Security → Files and Folders, grant access, or reopen with ⌘O |
| **A URL will not open** | Check the URL and your connection. Streaming services have the limits described above |
| **No sound** | Is an audio track selected (menu → Audio Track)? |

## Contact

<hello@monneural.dev>
