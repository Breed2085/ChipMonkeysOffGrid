# Ion Exchange Membrane — Rowow Method

**A complete step-by-step guide to making ion exchange membranes from hardware store materials.**

Based on the open-source work of [Rowow](https://youtube.com/@Rowow) ([GitHub](https://github.com/Rowow1/Open-sourced-off-the-shelf-ion-exchange-membrane) | [Website](https://rowow.net)).

This guide is written to be followed on camera for YouTube Episode 4.

---

## What You're Making

An ion exchange membrane — we call these **diode films**. Just like a diode in electronics only lets current flow one direction, a diode film only lets specific ions pass through while blocking everything else. It's a one-way valve at the molecular level.

In the battery, the diode film passes ions (H⁺, Fe²⁺) but blocks electrons. This is the wall between the two half-cells. Without it, the cell short-circuits. With it, electrons are forced through the external circuit — that's your usable electricity.

Commercial ion exchange membranes (Nafion) cost $500-1,000 per square meter. This one costs about **$0.10 per cell** from materials you can buy at a pet store and Home Depot.

---

## Diode Films — Cation vs Anion

There are two types of diode films, and we make both from the same bag of mixed bed resin beads.

### Cation Diode Film (CEM — Cation Exchange Membrane)

Made from **SAC (Strong Acid Cation) resin** — the beads that **sink** in brine.

**What it does:** Only lets **positive ions** through. Hydrogen ions (H⁺), iron ions (Fe²⁺, Fe³⁺), sodium (Na⁺), calcium (Ca²⁺) — anything with a positive charge can pass. Negative ions and electrons are blocked.

**How it works:** The resin has sulfonic acid groups (-SO₃H) bonded to the polymer. These groups carry a permanent negative charge. That fixed negative charge attracts positive ions and repels negative ones — like a bouncer at a club that only lets certain people through the door.

**Real-world analogy:** Think of a screen door that only lets warm air out but blocks cold air from coming in. The mesh is the physical barrier, but it's selective — some things pass, others don't. The cation diode film is selective at the ionic level — positive charges pass, negative charges bounce off.

**Used in:** Flow battery cells, SEM cells

### Anion Diode Film (AEM — Anion Exchange Membrane)

Made from **SBA (Strong Base Anion) resin** — the beads that **float** in brine.

**What it does:** Only lets **negative ions** through. Chloride (Cl⁻), sulfate (SO₄²⁻), nitrate (NO₃⁻) — anything with a negative charge can pass. Positive ions and electrons are blocked.

**How it works:** The resin has quaternary ammonium groups (-NR₃⁺) bonded to the polymer. These carry a permanent positive charge. That fixed positive charge attracts negative ions and repels positive ones — the opposite bouncer.

**Real-world analogy:** Same screen door concept, but it only lets bugs out and blocks the warm air. Selective in the opposite direction.

**Used in:** Electrodialysis water purification (alternating with cation films)

### The Diode Analogy

In electronics, a diode lets current flow in one direction but blocks it in the other. Our diode films do the same thing for ions:

```
ELECTRONIC DIODE:    Current → [DIODE] → passes
                     Current ← [DIODE] ← BLOCKED

CATION DIODE FILM:   (+) ions → [CEM] → passes
                     (-) ions → [CEM] → BLOCKED

ANION DIODE FILM:    (-) ions → [AEM] → passes
                     (+) ions → [AEM] → BLOCKED
```

Both types block electrons completely. That's critical — if electrons could pass through the membrane, the battery would short-circuit internally.

### Why "Diode Film"?

The industry calls these "ion exchange membranes" or "ion selective membranes." We call them diode films because that's what they are — and because it makes the concept instantly click for anyone who's ever seen a diode. You don't need a chemistry degree to understand "it lets one thing through and blocks the other."

---

## Materials

| Material | Source | Cost | Buy |
|----------|--------|------|-----|
| Mixed bed DI resin, 5 lb | Amazon | ~$25 | [Amazon](https://www.amazon.com/dp/B07L4YX52J?tag=chipmonkeysof-20) |
| PVC cement, clear, 16 oz | Home Depot | ~$6 | [Amazon](https://www.amazon.com/dp/B001D9WRWG?tag=chipmonkeysof-20) |
| Landscape fabric, non-woven PP | Home Depot | ~$15/roll | [Amazon](https://www.amazon.com/dp/B0BQD91HH9?tag=chipmonkeysof-20) |
| Dedicated spice grinder | Amazon | ~$15 | [Amazon](https://www.amazon.com/dp/B07SYTRPSG?tag=chipmonkeysof-20) |
| Table salt, 1 lb | Grocery | ~$1 | — |
| Large bowl or bucket | — | — | — |
| Flat surface + clamps | — | — | — |

*As an Amazon Associate I earn from qualifying purchases.*

---

## Step 1: Separate the Resin Beads (Brine Float Method)

Mixed bed DI resin contains two types of beads mixed together. We need to separate them.

### What you need
- Mixed bed DI resin (any amount — start with 1-2 cups for testing)
- Table salt
- Warm water
- Large bowl or bucket
- Slotted spoon or fine strainer

### Procedure

1. **Make saturated brine.** Fill a container with warm water. Add table salt and stir until it stops dissolving — you'll see undissolved crystals on the bottom. That's saturated, roughly 1.2 g/mL density.

2. **Add resin beads.** Pour a batch of mixed bed resin into the brine. Stir vigorously for 30 seconds, then stop and wait 5-10 minutes.

3. **Watch them separate.**
   - **Cation beads (SAC) SINK** — density 1.25-1.30 g/mL. These are heavier than the brine. These make cation diode films for the battery and SEM cells.
   - **Anion beads (SBA) FLOAT** — density 1.04-1.08 g/mL. These are lighter than the brine. These make anion diode films for electrodialysis (ED) water purification.

4. **Skim the floaters.** Use the slotted spoon to scoop the floating anion beads off the top. Put them in a separate container labeled "ANION — for ED diode films."

5. **Collect the sinkers.** Drain off the brine and collect the cation beads that sank to the bottom. These are your membrane material.

6. **Rinse both batches** with clean water to remove salt residue.

7. **Repeat** if separation wasn't clean — do another float cycle on each batch. 2-3 cycles gets you to 98%+ purity.

### On camera
- Show the beads going in (they're usually different colors — makes great footage)
- Close-up of the separation happening in real time
- Show the sinkers vs floaters side by side

---

## Step 2: Grind the Cation Beads

### What you need
- Separated cation (SAC) beads, dry
- Dedicated electric spice grinder (NEVER use for food again — resin dust)
- Eye protection (fine dust)

### Procedure

1. **Dry the beads.** Spread them on a paper towel or baking sheet. Let air dry or use a fan. They need to be dry or they'll gum up the grinder.

2. **Grind in small batches.** Fill the grinder about 1/3 full. Pulse 10-15 seconds, check consistency, repeat until you have fine powder.

3. **Target consistency:** Fine enough that it feels smooth between your fingers, like powdered sugar. The finer the grind, the better the ionic conductivity — more surface area from the sulfonic acid groups.

4. **Store the powder** in a sealed container. Label it "GROUND SAC RESIN."

### On camera
- Show the whole beads, then the ground powder side by side
- Rub some between fingers to show texture
- "This spice grinder is now retired from kitchen duty permanently"

---

## Step 3: Mix the Membrane Slurry

### What you need
- Ground SAC resin powder
- PVC cement (clear)
- Mixing container (disposable cup works)
- Stir stick

### Recipe

**50% ground SAC resin + 50% PVC cement by volume**

That's it. Equal parts by volume. Mix thoroughly.

### Critical rules
- **NO graphite.** NO carbon black. NO activated charcoal. NOTHING electronically conductive.
- The membrane must be an **electronic insulator**. It passes ions only. Any carbon creates a short circuit path and your battery is dead.
- The PVC cement provides the structural matrix. The resin particles provide the ion-conducting pathways through that matrix.

### Procedure

1. **Measure** equal volumes of ground resin and PVC cement.
2. **Combine** in a mixing container.
3. **Stir thoroughly** — 2-3 minutes until uniform. No dry clumps, no clear spots.
4. **Work quickly** — PVC cement starts setting as the solvent evaporates. You have maybe 10-15 minutes of working time.

### On camera
- Show the two materials measured out
- "Fifty-fifty by volume. That's the whole recipe."
- Show the mixing process — emphasize that it needs to be uniform

---

## Step 4: Cast the Membrane

### What you need
- Membrane slurry (from Step 3)
- Landscape fabric (non-woven polypropylene or polyester) cut to size
- Flat surface (glass, tile, or smooth table)
- Clamps or weights

### Sizing the fabric
- Cut the landscape fabric **15-20mm larger** than your active cell area on all sides
- For a 50mm cell: cut fabric to ~80-90mm square
- The overhang becomes the gasket seal when assembled between box halves

### Procedure

1. **Spread a layer of slurry** on your flat surface, slightly larger than the fabric piece. About 0.5-1mm thick.

2. **Press the landscape fabric** into the wet slurry. Push it down so the slurry wicks up through the fabric. The fabric should be fully saturated — no dry white spots visible.

3. **Spread more slurry on top** of the fabric. Cover completely. Total membrane thickness should be about 1-2mm including the fabric.

4. **Clamp or weight lightly.** Don't squeeze — you want even thickness, not squished-out slurry. A flat board with a book on top works.

5. **Cure 24 hours.** Don't touch it. The MEK/THF solvents need to fully evaporate. Do this outdoors or in a very well-ventilated area — the fumes are real.

6. **Check the result.** The membrane should be firm, slightly flexible, and uniform. No holes, no thin spots, no dry patches.

### Why landscape fabric?

The landscape fabric does **four jobs** simultaneously:
1. **Reinforcement** — gives the membrane mechanical strength
2. **Thickness control** — sets a consistent membrane thickness
3. **Gasket seal** — the overhang bonds between box halves with PVC cement, sealing the cell
4. **Terminal insulation** — prevents terminal screws from shorting to the opposite electrode's mesh

One material. Four functions. $0.02 per cell.

### On camera
- Show the fabric being cut oversized — explain the overhang purpose
- Show the slurry being spread and the fabric pressed in
- Close-up of the slurry wicking through the fabric
- Time lapse of the 24-hour cure

---

## Step 5: Apply the Popcorn Ball Electrode

After the membrane is fully cured (24+ hours), apply the popcorn ball electrode directly onto both faces.

**See [electrode/](../electrode/) for the complete recipe and torch process.**

Summary:
1. Mix Bowl A (Elmer's + cornstarch) into Bowl B (PVC cement + ground SAC resin)
2. Paint onto both membrane faces, ~1-2mm thick
3. Press soot-blackened stainless screen into each side
4. Dry completely (12-24 hours)
5. Torch from the screen side — cornstarch puffs into carbon foam

The PVC cement in the electrode mix chemically welds to the PVC cement in the membrane. The result is a complete MEA: membrane + two electrodes + two screens, all chemically bonded into one unit.

---

## How It Works — The Science

### Why It's a Diode

Think about what a diode really does. An electronic diode has a P-N junction — the P side has fixed negative charges (acceptor atoms), and the N side has fixed positive charges (donor atoms). Mobile charges can only cross in one direction because the fixed charges create a one-way gate.

A cation diode film works the same way. The sulfonic acid groups (-SO₃H) on the SAC resin are **fixed negative charges** permanently bonded to the polymer. They can't move. When the film swells in water, those fixed negative charges:
- **Attract and pass** positive ions (H⁺, Fe²⁺) — they hop from one sulfonic acid group to the next through the membrane
- **Repel and block** negative ions (Cl⁻, SO₄²⁻) — the fixed negative charges push them away

This is called **Donnan exclusion** — the same principle that makes an electronic diode work, applied to ions instead of electrons.

An anion diode film is the reverse. The quaternary ammonium groups (-NR₃⁺) are fixed positive charges that attract negative ions and repel positive ones. Same diode principle, opposite polarity.

### Ion Exchange Resin

SAC (Strong Acid Cation) resin beads are polystyrene beads with **sulfonic acid groups** (-SO₃H) bonded to the polymer surface. In water deionization (like in aquarium filters), these groups grab cations (positive ions) out of the water and replace them with H⁺ — that's the "ion exchange" part. In our diode film, we're using these same groups as a selective gate rather than an exchanger.

When you grind the beads into powder and bind them with PVC cement, the sulfonic acid groups are still active. When the diode film swells in water or acid electrolyte, the sulfonic acid groups create **ion-conducting pathways** through the PVC matrix. H⁺ and Fe²⁺ ions hop from one sulfonic acid group to the next, passing through the film.

### Real-World Example: Aquarium Filters

If you've ever used a DI (deionized) water filter for an aquarium or a car wash spotless rinse system, you've already used this exact resin. Those filters are packed with the same mixed bed resin beads we're buying. The beads pull dissolved minerals out of tap water — calcium, magnesium, iron, chloride — leaving pure water behind.

We're taking those same beads, separating the two types, grinding them up, and painting them into films. Instead of pulling ions out of water passing through a tube of loose beads, our diode films selectively pass or block ions across a flat barrier. Same chemistry, different geometry, completely different application.

### Why It Works Even With 50% PVC Binder

Rowow proved that even with thick fiberglass mat and a 50/50 resin/PVC ratio, the diode film conducts ions well enough to work. This tells us the SAC resin is **extremely conductive** when swollen — even with half the volume being insulating PVC binder, there are enough resin particles touching each other to form continuous ion pathways through the film.

The diode film is NOT the performance bottleneck in this system. The electrode surface area is. That's why we put our innovation effort into the electrode (popcorn balls) and keep the diode film recipe simple and proven.

---

## Batch Production

For making many membranes at once:
1. Mix a large batch of slurry
2. Lay out a long strip of landscape fabric
3. Squeegee slurry along the entire strip
4. Cure the whole sheet
5. Cut individual membranes to size with scissors or tin snips
6. Each one gets the popcorn ball electrode applied individually

This is how you'd produce membranes for kit sales — batch the casting, individualize the electrode application.

---

## Troubleshooting

| Problem | Likely cause | Fix |
|---------|-------------|-----|
| Membrane is brittle | Too much resin, not enough PVC | Remix at 50/50 ratio |
| Membrane has holes | Air bubbles during casting | Press fabric in more firmly, work out bubbles |
| Membrane is too thin | Not enough slurry | Apply thicker layers on both sides of fabric |
| Cell has internal short | Carbon contamination in membrane | Remake — keep carbon materials AWAY from membrane mixing |
| Low ionic conductivity | Resin not ground fine enough | Grind longer, finer powder |
| Slurry sets too fast | PVC cement evaporating | Work faster, or add a tiny amount of MEK/acetone to extend working time |
