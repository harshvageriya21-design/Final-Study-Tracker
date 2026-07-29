# CA Study Tracker (Foundation + Intermediate + Final) — Installable Mobile App

One single app now covers all three CA levels. A dropdown at the top lets
you (or any friend using it) switch between:
- CA Foundation
- CA Intermediate
- CA Final

Each level keeps its own completely separate data (subjects, chapters,
weightage, revisions, question bank, test log, exam date) within the same
installed app — switching levels never mixes or overwrites another level's
progress.

Each person who installs this gets their OWN independent copy of the data,
stored only on their own phone/browser — nothing is shared or synced
between users.

## Files
- index.html          -> the app itself
- manifest.json         -> tells phones how to install it (name, icon, colors)
- service-worker.js      -> lets it work offline once installed
- icons/icon-192.png, icons/icon-512.png -> app icons

## Step 1 - Put it online (needed once, by you)
1. **Netlify Drop** (free, fastest, no signup for a quick test)
   - Go to https://app.netlify.com/drop
   - Drag this whole folder onto the page — you get a live URL instantly.
   - To keep the link permanent, create a free Netlify account and claim
     the site afterwards (Site settings -> your dashboard).

2. **GitHub Pages** (also free)
   - Create a public GitHub repo, upload all files (keep the icons/ folder).
   - Settings -> Pages -> Deploy from branch -> main -> / (root) -> Save.

## Step 2 - Install it on a phone
On the live URL:
- **Android (Chrome)**: 3-dot menu -> "Add to Home screen" / "Install app"
- **iPhone (Safari)**: Share icon -> "Add to Home Screen"

It then opens as its own full-screen app icon and works offline.

## Notes for your friends using it
- Pick your level from the dropdown at the top once — the tracker remembers
  your choice and reopens on the same level next time.
- Data is stored per person, per browser, per device — it does NOT sync
  between people or between a phone and a laptop.
- Keep reopening the same installed icon/URL — don't reinstall from a
  different link or clear site data, or entries will reset.
- The "⬇ Backup JSON" button saves everything (all three levels) as one
  file — useful before clearing browser data or switching phones.
