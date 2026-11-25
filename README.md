# Autoclip IP‑Location Tracker

This repository contains a single static HTML page (`index.html`) that:

1. Detects the visitor’s public IP address and approximate location using the free **ip‑api.com** service.
2. Shows the IP, city, region, country, ZIP code, coordinates and ISP.
3. After a short 3‑second pause it automatically redirects the visitor to a YouTube video (default is the classic “Rick‑Roll” – replace the URL in `index.html` with your own video if desired).

## Deploying
You can host this page on any static‑site provider (GitHub Pages, Netlify, Vercel, Azure Static Web Apps, etc.). The easiest way is GitHub Pages:

1. Create a new **public** repository on GitHub (e.g., `autoclip‑tracker`).
2. Add this repository as a remote and push the contents.
3. Enable **GitHub Pages** in the repo settings – set the source to the `master` (or `main`) branch and root folder.
4. Your tracker will be reachable at `https://<username>.github.io/autoclip‑tracker/`.

## Updating the YouTube link
Edit `index.html` and replace the value of `redirectUrl` near the top of the script with the URL of the video you want visitors to be sent to.

```js
const redirectUrl = 'https://www.youtube.com/watch?v=YOUR_VIDEO_ID';
```

## License
Public domain / CC0 – feel free to use, modify, or embed wherever you need.
