# Bavaria COP 1809
### Common Operating Picture — 1809 Danube Campaign
**U.S. Army War College — Napoleonic Studies**

> ⚔ **[Launch the App](https://emilpoisdown-dev.github.io/Bavarian-COP-1809/)**

---

## ⚠ License and Copyright

**© 2026 Frank L. Adams III. All Rights Reserved.**

This software is proprietary. It is made available for **educational use at the U.S. Army War College only**. Commercial use, redistribution, modification, or use outside the USAWC community is strictly prohibited without prior written permission from the author.

See [LICENSE.txt](LICENSE.txt) for full terms.

For commercial licensing inquiries: **fl16stuff@gmail.com**

---

## What This Is

A browser-based Common Operating Picture built for the **Flight of the Eagle** 1809 Danube Campaign wargame at the U.S. Army War College. It allows players and umpires to:

- Track all French and Austrian unit positions on a real map of Bavaria
- Issue movement orders with **road-network distance calculations** matching the game rules
- Calculate accurate ETAs based on period march rates along actual 1809 roads
- Monitor contact between opposing forces automatically
- View the full 1809 Order of Battle hierarchy
- Overlay georeferenced period maps from the campaign era

---

## Files in This Repository

| File | Description |
|---|---|
| `bavaria_cop_leaflet.html` | The application — open this in Chrome |
| `game_map_georef.jpg` | Pratzen-style Bavaria 1809 tactical map — georeferenced |
| `alps_map_georef.jpg` | Thiers/Dufour Carte des Alpes 1809 — georeferenced |
| `rhine_danube_map_georef.jpg` | Thiers/Dufour Carte No. 29 Rhine-Danube — georeferenced |
| `Bavaria_COP_1809_User_Guide.pdf` | Full user guide |
| `Bavaria_COP_1809_Icon.png` | App icon |
| `LICENSE.txt` | Proprietary software license |
| `README.md` | This file |

> **Important:** All four files (HTML + three JPGs) must be in the same folder for the period map overlays to work.

---

## How to Open It

1. Download all files to the **same folder** on your computer
2. Open **Chrome** or **Edge**
3. Drag `bavaria_cop_leaflet.html` into the browser window
4. The map loads centered on the Bavaria 1809 theater

> An internet connection is required on first open to load the OpenStreetMap base tiles. The period map overlays (JPG files) load from your local folder and work offline immediately.

---

## Key Features

### 🛣 Road Network Distance Calculator
All march distances are calculated along the **1809 period road network** — not straight lines. The app uses Dijkstra's shortest-path algorithm through a hand-built road graph matching the game map. ETAs match what your umpire calculates.

**Verified key distances:**

| Route | Road Distance | Via |
|---|---|---|
| Straubing → Regensburg | 44 km | Wörth an der Donau → Barbing |
| Regensburg → Abensberg | 32 km | Kelheim |
| Regensburg → Landshut | 70 km | Eggmühl → Schierling → Mallersdorf |
| Ingolstadt → Landshut | 64 km | Mainburg → Pfeffenhausen |
| Straubing → Passau | 93 km | Geiselhöring → Plattling → Deggendorf |
| Donauwörth → Regensburg | 102 km | Neuburg → Ingolstadt → Kelheim |

### 📜 Period Map Overlays
Three georeferenced historical maps toggle from the header dropdown:
- **Game Map** — Pratzen-style Bavaria 1809 tactical map
- **Alps 1809** — Thiers/Dufour strategic theater map
- **Rhine-Danube** — Napoleon's western approach axis (Carte No. 29)

### ⚔ NATO Unit Symbols
Blue rectangle = Friendly. Red diamond = Enemy. Toggle perspective between FRENCH and AUSTRIAN with one click — all symbols flip instantly.

### 📋 Order of Battle
Full 1809 OOB pre-loaded. Fully editable — reassign units, or reset to historical with one click.

### ⚠ Contact Detection
Automatic alerts at 25 km (contact), 5 km (engagement), and when routes are converging (projected contact).

### 🕐 Game Clock
Advance manually or play at 1×, 5×, 30×, or 60× speed. Units animate along road routes as the clock runs.

---

## Pre-Loaded Starting Positions — 16 APR 1809 at 0600

| Unit | Location | Faction |
|---|---|---|
| Napoleon | Donauwörth | French — Army HQ |
| Davout HQ, Morand, Saint-Hilaire, Gudin, Friant, Demont, Montbrun, Saint-Sulpice | Regensburg | French — III Corps |
| Vandamme HQ, Württemberg Cav, Württemberg Inf, Nansouty | Weihmichl | French — VIII Corps |
| Hiller | Landshut | Austrian — VI Corps |
| Archduke Charles HQ, Hohenzollern, Rosenberg, Bellegarde, FML von Kienmayer | Straubing | Austrian — Hauptarmee |

---

## March Speeds

| Unit Type | Speed |
|---|---|
| Napoleon / Army HQ courier | 8 km/hr |
| French / Austrian Cavalry HQ | 5 km/hr |
| French Cavalry | 5 km/hr |
| French Line Infantry | 4 km/hr |
| Austrian Cavalry | 4 km/hr |
| Austrian Infantry | 3 km/hr |

---

## Tips for Classroom Use

- **Umpire** uses this as the master COP — update positions as written reports come in
- **Players** use it to plan move orders and calculate ETAs before submitting to the umpire
- The **road path display** shows exactly which towns a unit marches through (e.g. "via Kelheim → Abensberg")
- Use **PLAY at 30×** to fast-forward and see where units will be at a given time
- **Movement Log** in the INTEL tab records all actions — useful for after-action review
- **Contact alerts** fire automatically when opposing forces close within range

---

## Technical Notes

- Built with **Leaflet.js 1.9.4** and **OpenStreetMap** tiles
- Road network routing uses **Dijkstra's shortest-path algorithm**
- Period maps georeferenced using affine transforms from known anchor points
- GPS distances calculated using the **Haversine formula**
- Single HTML file — no server, no installation, no framework dependencies
- Tested in Chrome and Edge

---

## Credits

Built for the **Flight of the Eagle — 1809 Danube Campaign** wargame at the U.S. Army War College, Carlisle Barracks, Pennsylvania.

**Historical sources:**
- John H. Gill, *From Abensberg to Znaim: the Franco-Austrian War of 1809* (USAWC monograph, v.2, January 2026)
- Jay Luvaas, *Napoleon on the Art of War* (The Free Press, 1999)
- Napoleon's Historical Correspondence, Germany and Italy 1809
- Flight of the Eagle Umpire Reference V4

**Map sources:**
- Period map overlays: Thiers/Dufour, *Histoire du Consulat et de l'Empire* (Paulin, Paris, c.1845–1862) — public domain, georeferenced by Frank L. Adams III
- OpenStreetMap © OpenStreetMap contributors (ODbL)

---

*This tool is for educational use in support of USAWC professional military education.*

**Bavaria COP 1809 © 2026 Frank L. Adams III. All Rights Reserved.**
