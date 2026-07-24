# CA Final Study Tracker — Installable Mobile App (PWA)

This folder is a complete, installable web app (a "Progressive Web App").
Each person who installs it gets their OWN independent copy of the data,
stored only on their own phone/browser — nothing is shared or synced
between users, and nothing goes through any of your accounts.

## Files
- index.html          -> the app itself
- manifest.json        -> tells phones how to install it (name, icon, colors)
- service-worker.js     -> lets it work offline once installed
- icons/icon-192.png, icons/icon-512.png -> app icons

## Step 1 - Put it on the internet (needed once, by you)
A PWA needs to be served from a real URL (not just opened as a local file)
for "Add to Home Screen" and offline mode to work properly. Easiest free
options, no coding required:

1. **GitHub Pages** (free, keeps a URL forever)
   - Create a free GitHub account if you don't have one.
   - Create a new repository, upload all files in this folder (keep the
     "icons" folder structure as-is).
   - Go to Settings -> Pages -> set source to your main branch -> Save.
   - GitHub gives you a URL like: https://yourusername.github.io/reponame/

2. **Netlify Drop** (free, fastest, no account needed for a quick test)
   - Go to https://app.netlify.com/drop
   - Drag this whole folder onto the page.
   - It instantly gives you a live URL you can share.

Either way, once it's live, share that URL with anyone you want to use it.

## Step 2 - Install it on a phone
Whoever visits the URL on their phone:
- **Android (Chrome)**: tap the 3-dot menu -> "Add to Home screen" / "Install app"
- **iPhone (Safari)**: tap the Share icon -> "Add to Home Screen"

It will then appear as its own app icon, open full-screen (no browser bars),
and work offline after the first visit.

## Important notes
- Data is stored per person, per browser, per device — it does NOT sync
  between a phone and a laptop, or between two different people.
- Each person should keep using the same URL/installed icon going forward —
  don't reinstall from a different link or clear site data, or their
  entries will reset.
- If you update the tracker later (new columns, fixed bugs, etc.), just
  re-upload the changed files to the same GitHub/Netlify location — everyone's
  installed app will pick up the new version next time they open it with
  an internet connection (the old data stays untouched).
