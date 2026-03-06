# "Popcorn Ball" Electrode — Intumescent Carbon Foam

**A novel electrode fabrication method for flow batteries using hardware store materials.**

This electrode is designed to bond directly to the membrane from the [membrane guide](../membrane/).

Inspired by [Night Hawk in Light's](https://youtube.com/@NightHawkInLight) intumescent coating and Starlite demonstrations. Pyrolysis concepts informed by [Cody's Lab](https://youtube.com/@CodysLab).

---

## The Problem

Commercial flow batteries use carbon felt electrodes ($20-50+ per sheet, specialty supplier only) or graphite plates. These work great but they're expensive, hard to source, and they just sit against the membrane — point contact relying on mechanical pressure. The interface resistance between a pressed felt sheet and a membrane is always a limiting factor.

## Our Solution

Mix water-soluble sacrificial materials (Elmer's glue + cornstarch) with PVC cement and ground ion exchange resin. Paint it directly on the membrane. Torch it. The cornstarch puffs into intumescent carbon foam — little "popcorn balls" of porous carbon chemically bonded to the membrane surface.

**The electrode forms IN SITU on the membrane.** Intimate chemical bond through PVC cement. Zero interface gap. This is fundamentally better contact than pressing a separate material against the membrane.

---

## The Science — Three Porosity Mechanisms

The magic is that this process is **self-correcting**. Three independent mechanisms create porosity, and they compensate for each other:

### Mechanism 1: Emulsion Drying
Elmer's glue is water-based. PVC cement is MEK/THF-based. They're **immiscible** — when you mix them, water droplets suspend in the solvent phase. MEK boils at 80°C, THF at 66°C, water at 100°C. The solvents flash off first, PVC starts setting around the water droplets. The water evaporates later, leaving **pores where the droplets were**.

### Mechanism 2: Intumescent Torching
When you hit cornstarch with a propane torch, it carbonizes and **expands** — the same principle as intumescent fire coatings and Night Hawk's Starlite material. The starch puffs into carbon foam almost instantly. The expanding carbon layer is an excellent thermal insulator, which **protects the membrane underneath from the heat**. The stainless steel screen also diffuses the direct flame.

### Mechanism 3: Acid Dissolution
Whatever cornstarch and Elmer's glue didn't fully carbonize... both are water-soluble. When you fill the cell with acidic electrolyte (pH 1-2 HCl), the unreacted organic material **dissolves out**, leaving behind additional flow channels for electrolyte access to the membrane.

### Self-Correcting Balance

| Torch too much | Torch too little | Just right |
|----------------|-----------------|------------|
| More carbon formed | Less carbon formed | Both mechanisms active |
| Less material dissolves out | More material dissolves out | Balanced porosity |
| Porous from puffing | Porous from dissolution | Maximum performance |

**You can't lose.** The torch technique doesn't need to be precise because the acid cleanup handles whatever the heat missed.

---

## Electrochemical Design — The Transition Gradient

The electrode must conduct BOTH electrons (from the screen to reaction sites) AND ions (from the membrane to reaction sites). But the membrane must conduct ions ONLY — any electronic conductivity in the membrane would short-circuit the cell.

Our design creates a natural gradient:

```
Screen (electrons only)
  → Popcorn ball layer (electrons via carbon + ions via SAC resin)
    → PVC cement interface (ions via SAC resin — NO carbon here)
      → Membrane (ions ONLY — pure SAC resin + PVC cement)
```

**Critical rule:** No carbon at or near the membrane interface. Carbon is an electronic conductor. The transition from mixed conductor (electrode) to pure ionic conductor (membrane) is what forces electrons into the external circuit. The PVC cement + SAC resin in the popcorn mix naturally provides this transition — the carbon puffs UP (away from the membrane) while the PVC cement bonds DOWN (to the membrane).

---

## Materials

| Material | Source | Cost | Buy |
|----------|--------|------|-----|
| Elmer's white glue | Walmart | ~$3 | [Amazon](https://www.amazon.com/s?k=elmers+white+glue&tag=chipmonkeysof-20) |
| Cornstarch | Grocery | ~$2 | [Amazon](https://www.amazon.com/s?k=cornstarch&tag=chipmonkeysof-20) |
| PVC cement (clear) | Home Depot | ~$6 | [Amazon](https://www.amazon.com/dp/B001D9WRWG?tag=chipmonkeysof-20) |
| Ground SAC resin | [See membrane prep](../membrane/) | — | — |
| SS window screen 18 mesh | Hardware store | ~$15 | [Amazon](https://www.amazon.com/dp/B09TGDRFKZ?tag=chipmonkeysof-20) |
| Activated charcoal | Pet shop | ~$8/lb | [Amazon](https://www.amazon.com/dp/B01GN7ZQ70?tag=chipmonkeysof-20) |
| Propane torch | Hardware store | ~$15 | [Amazon](https://www.amazon.com/s?k=propane+torch+bernzomatic&tag=chipmonkeysof-20) |
| Candle (for soot) | Dollar store | ~$1 | — |

*As an Amazon Associate I earn from qualifying purchases.*

---

## Recipe

**Bowl A:** Elmer's white glue + cornstarch — mix to thick paste

**Bowl B:** PVC cement (clear) + ground SAC resin powder — mix

**Combine A into B** — stir vigorously. A water-in-solvent emulsion forms automatically because the water phase (Elmer's) and solvent phase (PVC cement) are immiscible. This is the emulsion that creates Mechanism 1 porosity.

---

## Process — Step by Step

### 1. Screen Prep
- Run the stainless steel screen over a candle flame to **soot-blacken** it
- This creates a carbon coating on the metal wires — better carbon-to-carbon contact with the electrode
- Cut to size for your cell

### 2. Application — Membrane Faces
- Paint the mixed slurry onto the **fully cured membrane** surface, ~1-2mm thick
- Press the soot-blackened screen into the wet layer
- The PVC cement in the mix chemically welds to the PVC cement in the membrane
- The screen mesh embeds in the slurry — mechanical grip + chemical bond

### 3. Application — Box Interior Walls
- Paint the same slurry on **all interior walls** of the ASA box
- PVC cement welds to ASA the same way it welds to the membrane
- Every interior surface becomes active electrode area

### 4. Drying
- Let dry completely — outdoors or in well-ventilated area (PVC cement fumes are MEK/THF)
- During drying, Mechanism 1 activates: solvents flash off, water evaporates later, pores form
- Full cure: 12-24 hours

### 5. Torching
- Propane torch from the **screen side**
- Quick passes — not sustained heat in one spot
- The cornstarch puffs into carbon foam almost immediately (Mechanism 2)
- The intumescent foam insulates the membrane from further heat
- The screen diffuses direct flame — no hot spots
- You'll see the surface puff and darken — that's the popcorn balls forming

### 6. Cavity Fill
- Pour **coarse activated charcoal** into the popcorn-coated box cavity
- The charcoal contacts the conductive popcorn layer on the walls, extending the electron network through the entire cavity volume
- Grate bars at the flow ports retain the fill
- Don't pack tight — the gaps between granules ARE the electrolyte flow channels

### 7. Assembly
- Glue the box halves onto the MEA with PVC cement at the landscape fabric overhang
- Connect vinyl tubing to ports
- Fill with electrolyte — Mechanism 3 activates as unreacted organics dissolve

---

## Why Electrolyte Must Reach the Membrane

This is critical to understand. The membrane needs **liquid electrolyte physically touching its surface** to conduct ions. If you pack solid material against the membrane with no gaps, you starve the ion transport and the cell dies.

The popcorn ball structure solves this naturally:
- **Carbon balls** provide electron conduction and reaction surface
- **Gaps between balls** allow electrolyte to reach the membrane
- **Resin particles** in the mix provide ion conduction shortcuts

The charcoal fill in the cavity works the same way — loose granules with electrolyte-filled gaps between them.

---

## Future: Pyrolyzed 3D Printed Electrodes

The cavity fill can be upgraded from loose charcoal to custom-geometry carbon structures:

1. **Design** electrode geometry in Fusion 360 (gyroid, honeycomb, lattice)
2. **Print** in PLA (cheap, best fine detail, doesn't need to survive — it's sacrificial)
3. **Soak** in concentrated sugar water — sugar wicks into every crevice
4. **Pyrolyze** in a sealed steel pipe (campfire, fire pit, or charcoal chimney starter)
   - PLA decomposes and vents as gas
   - Sugar converts to carbon (~25% yield), maintaining the 3D geometry
   - The sealed pipe IS the inert atmosphere — limits oxygen
5. **Result:** Carbon electrode with precisely designed 3D flow geometry

### Why This Could Be Better Than Carbon Felt

| | Carbon felt | Pyrolyzed 3D print |
|---|---|---|
| Surface area | 1-10 m²/g | Controlled by geometry |
| Flow channels | Random fiber orientation | Designed in CAD |
| Reproducibility | Batch-to-batch variation | Identical every print |
| Cost | $20-50/sheet | Pennies (PLA + sugar) |
| Customizable | No | Parametric — change one number |

### Community Electrode Challenge

We test community-submitted electrode geometries on the [YouTube channel](https://youtube.com/@ChipMonkeysOffGrid). Submit your STL as a pull request to [community-designs/](community-designs/). Design something, we'll carbonize it and test it. Best designs get featured.

Pyrolysis technique inspired by [Cody's Lab](https://youtube.com/@CodysLab). Gyroid geometry concepts from [Makers Muse](https://youtube.com/@MakersMuse).
