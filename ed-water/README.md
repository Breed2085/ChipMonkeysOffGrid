# Electrodialysis Water Purification

**A complete guide to building a $100-150 drinking water purification system from Rowow membranes and hardware store materials.**

Remove dissolved metals, salts, minerals, and contaminants from well water or creek water using electricity and diode films — the same films used in the flow battery, plus the anion version.

This guide is written to be followed on camera for YouTube Episode 10.

---

## What You're Building

An electrodialysis (ED) system that pulls ions (dissolved metals, salts, minerals) out of water using an electric field and alternating **diode films**. Combined with activated charcoal filtration and UV sterilization, this is a complete drinking water system.

We call ion exchange membranes "diode films" because they work like a diode — each one only lets specific ions pass through while blocking everything else. A one-way valve at the molecular level. Full explanation in the [membrane guide](../membrane/).

**Total cost: $100-150** vs $1,500-4,000 for conventional well water treatment systems.

---

## How Electrodialysis Works

### The Basics

Imagine a stack of alternating cation and anion diode films with water flowing between them. Apply an electric field across the stack. Each diode film acts like a one-way valve — cation films only let positive ions through, anion films only let negative ions through.

The electric field provides the driving force — it pulls positive ions toward the cathode and negative ions toward the anode. But the diode films control WHICH direction each ion can actually move:

- **Cation diode film (CEM):** Only lets positive ions through (Na⁺, Ca²⁺, Fe²⁺, Mg²⁺) — like a turnstile that only opens for blue wristbands
- **Anion diode film (AEM):** Only lets negative ions through (Cl⁻, SO₄²⁻, NO₃⁻, HCO₃⁻) — same turnstile, but for red wristbands

Between each pair of diode films, ions get pulled out of the "dilute" channel (your clean water) and trapped in the "concentrate" channel (waste brine). The films act as one-way gates — ions can enter the concentrate channel but can't get back out.

```
          CATHODE (-)                              ANODE (+)
            │                                        │
            │  ← Na⁺  ← Ca²⁺  ← Fe²⁺              │
            │         │           │           │      │
  ┌─────────┼─────────┼───────────┼───────────┼──────┼─────────┐
  │  CONC   │  CEM    │  DILUTE   │   AEM     │ CONC │  CEM    │
  │ (waste) │(cation  │  (clean)  │ (anion    │(waste)│(cation  │
  │         │ diode)  │  water    │  diode)   │      │ diode)  │
  └─────────┼─────────┼───────────┼───────────┼──────┼─────────┘
            │         │           │           │      │
            │               Cl⁻ →   SO₄²⁻ →         │
            │                                        │

CEM = Cation Diode Film (SAC resin — same as battery)
AEM = Anion Diode Film (SBA resin — the floaters from brine separation)
```

### Key Advantages Over Reverse Osmosis

| | Electrodialysis | Reverse Osmosis |
|---|---|---|
| Membrane cost | $0.10 each (Rowow DIY) | $50-200 per cartridge |
| Membrane life | Years (self-cleaning) | 6-12 months |
| Pressure needed | None (gravity flow OK) | 40-80 PSI (pump required) |
| Power | 5-60W DC | 100-300W (pump) |
| Maintenance | Polarity reversal cleans scale | Filter replacement |
| Removes bacteria? | No (add UV stage) | Yes |
| Removes dissolved ions? | Yes | Yes |
| DIY difficulty | Moderate | Difficult (pressure vessel) |

### The Secret Weapon: EDR (Electrodialysis Reversal)

Scale buildup (calcium carbonate, iron deposits) is the enemy of all water treatment membranes. ED solves this with **polarity reversal:**

1. Run the cell normally for a set period (hours to days)
2. Reverse the polarity — swap positive and negative
3. The dilute and concentrate channels swap roles
4. Scale deposits that formed during forward operation **dissolve** during reversal
5. Swap back to normal operation

**The membranes self-clean.** No chemical cleaning, no filter replacement, no maintenance schedule. Just flip the polarity periodically.

---

## Diode Film Types — Using Both Resin Batches

Remember the brine float separation from the [membrane guide](../membrane/)? The sinkers (SAC/cation beads) go into cation diode films for the battery. The floaters (SBA/anion beads) are used HERE for anion diode films.

| Diode Film Type | Resin Used | What It Passes | What It Blocks | Color (typical) |
|-----------------|-----------|----------------|----------------|-----------------|
| Cation (CEM) | SAC (sinkers) | Positive ions (Na⁺, Ca²⁺, Fe²⁺) | Negative ions, electrons | Amber/dark |
| Anion (AEM) | SBA (floaters) | Negative ions (Cl⁻, SO₄²⁻) | Positive ions, electrons | Light/clear |

**Fabrication is identical** for both types — 50/50 resin powder + PVC cement, painted onto landscape fabric. The only difference is which resin you grind up. Same recipe, opposite selectivity — like making two diodes with reversed polarity.

### On Camera
- Show the two resin batches side by side — "the sinkers for batteries, the floaters for water purification"
- "Same recipe, different beads — one makes a positive-ion diode, the other makes a negative-ion diode"
- "Together they sort ions out of your drinking water like a coin sorter separates quarters from dimes"

---

## Materials

| Material | Source | Cost | Buy |
|----------|--------|------|-----|
| Mixed bed DI resin (for SBA floaters) | Amazon | Already have from battery project | [Amazon](https://www.amazon.com/dp/B07L4YX52J?tag=chipmonkeysof-20) |
| PVC cement (clear) | Home Depot | ~$6 | [Amazon](https://www.amazon.com/dp/B001D9WRWG?tag=chipmonkeysof-20) |
| Landscape fabric (non-woven PP) | Home Depot | ~$15 | [Amazon](https://www.amazon.com/dp/B0BQD91HH9?tag=chipmonkeysof-20) |
| Activated charcoal (granular) | Pet store / Amazon | ~$8/lb | [Amazon](https://www.amazon.com/dp/B01GN7ZQ70?tag=chipmonkeysof-20) |
| Graphite electrodes (2) | Amazon | ~$5-10 | [Amazon](https://www.amazon.com/s?k=graphite+electrode+rod&tag=chipmonkeysof-20) |
| HDPE or acrylic sheets (for stack frame) | Hardware store | ~$10-15 | — |
| Silicone gasket sheet or O-rings | Amazon | ~$5-10 | [Amazon](https://www.amazon.com/s?k=silicone+gasket+sheet&tag=chipmonkeysof-20) |
| 12V DC power supply (1-3A) | Amazon | ~$10 | [Amazon](https://www.amazon.com/s?k=12v+dc+power+supply+3a&tag=chipmonkeysof-20) |
| UV-C sterilization lamp | Amazon | ~$30-50 | [Amazon](https://www.amazon.com/s?k=uv-c+water+sterilizer&tag=chipmonkeysof-20) |
| TDS meter (total dissolved solids) | Amazon | ~$10-15 | [Amazon](https://www.amazon.com/s?k=tds+meter+water&tag=chipmonkeysof-20) |
| Vinyl tubing 1/4" ID | Hardware store | ~$5 | [Amazon](https://www.amazon.com/dp/B0B14GPGGL?tag=chipmonkeysof-20) |

*As an Amazon Associate I earn from qualifying purchases.*

---

## System Design

### Three-Stage Purification

```
STAGE 1: Electrodialysis (ED)          STAGE 2: Carbon         STAGE 3: UV
┌──────────────────────────┐    ┌──────────────────┐    ┌─────────────┐
│  Alternating CEM + AEM   │    │ Granular activated│    │  UV-C lamp  │
│  membranes with DC field │───→│ carbon column     │───→│  in quartz  │───→ CLEAN
│  Removes dissolved ions  │    │ Removes organics, │    │  tube       │     WATER
│  (metals, salts, minerals)│   │ chlorine, taste   │    │  Kills      │
│                          │    │                  │    │  bacteria   │
└──────────────────────────┘    └──────────────────┘    └─────────────┘
         5-60W DC                    Passive                5-10W
```

**Stage 1 — Electrodialysis:** Removes dissolved ions (hardness, iron, sodium, chloride, sulfate, nitrate). This is the heavy lifter.

**Stage 2 — Activated Carbon Filter:** Removes organic compounds, chlorine, taste, and odor. A simple PVC pipe filled with granular activated carbon. Passive — water flows through by gravity.

**Stage 3 — UV Sterilization:** Kills bacteria, viruses, and parasites. A $30-50 UV-C lamp in a quartz tube. Required for any surface water source (creek, pond). Optional for deep well water.

### Charcoal-Filled ED Channels — Dual Function

Here's the clever part: the spacer channels between membranes in the ED stack can be filled with **granular activated carbon**. This serves two purposes simultaneously:

1. **Ion conduction:** The charcoal provides conductivity between membranes, reducing electrical resistance
2. **Carbon filtration:** The water flowing through the charcoal channels gets filtered as it's being deionized

**And the electric field regenerates the carbon.** Ions that have adsorbed onto the charcoal get pulled off by the electric field and driven into the concentrate stream. The carbon filter self-regenerates during normal operation — it lasts 5-10x longer than a passive carbon filter.

### On Camera
- Show the three stages laid out
- "Electrodialysis for ions, carbon for organics, UV for bugs — $150 total"
- TDS meter reading before and after each stage

---

## Step 1: Make Both Membrane Types

### What you need
- Separated SAC (cation) resin — sinkers from brine float
- Separated SBA (anion) resin — floaters from brine float
- PVC cement, landscape fabric, grinder (same as battery membrane)

### Procedure

1. **Separate resin beads** using the brine float method (see [membrane/](../membrane/) Step 1). You need BOTH batches this time:
   - Sinkers (SAC) → Cation exchange membranes (CEM)
   - Floaters (SBA) → Anion exchange membranes (AEM)

2. **Grind each type separately.** Use the same spice grinder. Grind SAC to fine powder, store labeled "SAC POWDER — CEM." Grind SBA to fine powder, store labeled "SBA POWDER — AEM." Clean the grinder between types.

3. **Make CEM membranes:** 50/50 SAC powder + PVC cement, painted onto landscape fabric. Identical to the battery membrane process.

4. **Make AEM membranes:** 50/50 SBA powder + PVC cement, painted onto landscape fabric. Same process, different resin.

5. **Cure 24 hours** each. Label each membrane clearly — CEM vs AEM. They look similar once made.

### How many membranes?

| Application | Cell Pairs | CEMs needed | AEMs needed |
|-------------|-----------|-------------|-------------|
| Test (proof of concept) | 3 | 4 | 3 |
| Drinking water (0.5 L/min) | 10 | 11 | 10 |
| Inline 1 GPM | 20 | 21 | 20 |

A "cell pair" = one CEM + one AEM + one dilute channel + one concentrate channel.

### On Camera
- Show both resin types ground side by side
- Make one of each membrane type
- "Cation resin for cation membranes, anion resin for anion membranes — same recipe, different beads"

---

## Step 2: Build the Stack Frame

### What you need
- HDPE or acrylic sheet (for end plates and spacers)
- Silicone gasket material or O-rings
- Threaded rods and nuts (for compression)
- Graphite electrodes (one per end plate)

### Stack Assembly Order

For a 3-cell-pair test stack:

```
END PLATE (cathode + graphite electrode)
  Gasket
    CEM (cation membrane)
      Spacer + charcoal (CONCENTRATE channel)
    AEM (anion membrane)
      Spacer + charcoal (DILUTE channel — clean water)
    CEM
      Spacer + charcoal (CONCENTRATE channel)
    AEM
      Spacer + charcoal (DILUTE channel)
    CEM
      Spacer + charcoal (CONCENTRATE channel)
    AEM
      Spacer + charcoal (DILUTE channel)
    CEM
  Gasket
END PLATE (anode + graphite electrode)
```

### Spacer Design

Spacers create the flow channels between membranes. Options:

1. **Simple:** Cut frames from HDPE sheet with open centers. Fill centers with granular activated charcoal. Thickness: 3-5mm.

2. **3D Printed (ASA):** Print frames with internal flow distribution features. PVC cement bonds ASA to the membrane edges for a sealed channel.

3. **Corrugated PP sheet:** Cheap, creates turbulence. Cut to fit between membranes.

Each spacer has inlet and outlet holes for water manifolding.

### On Camera
- Show the stack being assembled layer by layer
- "CEM, spacer, AEM, spacer — that pattern repeats for as many cell pairs as you want"
- Show the charcoal being poured into spacer channels

---

## Step 3: Plumb and Connect

### Water Flow

Two independent water circuits:

1. **Dilute circuit (clean water):** Feed water → dilute channels (between AEM-CEM pairs) → clean water out
2. **Concentrate circuit (waste):** Fresh water or recirculated brine → concentrate channels → waste brine out

Manifold the channels with vinyl tubing and PVC pipe, same approach as the flow battery plumbing.

### Electrical

- **12V DC** across the stack (cathode at one end, anode at the other)
- Current: 1-3A for a 10-cell-pair stack (5-36W)
- Higher voltage = faster ion removal, but diminishing returns above ~2V per cell pair
- Can run directly from solar panel or flow battery — DC in, clean water out

### On Camera
- Show the plumbing connections
- Show the power supply hookup
- "12 volts DC — same power supply as the SEM cell"

---

## Step 4: Run and Test

### What you need
- TDS meter (total dissolved solids — ~$10-15 on Amazon)
- pH strips
- Source water (well water, tap water, or creek water for testing)

### Procedure

1. **Measure source water TDS.** This is your baseline. Typical well water: 200-800 ppm. Creek water: 50-300 ppm. Tap water: 100-400 ppm.

2. **Fill both circuits** with source water. No salt needed — you're removing ions, not adding them.

3. **Apply 12V DC.** Observe current draw on multimeter.

4. **Run for 10-30 minutes** for initial test.

5. **Measure output TDS** from the dilute (clean) stream.
   - Target: <50 ppm for drinking water (EPA secondary standard)
   - Excellent: <10 ppm (approaching DI water quality)
   - Under 500 ppm is safe per EPA primary standards

6. **Measure concentrate TDS** — should be rising as ions accumulate.

7. **Adjust:** More cell pairs = lower output TDS at the same flow rate. Higher voltage = faster removal. Slower flow = lower output TDS.

### Polarity Reversal (EDR Cleaning)

Every 4-24 hours of operation (or when you notice reduced performance):

1. Stop flow
2. Reverse the DC polarity (swap + and -)
3. Run for 15-30 minutes — scale deposits dissolve
4. Swap polarity back to normal
5. Resume normal operation

Automate this with a DPDT relay and a timer if running continuously.

### On Camera
- TDS meter readings before and after — "we started at 450 ppm, now we're at 35"
- Show the concentrate stream getting more mineral-rich
- "No filters to replace, no pressure pump, just electricity and membranes we made ourselves"

---

## Step 5: Add Carbon and UV Stages

### Carbon Filter Column

1. **Get a PVC pipe section** — 2-3" diameter, 12-18" long
2. **Fill with granular activated carbon**
3. **Cap both ends** with screen mesh to retain the carbon
4. **Plumb inline** after the ED output
5. Removes organic compounds, chlorine, and improves taste

The carbon in the ED stack channels already does significant filtration, but a dedicated column after the stack polishes the water further.

### UV Sterilization

1. **Buy a UV-C water sterilizer** — $30-50 on Amazon, designed for inline water purification
2. **Install after the carbon filter** — last stage before the tap
3. **Kills 99.9%** of bacteria, viruses, and parasites
4. **Required** for any surface water source (creek, pond, rainwater)
5. **Recommended** even for deep well water as a safety margin

### On Camera
- Show the full three-stage system assembled
- Run water through all three stages
- Final TDS reading + "and the UV kills anything the other two missed"

---

## System Sizes

| Application | Flow Rate | Cell Pairs | Power | Approx. Cost |
|-------------|-----------|------------|-------|-------------|
| Test (proof of concept) | 0.2 L/min | 3 | 5-10W | ~$50 |
| Drinking water (family) | 0.5 L/min | 10 | 5-15W | ~$100-150 |
| Inline 1 GPM | 3.8 L/min | 20 | 30-60W | ~$200-300 |
| Batch DI for truck washing | 1-2 L/min | 10 | 10-30W | ~$100-150 |

---

## Integration with Flow Battery and Homestead

### Power Source
The ED system runs on 12V DC — perfect for direct connection to the flow battery or a solar panel. No inverter needed. 5-15W for a family drinking water system is trivial compared to the battery's output.

### Concentrate Stream Uses
The waste brine from the concentrate channels isn't waste at all:
- **High mineral content** → garden irrigation (plants love the minerals)
- **High iron content** (from iron-rich well water) → additional battery electrolyte feedstock
- **High salt content** → SEM cell feedstock for acid/lye production

### The Closed Loop
```
Well Water → ED System → Clean Drinking Water
                ↓
           Concentrate
                ↓
    ┌──────────┴──────────┐
    │                     │
 Garden              If high iron:
 Irrigation          Iron for electrolyte
                          ↓
                     Flow Battery
                          ↓
                     Powers ED System
```

---

## Troubleshooting

| Problem | Likely Cause | Fix |
|---------|-------------|-----|
| TDS not dropping | Low current, insufficient cell pairs | Increase voltage, add more cell pairs, slow flow rate |
| Current very low | Membrane not conducting, dry channel | Ensure membranes were soaked, check for air bubbles |
| Membranes leaking between frames | Poor gasket seal | Replace gaskets, increase compression |
| Scale buildup on membranes | Hard water deposits (CaCO₃) | Run polarity reversal cycle (EDR) |
| Water tastes off | Organic contamination passing through | Add/replace activated carbon filter |
| Brown water output | Iron precipitating | Check membrane order (CEM/AEM may be swapped) |
| High power draw | Short circuit in stack | Check for membrane tears, ensure no metal touching both electrodes |

---

## Safety

- **Electrical:** 12V DC is low voltage and safe, but keep connections dry. The electrodes produce small amounts of gas (hydrogen at cathode, chlorine/oxygen at anode in an ED stack) — ensure ventilation.
- **Water quality:** Always test output water with TDS meter before drinking. Add UV sterilization for any surface water source.
- **Concentrate stream:** Contains concentrated minerals — don't pour onto sensitive plants or into fish habitat. Dilute for garden use.
- **Membrane handling:** PVC cement fumes during fabrication — work in ventilated area. Finished membranes are inert and safe to handle.
