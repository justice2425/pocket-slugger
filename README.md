# Pocket Slugger ⚾

A small, ad-free baseball game for iPad and Mac. It works offline, has no accounts, and collects no data.

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The whole game (code, graphics and sounds are all inside) |
| `sw.js` | Lets the game work offline after the first visit |
| `manifest.webmanifest`, `icon-*.png` | Name and icon for the Home Screen / Dock |
| `README.md` | These instructions |

## 1. Put it on GitHub Pages (one time, about 10 minutes)

1. Sign in to github.com as **justice2425**, then click **+** (top right) → **New repository**.
2. Name it exactly `pocket-slugger` (lowercase, with the dash). Leave it **Public**, because GitHub Pages on a free account only works with public repositories. Click **Create repository**.
3. On the new repository page, click **uploading an existing file**.
4. Drag in **all the files from this folder** (not the folder itself). Click **Commit changes**.
5. Go to **Settings** → **Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, folder **/ (root)**, then click **Save**.
6. Wait 1–2 minutes and refresh that page. It will show your game's address:
   **https://justice2425.github.io/pocket-slugger/**
   (Note: this address only works if you named the repository exactly `pocket-slugger`.)

## 2. Install it on the iPad

1. Open **https://justice2425.github.io/pocket-slugger/** in **Safari** and wait until the title screen appears.
2. Tap **Share** (the square with an arrow) → **Add to Home Screen** → **Add**.
3. Open the game **from the new icon** once while you're online. This saves it for offline play.
4. Test it: turn on Airplane Mode, then open the icon. It should still work.

Always play from the icon rather than from a Safari tab. The icon and Safari keep separate save data, so a team built in one won't show up in the other.

## 3. Install it on the Mac

- **Option A (Safari on macOS Sonoma or later):** open **https://justice2425.github.io/pocket-slugger/** in Safari → **File → Add to Dock**.
- **Option B (no internet at all):** double-click `index.html` from this folder. It opens in your browser and works fully offline. Saves made this way are separate from the Dock version.

## Saving and moving teams between devices

- Progress is saved only on the device and app you play on. Nothing is uploaded.
- **My Team → Make a backup code** gives you a text code. Paste it into **Load a backup** on another device (or after erasing Safari data) to bring the team back.

## Updating the game later

Upload a new `index.html` (and `sw.js`) to the repository the same way, replacing the old files. The game picks up the new version the next time it's opened while online.

## Security notes

- The page has a strict Content Security Policy. It runs only its own built-in code and is blocked from connecting to the internet.
- The offline helper (`sw.js`) only handles this site's own files.
- Names typed into the game are shown as plain text and never run as code. Backup codes are checked and cleaned before loading.
- The repository is public, so anyone could read the code. It contains no personal information or passwords.

## How to play (short version)

- **Batting:** tap as the ball reaches the white box. Early pulls the ball, late pushes it the other way. *Rookie* mode only needs timing. *Pro* mode needs timing **and** a tap where the ball crosses.
- **Pitching:** pick a pitch, tap a spot, then tap when the ring turns gold.
- **Fielding:** on close plays, tap when the ring hits the gold circle around your player.
- **Running:** use **Steal** before a pitch. After a hit you may be asked whether to go for an extra base.
- **Team:** earn coins against the computer and spend them on upgrades.
- **Mac keyboard:** Space = swing / throw / tap, arrow keys = aim, 1–4 = pitch type, S = steal, Y / N = run or stay, Esc = pause.
