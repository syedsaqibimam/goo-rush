# Goo Rush: Zombie Parkour 🧟💚

A cartoony 3D parkour survival game for phones and computers. A zombie horde chases you through a city: climb rooftops, slide under grabs, ride ziplines, and open chests for guns. Zombies melt into goo (no blood).

## Play / install on your phone
1. Open the GitHub Pages link for this repo on your phone (Settings → Pages shows it, e.g. `https://<username>.github.io/goo-rush/`).
2. Install it:
   - **Android (Chrome):** menu ⋮ → **Install app** / **Add to Home screen**
   - **iPhone (Safari):** Share → **Add to Home Screen**
3. Launch it from the home-screen icon: full screen, landscape, and it works offline after the first load.

## Controls
| | Phone | Computer |
|---|---|---|
| Move | Left-side joystick | WASD / arrows |
| Attack (auto-aim) | 💥 button | Click / F |
| Jump | ⤒ button | Space |
| Slide | ⤵ button | Shift |
| Zipline | 🪂 button (appears near one) | E |

## Gameplay
- Start with a **knife** (1 damage). Stand by a chest to open it:
  - 🟫 Brown → **Pistol** (common)
  - 🟦 Blue → **Minigun** (uncommon)
  - 🟨 Gold → **Alien Blaster** (rarest, pierces)
- Zombies: 🟢 **Normal**, 🔵 **Fast** (after ~25s), 🟠 **Strong** (after ~55s, climbs walls)
- Zombies follow you up **ramps**; they can't follow you on **ziplines**
- Zip, slide and air kills score **x2**

## Tech
Single-page Three.js (r128) game, no build step. `sw.js` + `manifest.webmanifest` make it an installable, offline-capable PWA. Deployed with the GitHub Pages workflow in `.github/workflows/pages.yml`.

Run locally: `python3 -m http.server` then open http://localhost:8000
