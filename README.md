# 1% Better — Habit Tracker PWA

A responsive installable Progressive Web App for tracking 20 habits, daily reflections, history, streaks, and charts. All habit data is stored locally in the browser on each device.

## Run locally on Windows

1. Extract the ZIP file.
2. Open the folder in VS Code.
3. Open a terminal in the folder.
4. Start a local web server. If Python is installed, run:

   ```powershell
   py -m http.server 8000
   ```

   Or, if `py` is unavailable:

   ```powershell
   python -m http.server 8000
   ```

5. Open `http://localhost:8000` in Chrome or Edge.

Service workers and PWA installation need `localhost` or HTTPS; opening `index.html` directly as a file will not enable offline/install support.

## Install on Windows

For an installable app on Windows, deploy the folder to an HTTPS static host, then open its URL in Chrome or Edge. Use the browser's Install app option (or the install button if offered). Some browsers may also support installation from localhost for development.

## Install on Android

1. Deploy the folder to an HTTPS static host.
2. Open the URL in Chrome on Android.
3. Open the three-dot menu and choose **Install app** or **Add to Home screen**.

## Publish it online (static hosting)

Upload the contents of this folder to any static web host that serves HTTPS and preserves the folder structure. No build step or npm packages are required. Examples include GitHub Pages or Netlify. If using GitHub Pages, place the files at the root of a repository and enable Pages for the chosen branch/folder.

## Data and privacy

- Data is stored in browser `localStorage` on that device. It is not synced between your laptop and phone automatically.
- Use **Export my data** in the footer to download a JSON backup, and **Import backup** on another device to transfer it.
- Clearing browser/site data can delete the local history, so export backups occasionally.
- The app's core files are cached for offline use after the first successful load. Google Fonts are optional and may not load offline.

## Edit the habits

Edit the `HABITS` array near the top of `app.js`. Keep 20 items if you want the progress ring and percentages to remain out of 20.
