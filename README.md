# Tube Tools by DC

A Mac app for YouTube: search videos and channels, grab live chat and transcripts, watch, and download videos.

### [⬇️ Download Tube Tools for Mac](https://github.com/danielchi88/tubetools/releases/latest/download/Tube-Tools-by-DC.zip)

Always the latest version · Apple silicon and Intel · macOS 13 Ventura or later · [All releases](https://github.com/danielchi88/tubetools/releases)

## What it does

- **Search** YouTube, or browse a channel by typing its `@handle`. Filter by type (videos, Shorts, live now,
  past streams), views and upload date.
- **Live chat**: capture a stream's chat as it happens, or grab the full chat replay of a finished stream.
- **Transcripts** in the video's language or a translation, with or without timestamps.
- **Download videos** at the resolution you choose (up to 4K), or just the audio.
- **Watch** right in the app, save full-size thumbnails, and keep a history of everything you've captured.

Chats and transcripts save as plain `.txt` files.

## Install

1. **Download** the app with the link above. Safari unzips it for you; otherwise double-click
   `Tube-Tools-by-DC.zip`.
2. **Drag "Tube Tools by DC" into your Applications folder.** (It needs to live there to update itself.)
3. **Open it.** The first time, macOS stops it with a message that Apple couldn't verify the app. That's
   expected: the app isn't notarized by Apple (that needs a paid developer account). To allow it, once:
   - **macOS 15 Sequoia and later:** click **Done**, then open **System Settings → Privacy & Security**, scroll
     down to *"Tube Tools by DC" was blocked*, click **Open Anyway** and confirm with your password.
   - **macOS 13–14:** right-click (or Control-click) the app in Applications, choose **Open**, then **Open** again.

   Or, in Terminal: `xattr -dr com.apple.quarantine "/Applications/Tube Tools by DC.app"`

After that it opens normally.

## Updates

Tube Tools checks for updates each time it opens, for the app itself and for the two tools it uses
([yt-dlp](https://github.com/yt-dlp/yt-dlp) and [FFmpeg](https://ffmpeg.org)), and asks before installing.
You can also click **Check for Updates** at the bottom of the sidebar, pick what to check, and anything newer
is installed right away. The app restarts itself after updating.

Keeping yt-dlp up to date matters: YouTube changes often, and yt-dlp updates are what keep downloads working.

## Tips

- **"Sign in to confirm you're not a bot"**, members-only or age-restricted videos: choose your browser under
  **Cookies** so Tube Tools can use your YouTube sign-in. Safari's cookies need Full Disk Access for the app
  (System Settings → Privacy & Security → Full Disk Access).
- **Live streams** can be downloaded once they've ended. While live, use the chat capture.
- Videos above 1080p use the AV1 or VP9 format. QuickTime plays AV1 on Macs with an M3 chip or newer; on other
  Macs, use a player like [IINA](https://iina.io) or [VLC](https://www.videolan.org).
- History, settings and updated tools are kept in `~/Library/Application Support/TubeTools`.

## Credits

Made by Daniel Chi · [youtube.com/@danielchilive](https://youtube.com/@danielchilive)

Tube Tools uses [yt-dlp](https://github.com/yt-dlp/yt-dlp) (public domain, Unlicense) and
[FFmpeg](https://ffmpeg.org) (GNU LGPL/GPL; builds from [ffmpeg.martin-riedl.de](https://ffmpeg.martin-riedl.de),
source code at [ffmpeg.org](https://ffmpeg.org/download.html)).
Not affiliated with YouTube or Google. Please only download content you have the right to.
