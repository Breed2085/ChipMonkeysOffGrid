# ChipMonkeys Off Grid

**Open-source off-grid power, water purification, and homestead systems built from hardware store materials.**

We're moving to Tennessee to homestead. We need to store power, purify water, and live off the grid. Can we pull it off with 3D printing, table salt, and scrap iron? Yeah. We got this.

## What's Here

| Project | Status | Description |
|---------|--------|-------------|
| [Flow Battery](flow-battery/) | Active | All-iron flow battery from hardware store materials |
| [Membrane](membrane/) | Active | Open-source ion exchange membranes (Rowow method) |
| [Electrode](electrode/) | Active | "Popcorn Ball" intumescent carbon electrode |
| [Electrolyte](electrolyte/) | Active | FeCl₂ from scrap iron + HCl (or SEM cell) |
| [SEM Cell](sem-cell/) | Planned | Salt Electro Mining — make acid from table salt |
| [ED Water](ed-water/) | Planned | Electrodialysis water purification |
| [Store](store/) | Planned | Kit sales and e-commerce |

## The Flow Battery — Quick Overview

An all-iron redox flow battery stores energy in liquid electrolyte (ferrous chloride in hydrochloric acid). It uses two identical 3D-printed ASA boxes sandwiching a homemade ion exchange membrane. The electrolyte is made from scrap iron and table salt. Total materials cost for a 4-cell demo: ~$150.

**Why this matters:**
- Infinite cycle life — iron doesn't degrade like lithium
- Non-toxic — iron and salt, not cobalt and lithium
- Self-healing — same electrolyte both sides, membrane crossover is harmless
- Scalable — bigger tanks = more energy, more cells = more power
- Dirt cheap — electrolyte is literally free if you have scrap iron

## Standing on the Shoulders of

This project wouldn't exist without the open-source work and inspiration of:

- **[Rowow](https://youtube.com/@Rowow)** — Invented the open-source ion exchange membrane technique using ground resin beads and PVC cement. The foundation of everything here. [GitHub](https://github.com/Rowow1/Open-sourced-off-the-shelf-ion-exchange-membrane) | [Website](https://rowow.net)
- **[Night Hawk in Light](https://youtube.com/@NightHawkInLight)** — Intumescent coating and Starlite demonstrations directly inspired our "popcorn ball" electrode method
- **[Cody's Lab](https://youtube.com/@CodysLab)** — Pyrolysis and materials science inspiration for our carbonized 3D-printed electrode work
- **[FBRC](https://fbrc.dev)** — Open-source flow battery community
- **[Chemisting](https://chemisting.com)** — Daniel's documentation of DIY flow battery builds
- **[Cayrex2](https://youtube.com/@Cayrex2)** — Vanadium flow battery build series

## Watch the Build

**YouTube: [ChipMonkeys Off Grid](https://youtube.com/@ChipMonkeysOffGrid)**

Follow the entire build from first cell to full homestead power system.

## Get a Kit

**[chipmonkeysinc.com/offgrid](https://chipmonkeysinc.com/offgrid)**

Everything is open source. Build it yourself from the files here, or buy a kit with pre-measured materials.

## Materials — All Hardware Store / Amazon

| Material | Source | What It Does |
|----------|--------|-------------|
| Mixed bed DI resin | Amazon | Ground into powder for membranes |
| PVC cement (clear) | Home Depot | Universal binder, bonds to ASA |
| SS window screen (18x16) | Hardware store | Current collector / electrode backbone |
| Activated charcoal | Pet shop | High surface area electrode fill |
| Landscape fabric | Home Depot | Membrane reinforcement + gasket |
| ASA filament | Amazon | 3D printed cell boxes |
| Cornstarch | Grocery | Intumescent carbon electrode ("popcorn balls") |
| Elmer's glue | Walmart | Sacrificial pore former in electrode |
| Muriatic acid | Home Depot | Electrolyte acid (or make your own via SEM) |
| Scrap iron | Garage | Iron source for electrolyte |
| Table salt | Grocery | SEM cell feedstock |

## Safety

- **Acid:** pH 1-2, gloves and eye protection, baking soda nearby for spills
- **PVC cement fumes:** MEK/THF solvents, always ventilated area or outdoors
- **Chlorine gas:** SEM cell anode produces chlorine, run outdoors ONLY
- **Hydrogen gas:** From charging and iron dissolution, never seal airtight, no flames nearby
- **Torching electrodes:** Outdoors, fire-safe surface, keep extinguisher handy

## License

CERN Open Hardware License v2 — Strongly Reciprocal (CERN-OHL-S-2.0)

You can build, modify, and sell hardware based on these designs. If you distribute modified versions, you must share your changes under the same license.

## Contributing

Build one. Break one. Tell us what happened. Open an issue or pull request.

---

*ChipMonkeys Inc. — Indiana C-Corp*
