# Pocket Slugger ⚾

A small, ad-free baseball game for iPad and Mac. It works offline, has no accounts, and collects no data.

Your game's address: **https://justice2425.github.io/pocket-slugger/**

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The whole game (code, graphics and sounds are all inside) |
| `sw.js` | Lets the game work offline after the first visit |
| `manifest.webmanifest`, `icon-*.png` | Name and icon for the Home Screen / Dock |
| `README.md` | These instructions |

## Updating from the first version

1. On github.com, open your `pocket-slugger` repository and click **Add file → Upload files**.
2. Drag in **all the files from this folder** and click **Commit changes**. GitHub replaces the old files.
3. Wait 1–2 minutes. Then, **while online**, open the game from the iPad's Home Screen icon. Close it and open it once more. You'll now be on the new version.

Your son's team, coins and upgrades carry over. The new version reads the old save.

## First-time setup (if starting fresh)

1. Sign in to github.com as **justice2425**, then click **+** → **New repository**.
2. Name it exactly `pocket-slugger` and leave it **Public**. On free accounts, GitHub Pages only works with public repositories.
3. Click **uploading an existing file**, drag in all the files from this folder, then click **Commit changes**.
4. Go to **Settings → Pages**. Set Source to **Deploy from a branch**, Branch to **main**, folder **/ (root)**, and click **Save**.
5. After 1–2 minutes the game is at **https://justice2425.github.io/pocket-slugger/**

**iPad:**
1. Open the address in Safari.
2. Tap **Share → Add to Home Screen**.
3. Open the game from the icon once while online.
4. Test it with Airplane Mode turned on.

Always play from the icon: the icon and Safari keep separate saves.

**Mac:** either open the address in Safari (macOS Sonoma or later) and choose **File → Add to Dock**, or double-click `index.html`.

## Saving and moving teams

Progress is saved only on the device you play on. To move a team:
1. Go to **My Team → Make a backup code**.
2. On the other device, paste the code into **Load a backup**.

## Security notes

- The page has a strict Content Security Policy. It can only run its own built-in code, and it's blocked from connecting to the internet.
- The offline helper (`sw.js`) only handles this site's own files.
- The umpire and announcer voice uses voices built into the device only. If the device has no built-in English voice, the game stays silent rather than using an online one.
- Names typed into the game are treated as plain text, and backup codes are checked before loading.

## How to play

- **Batting:** tap as the ball reaches the box. In *Rookie* mode a ring shrinks onto the ball to help with timing. After each pitch you'll see which pitch it was and the path it took.
- **Batting options (before the pitch):** Swing, **Bunt**, or **Fly ball**. Fly ball turns into **Sac fly** when a runner is on third with fewer than two outs.
- **Running:** use **Steal** before a pitch. After a hit you may be asked whether to send a runner. After a catch you may be asked whether to tag up.
- **Pitching:** pick from your pitches, tap a spot, then tap when the ring turns gold. You get **pickoff** throws when a runner is on (2 per batter).
- **Fielding:**
  - On ground balls with runners on, **tap the base you want to throw to**.
  - On close plays, tap when the ring hits the gold circle.
  - When the computer steals, you get a chance to throw the runner out.
- **Team:** earn coins (games, hits, homers, strikeouts and trivia) and spend them on upgrades and **new pitches**. There are 11 pitches in all, including the knuckleball and the super-slow eephus.
- **Ballparks:** 10 made-up stadiums with different fences. Watch out for the Grand Wall, and the low gravity on the Moon.
- **Between innings:** a quick fact, rule, coach's tip or trivia question. You can change how often in Settings.
- **Mac keyboard:**
  - Space: swing / throw / tap
  - Arrow keys: aim
  - 1–7: pick a pitch
  - B: bunt
  - F: fly ball
  - S: steal
  - Y / N: go or stay
  - 1 / 2 / 3 / H: throw to a base
  - Esc: pause
