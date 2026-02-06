# AR Memory Frame (Pro) - Setup Guide

## 1. Asset Generation
To make the AR work, you need two specific assets in the `assets/` folder:

### A. The Target File (`targets.mind`)
1.  Go to the [MindAR Image Targets Compiler](https://hiukim.github.io/mind-ar-js-doc/tools/compile).
2.  Upload your photo(s).
    -   *For Single Target:* Upload 1 photo.
    -   *For Gallery Mode:* Upload multiple photos (e.g., Photo A, Photo B).
3.  Click **Start Compiler**.
4.  Download the compiled file and rename it to `targets.mind`.
5.  Place it in the `d:/ar/assets/` folder.

### B. The Video File(s)
1.  Select your video memory.
2.  Ensure it is `.mp4` format (H.264 codec preferred).
3.  Rename it to `video1.mp4`.
4.  Place it in the `d:/ar/assets/` folder.
    -   *For Gallery Mode:* Add `video2.mp4` etc., and uncomment the code in `index.html`.

## 2. Running the Project
AR requires a server to access the camera (HTTPS or localhost).

### Option A: VS Code "Live Server"
1.  Open the folder in VS Code.
2.  Install the **Live Server** extension.
3.  Right-click `index.html` -> "Open with Live Server".

### Option B: Local Testing (Mobile)
To test on your mobile device (which has the camera):
1.  You need to serve the file over HTTPS or use a tunneling service like **ngrok**.
    -   Run your local server (e.g., port 5500).
    -   Run `ngrok http 5500`.
    -   Open the generated HTTPS link on your phone.

## 3. "Pro" Features Guide
-   **Audio**: Tap the "Mute" icon to toggle sound. Starts muted by default.
-   **Snapshot**: Tap the "Camera" icon to save a clean photo without UI.
-   **Gallery Link**: Appears automatically when the video finishes playing.
