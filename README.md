# SOHEB AI VIDEO — starter app

A mobile-first progressive web app starter for the SOHEB AI VIDEO project.

## What works now
- Responsive dark-blue app UI
- Topic, language, duration, format, style and voice selection
- Saves video requests in this browser/device using localStorage
- My Videos list and delete request
- Backend URL setting and POST request to `/api/generate`
- Installable PWA shell (HTTPS hosting required for install/service worker)

## Important
This starter does **not** generate real videos by itself. To produce actual MP4 videos, deploy a compatible backend that runs MoneyPrinterTurbo or another rendering pipeline, then implement `POST /api/generate` so it returns a job ID/status. Set the deployed backend URL in Settings.

MoneyPrinterTurbo requires Python dependencies, video tools such as FFmpeg, and may use third-party AI services/API keys. Hosting and AI usage may incur costs. Do not put private API keys in this frontend.

## Run locally / deploy
Upload the files to a static hosting service that supports HTTPS (for example, a static site host). Open `index.html` to preview basic UI, though PWA install/offline features require HTTPS hosting.

## Suggested next integration steps
1. Deploy the MoneyPrinterTurbo backend on a compatible Python host or VPS.
2. Add a secure API wrapper endpoint `POST /api/generate`.
3. Store API keys as server-side environment variables.
4. Add job status polling and MP4 download URL handling.
5. Test with a short 30-second video before scaling.

This is a starter project, not a claim that a video backend is already connected.
