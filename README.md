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

## Updating from an earlier version

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

## Game modes

- **Play vs Computer / 2 Players:** regular games in any of the 10 ballparks.
- **🏆 Season:**
  - Your team plus 5 computer teams play 10 games each, with standings after every round.
  - The top 4 teams make the playoffs.
  - Win the championship to get a trophy and 200 coins.
  - The computer teams' other games are simulated. You can also simulate one of your own games if you're short on time.
- **🏟️ Home Run Derby:**
  - 10 swings to hit as many home runs as you can, solo or 2 players taking turns.
  - Pitches you don't swing at don't count.
  - Tracks your longest home run and your personal best, and pays 3 coins per homer.
- **⚾ Batting Cage:**
  - Unlimited practice: pick any pitch type (or mix them up) and the speed.
  - A **timing meter** after every swing shows exactly how early or late you were.
  - The meter also appears briefly in regular games.
- **🏅 Trophies:** your championship trophies, 22 badges (each pays 20 coins) and your records.
- **🧢 My Team:**
  - Tap **✏️ Look** on any player to change their skin tone, hair color and style, gear, jersey number, name and batting side.
  - Open **👕 Design your uniform** to pick a main and trim color, pinstripes or two-tone sleeves, pants color and a cap logo with your letter.
  - Players' names and numbers show on the backs of their jerseys.

## Saving and moving teams

Progress is saved only on the device you play on. To move a team:
1. Go to **My Team → Make a backup code**.
2. On the other device, paste the code into **Load a backup**.

## Security notes

- The page has a strict Content Security Policy. It can only run its own built-in code, and it's blocked from connecting to the internet.
- The offline helper (`sw.js`) only handles this site's own files.
- The umpire and announcer voice uses voices built into the device only. If the device has no built-in English voice, the game stays silent rather than using an online one.

## Making the voice sound natural

The game picks the best voice on the device and skips Apple's joke voices. For a much more natural voice:

1. Download a free **Premium** or **Enhanced** voice. Ava (Premium) is a good one.
   - **iPad:** Settings → Accessibility → **Read & Speak** → Voices → English. On older iPads it's called **Spoken Content**. You can also just search Settings for "Voices".
   - **Mac:** System Settings → Accessibility → Spoken Content → System Voice → Manage Voices.
2. In the game, open **Settings → Voice**, pick that voice and tap **Test voice**.

Voice options:
- **Umpire calls** (default): only the big calls, like "Strike three!", "Ball four", "Safe!", "Out!" and "Home run!"
- **Umpire + announcer**: also calls every pitch and each batter's name.
- **Off**
- Names typed into the game are treated as plain text, and backup codes are checked before loading.

## How to play

- **Batting:** tap as the ball reaches the box. In *Rookie* mode a ring shrinks onto the ball to help with timing. After each pitch you'll see which pitch it was and the path it took.
- **Batting options (before the pitch):** Swing, **Bunt**, or **Fly ball**. Fly ball turns into **Sac fly** when a runner is on third with fewer than two outs.
- **Running:** use **Steal** before a pitch. After a hit you may be asked whether to send a runner. After a catch you may be asked whether to tag up.
- **Pitching:** the camera sits behind your pitcher, looking in at the batter. Pick a pitch, steer the crosshair with the **thumb-stick** (bottom left) or tap where you want it, press **PITCH**, then press it again (**THROW!**) when the ring turns gold. **IBB** (tap twice) walks the batter on purpose. You get **pickoff** throws when a runner is on (2 per batter). Prefer the old view? Settings → *Camera when you pitch* → *Behind home plate*.
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
