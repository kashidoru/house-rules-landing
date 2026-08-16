# House Rules Landing Page

Deploy this `landing` folder as a Vercel project (Framework Preset: **Other**).

## Environment Variables

Set these Vercel environment variables before deployment:

- `DOWNLOAD_KEYWORD` — the keyword printed on your invite card (default: "JADESSS")
- `ANDROID_DOWNLOAD_URL` — your EAS internal-build install URL, or your Google Play Store URL

## Security Note

The keyword is verified by the serverless endpoint, so it is not embedded in browser code. This is an access gate, not DRM: someone who receives the final install URL can still share it.

⚠️ **Client-Side Fallback**: The landing page includes a client-side code check as a fallback. This is easily bypassed by viewing the page source and is NOT real security — it's just a casual gate. For production use, ensure the server-side API endpoint is properly configured.

## Features

- **JADESSS Wordmark**: Large stylized wordmark with gradient animation and smooth entrance
- **Access Code Gate**: Server-side keyword validation with client-side fallback
- **Modern UI**: Dark theme with glowing effects and smooth animations
- **Responsive**: Works on all screen sizes
- **No Database**: Static hosting with serverless API endpoint

## Deployment

1. Push this folder to a Git repository
2. Import the project in Vercel
3. Set environment variables
4. Deploy

## Analytics

No database is needed for this page or the game. Turn on Vercel Web Analytics if you want page-visit metrics. Reliable install/download totals require a tracked download service or a database-backed event endpoint.
