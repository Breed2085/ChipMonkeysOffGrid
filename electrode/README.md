# "Popcorn Ball" Electrode — Intumescent Carbon Foam

A novel electrode fabrication method inspired by [Night Hawk in Light's](https://youtube.com/@NightHawkInLight) intumescent coating and Starlite demonstrations.

## The Concept

Mix water-soluble sacrificial materials (Elmer's glue + cornstarch) with PVC cement and ground ion exchange resin. Paint it on, torch it. The cornstarch puffs into carbon foam ("popcorn balls") with three porosity mechanisms that are self-correcting.

## Materials

| Material | Source | Cost |
|----------|--------|------|
| Elmer's white glue | Walmart | ~$3 |
| Cornstarch | Grocery | ~$2 |
| PVC cement (clear) | Home Depot | ~$6 |
| Ground SAC resin | [See membrane prep](../membrane/) | — |
| SS window screen (18x16) | Hardware store | ~$8-15/roll |
| Propane torch | Hardware store | ~$15 |
| Candle | Dollar store | ~$1 |

## Recipe

**Bowl A:** Elmer's glue + cornstarch — mix to thick paste

**Bowl B:** PVC cement + ground SAC resin — mix

**Combine A into B** — stir. A water-in-solvent emulsion forms automatically (Elmer's is water-based, PVC cement is MEK/THF-based — they're immiscible).

## Process

### Screen Prep
1. Soot-blacken the stainless screen over a candle (carbon-to-carbon contact)
2. Cut to size

### Application
1. Paint the mixed electrode slurry onto the **cured membrane** faces (~1-2mm thick)
2. Press soot-blackened screen into the wet layer
3. Also paint all **interior box walls** (PVC cement welds to ASA)
4. Let dry completely (outdoors — PVC cement fumes)

### Torch
1. Propane torch from the screen side
2. Quick passes — the cornstarch puffs into carbon foam instantly
3. The intumescent foam protects the membrane from heat (same principle as Starlite)
4. The screen diffuses direct flame — no hot spots

### Fill
1. Pour coarse activated charcoal into the popcorn-coated cavity
2. Charcoal contacts the conductive popcorn layer on walls for electron network
3. Grate bars at flow ports retain the fill

## Three Porosity Mechanisms (Self-Correcting)

| Mechanism | When It Happens | What It Creates |
|-----------|----------------|----------------|
| Emulsion drying | During cure | MEK flashes off first, water later → pores |
| Intumescent puffing | During torching | Cornstarch carbonizes and expands → carbon foam |
| Acid dissolution | When cell is filled | Unreacted starch + Elmer's dissolve in acid → channels |

**Over-torch** = more carbon, less dissolves out. **Under-torch** = more dissolves, more porosity. Either way, you get a porous, conductive electrode. Can't lose.

## Why This Works

- Electrode forms IN SITU on the membrane surface — intimate chemical bond
- PVC cement chemically welds to both membrane AND ASA box walls
- Every cavity surface becomes active electrode area
- Screen is structural skeleton — electrode doesn't need to be self-supporting
- All materials from hardware store / Walmart / grocery store

## Future: Pyrolyzed 3D Printed Electrodes

The cavity fill can be upgraded from loose charcoal to custom-geometry carbon structures:

1. Design geometry in Fusion 360 (gyroid, honeycomb, lattice)
2. Print in PLA
3. Soak in concentrated sugar water
4. Pyrolyze in sealed steel pipe (campfire kiln)
5. Sugar converts to carbon maintaining 3D geometry

See our [YouTube series](https://youtube.com/@ChipMonkeysOffGrid) for testing results comparing different fill geometries.

Pyrolysis technique inspired by [Cody's Lab](https://youtube.com/@CodysLab).
