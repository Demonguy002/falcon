# FALCON SOVEREIGN — Cinematic Launch Website

Static HTML/CSS/JavaScript launch experience for the Team Falcon AI/ML forum.

## Contents

- `index.html` — main launch webpage
- `assets/falcon-narration.mp3` — narration audio
- `assets/mountain-leadership.mp3` — background music
- `assets/falcon-hero-reveal.mp4` — main cinematic reveal video
- `assets/falcon-logo-loop.mp4` — looping Team Falcon logo video
- `assets/falcon-poster.jpg` — video poster/fallback image

## Deploy to Vercel through GitHub

1. Create a GitHub repository, e.g. `falcon-sovereign-launch`.
2. Upload **the contents of this folder** so that `index.html` is at the repository root and the `assets` folder is beside it. Do not upload a parent folder that contains the project as a nested directory.
3. In Vercel, choose **Add New → Project**, import the GitHub repository, and continue.
4. Choose **Other** as the framework preset. Leave Build Command and Install Command empty. Leave Output Directory empty (or use `.` if the Vercel screen requires a value).
5. Click **Deploy**. Once deployment finishes, open the generated `vercel.app` URL.

## Important

All media paths are relative (`assets/...`). Keep the `assets` directory and filenames unchanged. The site is static; no backend or build process is required. Video/audio playback should begin after the visitor clicks **Initiate Launch**, because browsers restrict autoplay with sound.

## Test locally

Because media playback can be restricted when opening files directly, use a local web server. If Python is installed:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.
