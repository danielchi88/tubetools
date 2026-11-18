# Tube Tools by DC

A Mac app for YouTube: search videos and channels, grab live chat and transcripts, watch, and download videos.

### [⬇️ Download Tube Tools for Mac](https://github.com/danielchi88/tubetools/releases/latest/download/Tube-Tools-by-DC.zip)

Always the latest version · Apple silicon and Intel · macOS 13 Ventura or later · [All releases](https://github.com/danielchi88/tubetools/releases)

> **Only use Tube Tools on content you own or have permission to use.** It's meant for your own videos,
> streams, chats and transcripts. You are responsible for how you use it, including following
> [YouTube's Terms of Service](https://www.youtube.com/t/terms), copyright law and the rights of creators and
> viewers. Tube Tools is provided as is, without warranty, and its developer is not responsible for how it's used
> or for anything downloaded with it.

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

Each time it opens, Tube Tools shows its **Terms of Use**: you confirm you'll only use it on content you own or
have permission to use. Click **I Agree** to continue, or **Quit**. Tick **Don't show this again for 30 days** to
skip it for a month. You can read them again any time under **Help → Terms of Use…**.

## Updates

Tube Tools checks for updates each time it opens, for the app itself and for the two tools it uses
([yt-dlp](https://github.com/yt-dlp/yt-dlp) and [FFmpeg](https://ffmpeg.org)), and asks before installing.
You can also click **Check for Updates** at the bottom of the sidebar, pick what to check, and anything newer
is installed right away. The app restarts itself after updating.

Keeping yt-dlp up to date matters: YouTube changes often, and yt-dlp updates are what keep downloads working.

## Download limits

To keep you from being blocked by YouTube, downloads pause for a random 5–10 seconds between videos, and at most
**20 videos** are downloaded in any 15 minutes. Everything saved from one video counts as one, and loading a
video's chat and transcript doesn't count. When a limit kicks in, the download window shows a countdown
("Cooling down before the next video… 7s", or "Resuming in 4:12") and carries on by itself.

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
Not affiliated with YouTube or Google. Only download content you own or have permission to use.
