# Rainbow Gravity

A calm orbital gravity sandbox for phones. Fling worlds and watch them orbit, slingshot and collide, in rainbow colour. Runs fully offline.

**Play:** https://samplatypus.github.io/Rainbow-Gravity-Sim-Game/ (once GitHub Pages is switched on for this repo)

## How to play
- **Drag** to fling a world. A dotted line shows where it will go.
- **Tap** (or hold still, then let go) to drop a world into a ready-made circular orbit.
- **Two fingers** zoom and pan.
- Pick the mass with **Rock, Moon, Planet, Giant, Star**.
- The ••• menu has Time speed, Trail length, Glow, trail colour, camera and starting scenes (Sun, Binary, Figure 8, Empty).

## Offline
Open it once with a signal, then use your browser's **Add to Home screen** / **Install app**. After that it works with no connection. Every calculation runs on the phone; nothing is fetched from anywhere else.

## The physics
- Newtonian gravity between every pair of worlds, softened slightly so very close passes stay finite.
- Leapfrog (velocity Verlet) integration with a fixed step of 1/240 s. Changing the time speed changes how many steps run, never their size, so orbits stay stable at every speed. Energy holds to about one part in a million over 15 simulated minutes.
- Collisions merge worlds, keeping mass and momentum.
- Tap-to-orbit works out the exact circular speed, picks the right host using Hill spheres (a moon near a planet orbits the planet, not the sun), and orbits close pairs of stars as one.
- Automatically lowers detail on slower phones so it never freezes.

by @SamAndNinjaCat
