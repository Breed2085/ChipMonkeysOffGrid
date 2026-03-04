# ChipMonkeys Off Grid

**Open-source off-grid power, water purification, and homestead systems built entirely from hardware store materials.**

We're moving to Tennessee to homestead and we need to solve three problems: store power, purify water, and do it all without a monthly bill. Everything here is designed to be built by one person in a garage with a 3D printer, a propane torch, and a trip to Home Depot. No specialty lab equipment. No Nafion membranes. No $200/liter vanadium electrolyte.

Can we pull it off with table salt, scrap iron, and PVC cement? Yeah. We got this.

---

## What's Here

| Project | Status | Description |
|---------|--------|-------------|
| [Flow Battery](flow-battery/) | **Active** | All-iron redox flow battery — stores energy in liquid electrolyte |
| [Membrane](membrane/) | **Active** | DIY ion exchange membranes from ground resin beads + PVC cement |
| [Electrode](electrode/) | **Active** | "Popcorn Ball" intumescent carbon foam electrode — our novel contribution |
| [Electrolyte](electrolyte/) | **Active** | Ferrous chloride from scrap iron + hydrochloric acid |
| [SEM Cell](sem-cell/) | Planned | Salt Electro Mining — make your own HCl and NaOH from table salt |
| [ED Water](ed-water/) | Planned | Electrodialysis water purification — $100 vs $4,000 conventional |
| [Store](store/) | Planned | Kit sales and e-commerce |

---

## The All-Iron Flow Battery

A flow battery stores energy in liquid electrolyte, not in solid electrodes like lithium. The liquid is pumped through electrochemical cells where the reactions happen. Separate the power (cell size) from the energy (tank size) — want more runtime? Get bigger tanks. Want more watts? Add more cells. They're independent.

### The Chemistry

Both sides use the same base electrolyte: **ferrous chloride (FeCl₂) dissolved in hydrochloric acid**.

- **Positive side:** Fe²⁺ ↔ Fe³⁺ + e⁻ (iron stays dissolved, changes oxidation state)
- **Negative side:** Fe²⁺ + 2e⁻ ↔ Fe⁰ (iron plates as metal during charge, dissolves during discharge)
- **Cell voltage:** ~1.2V open circuit, ~1.0-1.1V under load
- **Round-trip efficiency:** 70-80%

### Why All-Iron Beats Everything Else for DIY

| Feature | All-Iron | Vanadium | Lithium |
|---------|----------|----------|---------|
| Electrolyte cost | Free (scrap iron + salt) | $150-200/liter | N/A (solid) |
| Toxic materials | No | Yes (V₂O₅) | Yes (cobalt, fluoride) |
| Membrane crossover | Self-healing | Capacity loss | N/A |
| Cycle life | Unlimited | 10,000+ | 500-2,000 |
| Fire risk | Zero | Low | High |
| DIY difficulty | Hardware store | Specialty chemicals | Don't try it |

The self-healing property is key: since both sides use the same iron electrolyte, if ions cross the membrane, they just end up where they started. No permanent damage, no capacity fade from crossover. Vanadium flow batteries lose capacity when the membrane leaks. Ours doesn't care.

### The Cell Architecture

Two identical 3D-printed ASA boxes glued face-to-face onto a flat membrane electrode assembly (MEA). No gaskets, no bolts through the cell, no complex frame geometry. The box IS the flow chamber, current collector housing, and structural support.

```
┌─────────────────────────────────────────┐
│  ASA Box (popcorn-coated walls)         │
│  ┌───────────────────────────────────┐  │
│  │  Coarse activated charcoal fill   │  │
│  │  ┌─────────────────────────────┐  │  │
│  │  │ SS Screen (soot-blackened)  │  │  │
│  │  │ ┌───────────────────────┐   │  │  │
│  │  │ │ Popcorn Ball Electrode│   │  │  │
│  │  │ └───────────────────────┘   │  │  │
│  │  └─────────────────────────────┘  │  │
│  └───────────────────────────────────┘  │
├─────────────────────────────────────────┤
│          MEMBRANE (ion gate)            │
│   landscape fabric + SAC resin + PVC    │
├─────────────────────────────────────────┤
│  ┌───────────────────────────────────┐  │
│  │ Popcorn Ball Electrode            │  │
│  │  ┌─────────────────────────────┐  │  │
│  │  │ SS Screen (soot-blackened)  │  │  │
│  │  └─────────────────────────────┘  │  │
│  │  Coarse activated charcoal fill   │  │
│  └───────────────────────────────────┘  │
│  ASA Box (popcorn-coated walls)         │
└─────────────────────────────────────────┘
```

### Key Design Decisions

- **ASA, not PLA:** PVC cement chemically welds to ASA (MEK/THF dissolves the surface). PLA does not bond — cement just sits on top and peels off. Every seal, coating, and bond in this system relies on PVC cement fusion.
- **Both boxes are identical:** One STL file. No left/right, no sorting, no labeling.
- **No gaskets or O-rings:** PVC cement chemical bonds + landscape fabric overhang = zero leak paths.
- **Terminals in the sealed zone:** Threaded holes in the box wall overlap the mesh in the glued/sealed zone — screws bite into the stainless screen but never penetrate the electrolyte cavity. Zero leak path at the terminals.
- **Open pocket with charcoal fill:** No serpentine maze channels. The charcoal granules create micro-turbulence and provide massive electrode surface area. The charcoal IS the flow distributor.

### Cell Specs

| Parameter | 50mm Test Cell | 300mm Production |
|-----------|---------------|-----------------|
| Active area | 25 cm² | 900 cm² |
| Power per cell @ 50mA/cm² | ~1.25W | ~49W |
| Power per cell @ 80mA/cm² | — | ~79W |
| Materials cost per cell | ~$0.72 | ~$5-8 |
| Print time (0.2mm layers) | ~10 min | ~45-60 min |
| Both sizes print on | VzBot 400 (400mm bed) | VzBot 400 |

**Phase 1 target:** 4 cells at 50mm = self-sustaining stack that powers its own pump and charges a phone. Total BOM: ~$150.

---

## The Electrode Innovation — "Popcorn Balls"

This is our novel contribution to the DIY flow battery space. Traditional approaches use expensive carbon felt ($20-50/sheet) or graphite plates. We use **cornstarch, Elmer's glue, PVC cement, and ground ion exchange resin** — mixed, painted on, and torched.

The cornstarch puffs into intumescent carbon foam (like Night Hawk in Light's Starlite material), creating a porous, conductive electrode with **three self-correcting porosity mechanisms:**

1. **Emulsion drying** — Elmer's (water-based) mixed into PVC cement (MEK-based) creates an immiscible emulsion. MEK flashes off first, water evaporates later, leaving pores.
2. **Intumescent torching** — Cornstarch carbonizes and puffs into foam. The expanding carbon layer insulates the membrane from heat (same principle as fire-retardant coatings).
3. **Acid dissolution** — Whatever didn't carbonize (unreacted starch, Elmer's) dissolves when the cell fills with acid electrolyte, creating additional flow channels.

Over-torch = more carbon. Under-torch = more dissolves. **Either way you get a porous, conductive electrode. Can't lose.**

The electrode forms directly on the membrane surface — intimate chemical bond through PVC cement, zero interface gap. This is fundamentally better contact than pressing a separate carbon felt sheet against a membrane.

Full recipe and process: [electrode/](electrode/)

---

## The Membrane — Rowow Method

Based entirely on [Rowow's](https://youtube.com/@Rowow) open-source ion exchange membrane technique. Ground commodity ion exchange resin beads (the same ones used in aquarium water filters) mixed 50/50 with PVC cement, painted onto landscape fabric. The sulfonic acid groups on the resin particles swell in water and form ion-conducting pathways through the PVC matrix.

This replaces Nafion ($500-1,000/m²) with a membrane that costs about $0.10 per cell from hardware store materials.

Full fabrication process: [membrane/](membrane/)

---

## The Electrolyte — Scrap Iron + Acid

Buy muriatic acid at Home Depot ($8/gallon). Drop scrap iron in it. Wait 24 hours. You have battery electrolyte.

Or make the acid yourself from table salt and electricity using a SEM (Salt Electro Mining) cell — same Rowow membrane, graphite electrodes, saturated brine, 12V DC. The byproduct (NaOH/lye) is worth $170-330 per batch.

Full details: [electrolyte/](electrolyte/) | [sem-cell/](sem-cell/)

---

## Water Purification — Electrodialysis

Same Rowow membrane technique, different resin type (anion beads instead of cation). Alternating membranes in an electric field pull ions out of water. Combined with activated charcoal channels and UV sterilization: **complete drinking water system for $100-150** vs $1,500-4,000 conventional.

Full details: [ed-water/](ed-water/)

---

## Materials — Everything From Hardware Store / Amazon

| Material | Where | What It Does | Cost |
|----------|-------|-------------|------|
| Mixed bed DI resin | [Amazon](https://www.amazon.com/dp/B07L4YX52J?tag=chipmonkeysof-20) | Ground into powder for membranes + electrodes | ~$25/5lb |
| PVC cement (clear) | [Amazon](https://www.amazon.com/dp/B001D9WRWG?tag=chipmonkeysof-20) | Universal binder — welds ASA, bonds membrane, seals tubing | ~$6/16oz |
| SS window screen 18 mesh | [Amazon](https://www.amazon.com/dp/B09TGDRFKZ?tag=chipmonkeysof-20) | Current collector, electrode backbone | ~$15 |
| Activated charcoal | [Amazon](https://www.amazon.com/dp/B01GN7ZQ70?tag=chipmonkeysof-20) | High surface area electrode fill | ~$8/lb |
| Landscape fabric (non-woven) | [Amazon](https://www.amazon.com/dp/B0BQD91HH9?tag=chipmonkeysof-20) | Membrane reinforcement + gasket + insulator | ~$15 |
| ASA filament 1.75mm | [Amazon](https://www.amazon.com/dp/B09DKPYYBP?tag=chipmonkeysof-20) | 3D printed cell boxes | ~$22/kg |
| Cornstarch | Grocery | Intumescent carbon electrode ("popcorn balls") | ~$2 |
| Elmer's white glue | Walmart | Sacrificial pore former in electrode emulsion | ~$3 |
| Muriatic acid 31% HCl | [Amazon](https://www.amazon.com/dp/B01LYNZA7Z?tag=chipmonkeysof-20) | Electrolyte acid (or make your own via SEM) | ~$8/gal |
| Scrap mild steel | Garage | Iron source for electrolyte | Free |
| Table salt | Grocery | SEM cell feedstock for acid + lye production | ~$1/lb |
| Graphite powder | [Amazon](https://www.amazon.com/dp/B0CL4QLS25?tag=chipmonkeysof-20) | Conductive filler | ~$12/lb |

*As an Amazon Associate I earn from qualifying purchases.*

Full BOM with all links: [flow-battery/bom/50mm-test-cell.md](flow-battery/bom/50mm-test-cell.md)

---

## Standing on the Shoulders of

This project wouldn't exist without the open-source work and inspiration of these people. We credit them by name because that's how open source should work.

- **[Rowow](https://youtube.com/@Rowow)** — Invented the open-source ion exchange membrane technique that makes this entire project possible. Ground resin beads + PVC cement = working membrane from hardware store materials. [GitHub](https://github.com/Rowow1/Open-sourced-off-the-shelf-ion-exchange-membrane) | [Website](https://rowow.net)
- **[Night Hawk in Light](https://youtube.com/@NightHawkInLight)** — His intumescent coating and Starlite demonstrations directly inspired our "popcorn ball" electrode method. The puffing carbon foam that protects the membrane from torch heat? That's his principle applied to electrochemistry.
- **[Cody's Lab](https://youtube.com/@CodysLab)** — Pyrolysis and materials science inspiration for our carbonized 3D-printed electrode work.
- **[FBRC](https://fbrc.dev)** — Open-source flow battery community and design files.
- **[Chemisting](https://chemisting.com)** — Daniel's detailed documentation of DIY flow battery builds.
- **[Cayrex2](https://youtube.com/@Cayrex2)** — 5-part vanadium flow battery build series showing what's possible.

---

## Watch the Build

**YouTube: [ChipMonkeys Off Grid](https://youtube.com/@ChipMonkeysOffGrid)**

Follow the entire journey from first test cell to full Tennessee homestead power system. Every build step documented. Every failure shown. Every file free.

---

## Get a Kit

**[chipmonkeysinc.com/offgrid](https://chipmonkeysinc.com/offgrid)**

Everything is open source — build it yourself from the files here. Or buy a kit with pre-measured, pre-ground materials and save yourself the prep time:

- **Materials Kit** ($25-40) — Pre-measured resin, graphite, charcoal, fabric
- **Pre-made MEAs** ($10-15 each) — Cast, torched, ready to glue into your boxes
- **Assembled Cells** ($30-50) — Complete, just add electrolyte
- **Electrolyte Concentrate** ($20-30/gal) — Ready to dilute and use

---

## Safety

This project involves acid, solvents, open flame, and gas generation. Respect the chemistry.

- **Acid (pH 1-2):** Chemical-resistant nitrile gloves and splash-proof goggles. Baking soda nearby for spill neutralization. Rinse skin contact immediately with water.
- **PVC cement fumes:** MEK and THF solvents. Always work in ventilated area or outdoors. Don't breathe this stuff.
- **Chlorine gas (SEM cell only):** The anode produces chlorine. Run SEM cells **outdoors ONLY**. If you smell "swimming pool," move upwind immediately.
- **Hydrogen gas:** Released during charging and iron dissolution. Never seal a cell or container airtight. No flames near the electrolyte.
- **Torching electrodes:** Outdoors on a fire-safe surface. Keep an extinguisher handy. The torch step takes seconds, not minutes.

---

## License

**CERN Open Hardware License v2 — Strongly Reciprocal (CERN-OHL-S-2.0)**

You can build, modify, and sell hardware based on these designs. If you distribute modified versions, you must share your changes under the same license. That's the deal — keep it open.

## Contributing

Build one. Break one. Tell us what happened. Open an issue or pull request. See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

We run a community electrode challenge — submit your 3D-printable electrode geometry STL and we'll test it on the YouTube channel. See [electrode/community-designs/](electrode/community-designs/).

---

*ChipMonkeys Inc. — Indiana C-Corp*
