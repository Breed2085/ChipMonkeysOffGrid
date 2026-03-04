# All-Iron Flow Battery

## How It Works

A flow battery stores energy in liquid electrolyte that's pumped through electrochemical cells. The power (watts) comes from the cell stack size. The energy (watt-hours) comes from the tank volume. They're independent — want more runtime? Bigger tanks. More watts? More cells. No other battery architecture gives you this.

### The Reactions

Both half-cells use **ferrous chloride (FeCl₂) in dilute HCl** (pH 1-2):

**Positive half-cell (stays dissolved):**
```
Fe²⁺ → Fe³⁺ + e⁻    (charge)
Fe³⁺ + e⁻ → Fe²⁺    (discharge)
```
Solution changes from pale green (Fe²⁺) to yellow/brown (Fe³⁺) during charge.

**Negative half-cell (plates/dissolves):**
```
Fe²⁺ + 2e⁻ → Fe⁰    (charge — iron plates as metal)
Fe⁰ → Fe²⁺ + 2e⁻    (discharge — metal dissolves back)
```

**Cell voltage:** ~1.2V open circuit, ~1.0-1.1V under load
**Round-trip efficiency:** 70-80%

### The Diode Film (Membrane)

The wall between the two half-cells is a **cation diode film** — we call it that because it works like a diode in electronics. It only lets positive ions (H⁺, Fe²⁺) pass through while blocking electrons. This forces the electrons to take the long way around through the external circuit — and that's your usable electricity. Without this one-way ion gate, the cell would just short-circuit internally. Full explanation of cation vs anion diode films: [membrane/](../membrane/)

### Why All-Iron Is Self-Healing

Both sides use the same base electrolyte. If Fe²⁺ ions cross the diode film (membrane crossover), they just end up in the other tank — still usable, no permanent damage. Vanadium flow batteries permanently lose capacity from crossover. All-iron doesn't care. This is why a DIY diode film works here when it wouldn't work for vanadium.

---

## Cell Architecture — "Fuel Cell v1"

### The Box

Each cell is two identical 3D-printed ASA boxes glued to opposite faces of a flat membrane electrode assembly (MEA). No gaskets, no bolts through the cell, no complex frame geometry.

**Box features:**
- **Interior pocket:** ~50×50mm active area (25 cm² for test cell)
- **Pocket depth:** ~13mm (fits 1/4" vinyl tubing through side walls)
- **Wall material:** ASA filament, all interior surfaces coated with popcorn ball electrode mix
- **Hose ports:** 1/4" ID vinyl tubing (3/8" OD) glued directly into holes with PVC cement — zero fittings
- **Flow pattern:** Two diagonal corners in, two diagonal corners out (X-pattern)
- **Grate bars:** Printed along inlet/outlet edges, 1mm gap, distributes flow and retains charcoal
- **Both boxes per cell are IDENTICAL** — one STL, print two, no sorting needed

### Terminal Design — Sealed Zone Thread

This is a key innovation. The terminal screws **never penetrate the electrolyte cavity:**

```
[ELECTROLYTE CAVITY]      [SEALED GLUE ZONE]      [OUTSIDE]
                          ┌──────────────────┐
  wet area                │  PVC cement seal  │
  ──mesh extends──────────│──mesh continues───│──────
  ──membrane──────────────│──membrane sealed──│
                          │                   │
                          │  ↑ screw threads  │  ← stud from outside
                          │  bite into mesh   │
                          │  in sealed zone   │
                          └──────────────────┘
```

- Threaded hole modeled into the box wall in the **sealed/glued zone**
- Membrane and mesh are fully sealed with PVC cement in that zone
- Screw threads press into the mesh, carve through PVC coating to make bare metal contact
- **Zero leak path** — the screw never sees electrolyte
- Add as many bus bar stud locations as needed along the sealed perimeter
- Multiple connection points per cell for lower resistance and voltage monitoring
- Landscape fabric layer prevents screws from shorting to the opposite electrode

### Interior Treatment

Every interior surface is coated with the [popcorn ball electrode mix](../electrode/), torched, then the cavity is filled with coarse activated charcoal:

1. Paint popcorn mix on all walls → PVC cement welds to ASA
2. Torch → cornstarch puffs into conductive carbon foam
3. Fill with coarse charcoal → contacts popcorn coating on walls
4. The entire cavity volume becomes active electrode

---

## Cell Specs

| Parameter | 50mm Test Cell | 300mm Production |
|-----------|---------------|-----------------|
| Active area | 25 cm² | 900 cm² |
| Power per cell @ 50mA/cm² | ~1.25W | ~49W |
| Power per cell @ 80mA/cm² | ~2W | ~79W |
| Materials cost per cell | ~$0.72 | ~$5-8 |
| Print time (0.2mm layers) | ~10 min | ~45-60 min |
| Printer | VzBot 400 | VzBot 400 |

**Demo target:** 4 cells × 1.2V = 4.8V stack → boost converter → charges a phone. Stack powers its own peristaltic pump (~0.5W) with power to spare.

---

## Plumbing

- **Cell connections:** 1/4" ID vinyl tubing, PVC cemented into box wall holes
- **Manifold:** 1/2" PVC pipe with holes for vinyl branch stubs, PVC cemented
- **Flow pattern:** X-pattern (diagonal in/out) — charcoal fill creates micro-turbulence
- **Zero fittings** — everything PVC cement welded
- **Total plumbing cost:** ~$5-8 for entire stack

### Pump Options

| Scale | Pump | Power | Cost |
|-------|------|-------|------|
| 50mm demo (3-4 cells) | Micro peristaltic 3-5V | 0.5W | $3-5 |
| 50mm extended (12-20 cells) | Micro submersible | 0.5-1.5W | $3-5 |
| 300mm production | Ceramic mag drive 12V | 5-19W | $15-20 |

**Strategy:** Peristaltic pumps for now — simple, self-priming, no wetted parts. Mag drive upgrade later if flow rate becomes the bottleneck at 300mm scale.

### Self-Sustaining Cell Bundles

3 cells minimum to power a 3V micro pump (~0.5W overhead). 12 cells at 50mm scale: 15W total, pump draws 0.5W, 14.5W usable output.

---

## Print Settings (ASA)

| Parameter | Value |
|-----------|-------|
| Nozzle temp | 240-260°C |
| Bed temp | 100-110°C |
| Enclosure | **Required** (ASA warps without it) |
| Layer height | 0.2mm |
| Nozzle diameter | 0.4mm |
| Minimum feature | ~1mm (0.5mm gaps bridge closed) |
| Printer | VzBot 400 (400mm bed) or any enclosed printer |

**Why ASA and not PLA:** PVC cement chemically welds to ASA — the MEK/THF solvents dissolve the surface and fuse the materials. PLA does not dissolve in these solvents. The cement just sits on top and peels off. Every bond in this system relies on PVC cement chemical fusion. Use PLA only for test-fitting dimensions.

---

## Files

- `designs/` — Fusion 360 source files (parametric — scale with one dimension change)
- `stl/` — Ready-to-print STL files
- `bom/` — [Bill of materials with Amazon links](bom/50mm-test-cell.md)
- `docs/` — Build instructions

---

## Scaling

The 50mm test cell exists to prove the concept and tune the electrode recipe. The 300mm production cell is the same architecture scaled up — same STL with different dimensions, same membrane recipe, same electrode process, same plumbing approach. Both sizes print on the VzBot 400.

**50mm → 300mm means:**
- 36x the active area (25 cm² → 900 cm²)
- ~40-63x the power per cell
- Same number of print/assembly steps per cell
- Larger electrolyte tanks (5-gallon buckets)
- Mag drive pump instead of peristaltic

The design is parametric in Fusion 360 — change one dimension and everything scales.
