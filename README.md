# 🎮 Bandersnatch Interactive Player

This is an interactive web-based video player inspired by Netflix’s *Bandersnatch*, enabling branching video narratives where users choose what happens next.

## 📂 Project Structure

```
project-folder/
├── index.html
├── bandersnatch.js         # Main object script with interactive metadata
├── SegmentMap.js           # Segment timing and structure definitions
├── Black.Mirror.Bandersnatch.2018.720p.WEB-DL.x264.DUAL.mkv  # (You must legally own this)
├── Black.Mirror.Bandersnatch.2018.720p.WEB-DL.x264.DUAL.en.vtt  # English subtitles
```

## ▶️ Features

* Full video playback with synchronized choice prompts
* Branching logic driven by segment and moment metadata
* Support for user state tracking (`persistentState`)
* Keyboard navigation:

  * `→` Jump forward
  * `←` Jump back
  * `F` Toggle fullscreen
  * `Space` Play/Pause
  * `R` Restart

## 🌐 How to Use

1. Place all files in the same folder.
2. Ensure your video and `.vtt` file are correctly named and accessible.
3. Open `index.html` in a browser that supports fullscreen and `video` autoplay.
4. Start watching and make choices!

> ⚠️ Note: Make sure the video is legally acquired. This project is for educational and demo purposes only.

## 🚀 Optional Improvements

* Host on a local server to avoid autoplay restrictions
* Add more condition logic for deep state transitions
* Customize UI with CSS for a Netflix-like theme

## 💡 Credits

* Inspired by *Netflix Bandersnatch*
* Based on reverse-engineered data from [jonluca/segment-parser](https://gist.github.com/jonluca/860f3f445e7d84054822276fd058301a)
* Segment map example from [jolbol1/Bandersnatch](https://github.com/jolbol1/Bandersnatch)
