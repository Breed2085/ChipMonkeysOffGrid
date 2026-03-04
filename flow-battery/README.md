# All-Iron Flow Battery

## How It Works

Two identical 3D-printed ASA boxes sandwich a flat membrane. Electrolyte (ferrous chloride in HCl) flows through both sides. On charge, iron plates on the negative side and Fe²⁺ oxidizes to Fe³⁺ on the positive. On discharge, it reverses. ~1.2V per cell.

## Cell Specs

| Parameter | 50mm Test Cell | 300mm Production |
|-----------|---------------|-----------------|
| Active area | 25 cm² | 900 cm² |
| Power per cell | ~1.25W @ 50mA/cm² | ~49-79W |
| Print time | ~10 min | ~45-60 min |
| Materials cost | ~$0.72 | ~$5-8 |

## Architecture

```
[ASA Box — popcorn-coated walls + charcoal fill]
  [Screen — soot-blackened, embedded in popcorn layer]
    [Popcorn Ball Electrode — PVC/starch/Elmer's/resin, torched]
      [Membrane — landscape fabric + 50/50 SAC resin/PVC cement]
    [Popcorn Ball Electrode]
  [Screen]
[ASA Box — popcorn-coated walls + charcoal fill]
```

## Files

- `designs/` — Fusion 360 source files
- `stl/` — Ready-to-print STL files
- `bom/` — Bill of materials with links and costs
- `docs/` — Build instructions

## Print Settings (ASA)

- Nozzle: 240-260°C
- Bed: 100-110°C
- Enclosure: Required
- Layer height: 0.2mm
- Nozzle: 0.4mm
- Printer: VzBot 400 (400mm bed) or any enclosed printer

**Why ASA:** PVC cement chemically welds to ASA. It does NOT bond to PLA. Every joint in this system relies on PVC cement fusion.
