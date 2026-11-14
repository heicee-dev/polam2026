# Polam Apartment — 3D Walkthrough

First-person 3D walkthrough of the Polam (“Pig House”) apartment floor plan.

## Open locally

The walkthrough is a single self-contained file. No build step is required.

```bash
# Option A — open directly in a browser
open index.html          # macOS
xdg-open index.html      # Linux

# Option B — local static server (recommended for pointer lock / mobile testing)
python3 -m http.server 8080 --bind 127.0.0.1
# then visit http://127.0.0.1:8080/
```

Requires network access once for the Three.js CDN script (`cdnjs.cloudflare.com`).

## Controls

| Input | Action |
|--------|--------|
| **WASD** / arrows | Move |
| **Mouse** | Look (click to lock pointer) |
| **Shift** | Sprint |
| **Esc** | Release pointer |
| **Mobile** | Left joystick move · right joystick look |

## Layout

- **Entrance** (east) — shoe rack by the door; start facing into the apartment
- **Living** (southwest) — sofa, coffee table, TV
- **Kitchen** (northwest) — counters, stove, sink, fridge
- **Bathroom** (center-north) — toilet, vanity, shower
- **Bedroom 1** (northeast) — bed, desk, wardrobe
- **Bedroom 2** (southeast) — bed, desk, wardrobe; shared wall with Bedroom 1 is **357 + 750 (door) + 2525 mm**

Includes wall collision, a HUD minimap, and floating room labels.

## Files

- `index.html` — complete Three.js walkthrough (classic CDN script tag)
- `floorplan.jpg` — schematic top-down floor plan
- `README.md` — this file
