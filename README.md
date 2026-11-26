# Racing Through Bulverde 🚗💨

A Pac-Man-style arcade game set on the roads of Bulverde, TX. One HTML file, no build step, no install.

**Play:** https://drod0422.github.io/racing-through-bulverde/

## How to play

- **Difficulty:** Rookie (slower critters, longer kolache time, 5 lives), Pro (arcade speed), or Legend (fast critters, short kolache time). Each has its own high score and Top 5 board.

- **Steer:** swipe, tap the on-screen arrows, or use the arrow keys / WASD. `P` pauses.
- **Road lights:** grab them all to clear the street.
- **🥐 Kolache:** the critters turn blue and run. Catch them back to back for 200 → 400 → 800 → 1,600.
- **⚡ Boost pads:** a quick speed burst.
- **Bonus food:** shows up below the barn twice a level.
- **Rides:** unlock new skins as your best score climbs (Walter the schnauzer from the start, then truck, BMX, race car, tractor, UFO).

High scores, unlocks, and the Top 5 board save on each device.

## Making it yours

Everything kid-editable is at the top of the `<script>` in `index.html`:

| Constant | What it controls |
|---|---|
| `LEVEL_NAMES` | Level names, shown in order (also the big sign at the top of the maze) |
| `PLACES` | Names on the green street signs: full name → short sign label |
| `SIGN_SPOTS` | Where signs sit on the maze: `[x, y, width]` on wall rows |
| `BONUS` | Bonus food per level: emoji, name, points |
| `SKINS` | Playable rides and the score that unlocks each |
| `CRITTERS` | Every critter that can chase you |
| `CASTS` | Which 4 critters chase you on each level |
| `SLOTS` | AI style per chaser slot (`chase`, `ahead`, `wander`, `shy`) |
| `MAP_SRC` | The maze. `#` wall, `.` road light, `o` kolache, `P` start, `G` barn. Keep every row 19 characters wide. |
| `DIFFS` | Speed, kolache time, lives, and release timing for each difficulty |
| `BOOST_PADS` | `[x, y]` tiles that give a speed boost |

Commit to `main` and GitHub Pages updates in about a minute.
