# 🎮 Bandersnatch Interactive Player

This is an interactive web-based video player inspired by Netflix's *Bandersnatch*, enabling branching video narratives where users choose what happens next.

> ❤️ This project is being maintained in memory of a child who loved the *Bandersnatch* experience and was heartbroken when Netflix removed the movie and the game disappeared. This player is a tribute to preserving that creativity and choice-driven storytelling for others to enjoy and learn from.

## 📂 Project Structure

```
project-folder/
├── LICENSE
├── README.md
├── SECURITY.md
├── bandersnatch.json
├── SegmentMap.json
├── bandersnatch.js                        # Main object script with interactive metadata
├── SegmentMap.js                          # Segment timing and structure definitions
├── index.html                             # Main player interface
├── Black.Mirror.Bandersnatch.2018.720p.WEB-DL.x264.DUAL.mkv  # Local video file
```nteractive Player

This is an interactive web-based video player inspired by Netflix’s *Bandersnatch*, enabling branching video narratives where users choose what happens next.

> ❤️ This project is being maintained in memory of a child who loved the *Bandersnatch* experience and was heartbroken when Netflix removed the movie and the game disappeared. This player is a tribute to preserving that creativity and choice-driven storytelling for others to enjoy and learn from.

## 📂 Project Structure

```
project-folder/
├── license
├── readme.md
├── SegmentMap.js                          # Segment timing and structure definitions
├── bandersnatch.js                        # Main object script with interactive metadata
├── index.html                             # configured for nebulaflix.stream
├── Black.Mirror.Bandersnatch.2018.720p.WEB-DL.x264.DUAL.en.vtt  # English subtitles
```

- `nebulaflix.stream`

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

1. **Download the video file** from: `https://fv5-2.files.fm/down.php?i=wc9kkj5mdc&n=Black.Mirror.Bandersnatch.2018.720p.WEB-DL.x264.DUAL.mkv`
2. **Place the downloaded video file** in the same folder as `index.html` with the exact filename: `Black.Mirror.Bandersnatch.2018.720p.WEB-DL.x264.DUAL.mkv`
3. **Ensure all required files are present**:
   - `bandersnatch.js` (contains interactive metadata)
   - `SegmentMap.js` (contains segment timing definitions)
4. **Open `index.html`** in a browser that supports fullscreen and `video` autoplay
5. **Start watching and make choices!**

> ⚠️ Note: This version uses a local video file. Host on a local server (e.g., with `python3 -m http.server`) to avoid browser restrictions. This project is for educational and memorial purposes only.

## 🚀 Optional Improvements

* Host on a local server to avoid autoplay restrictions (e.g. with `python3 -m http.server`)
* Add more condition logic for deep state transitions
* Customize UI with CSS for a Netflix-like theme
* Replace `eval()` usage with a safer parser for conditions
* Build a test version with royalty-free videos and simple JSON maps

## 💡 Credits

* Inspired by *Netflix Bandersnatch*
* Based on reverse-engineered data from [jonluca/segment-parser](https://gist.github.com/jonluca/860f3f445e7d84054822276fd058301a)
* Segment map example from [jolbol1/Bandersnatch](https://github.com/jolbol1/Bandersnatch)
