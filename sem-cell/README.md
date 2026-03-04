# SEM Cell — Salt Electro Mining

**A complete step-by-step guide to making hydrochloric acid and sodium hydroxide from table salt, water, and electricity.**

Based on [Rowow's SEM TECH documentation](https://rowow.net).

This guide is written to be followed on camera for YouTube Episode 5.

---

## What You're Making

A simple electrochemical cell that splits salt water (brine) into two valuable chemicals:

- **Anode side:** Hydrochloric acid (HCl) — used to make battery electrolyte
- **Cathode side:** Sodium hydroxide (NaOH / lye) — valuable byproduct worth $170-330 per large batch

The same Rowow membrane used in the flow battery separates the two chambers. Same fabrication technique, same materials.

**Overall reaction:**
```
2NaCl + 2H₂O → 2NaOH + Cl₂ + H₂
                (cathode) (anode) (cathode)

Cl₂ + H₂O → HCl + HClO (anode side — chlorine dissolves into acid)
```

---

## Why Build a SEM Cell

| Reason | Details |
|--------|---------|
| **Free acid** | Make HCl from table salt (~$0.15/gallon vs $8/gallon store-bought) |
| **Valuable byproduct** | NaOH sells for $2-4/lb — 84 lbs from a 110-gallon batch = $170-330 |
| **Self-sufficiency** | No dependency on hardware store acid supply |
| **Closed-loop** | Salt → acid → electrolyte → battery → power → SEM cell → more acid |
| **Same membrane** | Uses the exact Rowow membrane you're already making for the battery |

---

## Materials

| Material | Source | Cost | Buy |
|----------|--------|------|-----|
| Two HDPE containers (2-5 gallon) | Dollar store / Home Depot | ~$4 | — |
| Graphite electrodes (2) | Amazon or carbon rods from D-cell batteries | ~$5-10 | [Amazon](https://www.amazon.com/s?k=graphite+electrode+rod&tag=chipmonkeysof-20) |
| Rowow cation membrane (1) | [See membrane/](../membrane/) | ~$2 | — |
| Table salt, 5-10 lbs | Grocery | ~$3-5 | — |
| 12V DC power supply (2-5A) | Amazon or old laptop charger | ~$10-15 | [Amazon](https://www.amazon.com/s?k=12v+dc+power+supply+5a&tag=chipmonkeysof-20) |
| PVC cement (clear) | Home Depot | ~$6 | [Amazon](https://www.amazon.com/dp/B001D9WRWG?tag=chipmonkeysof-20) |
| Vinyl tubing 1/4" ID | Hardware store | ~$5 | [Amazon](https://www.amazon.com/dp/B0B14GPGGL?tag=chipmonkeysof-20) |
| Alligator clip leads | Amazon | ~$5 | [Amazon](https://www.amazon.com/s?k=alligator+clip+leads&tag=chipmonkeysof-20) |
| Multimeter | Amazon | ~$15 | [Amazon](https://www.amazon.com/s?k=digital+multimeter&tag=chipmonkeysof-20) |
| Chemical-resistant nitrile gloves | Amazon | ~$10 | [Amazon](https://www.amazon.com/dp/B01DPEGZB0?tag=chipmonkeysof-20) |
| Splash-proof safety goggles | Amazon | ~$8 | [Amazon](https://www.amazon.com/s?k=chemical+splash+safety+goggles&tag=chipmonkeysof-20) |

*As an Amazon Associate I earn from qualifying purchases.*

---

## Step 1: Build the Cell Housing

### What you need
- Two HDPE containers (matching size — 2-gallon buckets work great for testing)
- Rowow cation membrane (already fabricated — see [membrane/](../membrane/))
- PVC cement
- Drill or hole saw

### Procedure

1. **Cut matching holes** in one side of each container. The holes should be large enough for electrolyte to contact the membrane — at least 3-4 inches across for a test cell.

2. **Sandwich the membrane** between the two containers at the holes. The landscape fabric overhang from the membrane gives you a sealing surface.

3. **Seal with PVC cement** around the entire perimeter of the membrane-to-container joint. Apply generously — this must be watertight. The PVC cement bonds to HDPE reasonably well when the surface is roughed up with sandpaper first.

4. **Let cure 24 hours.** Full solvent evaporation needed before filling with liquid.

5. **Leak test** by filling both sides with plain water. Check all seams. Fix any leaks with more PVC cement.

### Alternative: Single Container with Divider
- Use one larger container with the membrane mounted vertically as a divider wall
- Simpler construction, but harder to empty chambers independently
- Good for a first test, but two separate containers is better for production

### On Camera
- Show the container prep and hole cutting
- Show the membrane being sandwiched and sealed
- "This membrane is the same one we made in Episode 4 — same Rowow recipe, same materials"

---

## Step 2: Prepare the Electrodes

### What you need
- Graphite rods or plates (2)
- Wire or alligator clip leads

### Procedure

1. **Source graphite electrodes.** Options:
   - **Best:** Graphite rods from Amazon (~$5-10 for a set)
   - **Free:** Carbon rods extracted from D-cell alkaline batteries (remove the steel jacket, pull out the carbon rod) — works but smaller surface area
   - **Upgrade:** Graphite plates for maximum surface area

2. **Attach leads.** Wrap bare copper wire tightly around the top of each graphite rod (above the waterline). Or use alligator clips. The connection point MUST stay above the liquid level — copper dissolves in acid.

3. **Label the electrodes:**
   - **ANODE (+)** — goes in the acid/chlorine side
   - **CATHODE (-)** — goes in the lye side

### Why graphite and not metal?
- The anode side produces chlorine, which corrodes most metals
- Graphite is chemically inert to chlorine, acid, and lye
- Stainless steel works for the cathode but NOT the anode (chlorine eats it)
- Graphite for both sides keeps it simple

### On Camera
- Show extracting a carbon rod from a D-cell battery (great footage)
- Show the commercial graphite rod option side-by-side
- "Graphite survives everything we're going to throw at it"

---

## Step 3: Make Saturated Brine

### What you need
- Table salt (non-iodized preferred, but iodized works)
- Warm water
- Stirring stick

### Procedure

1. **Fill both chambers** with warm water (not hot — just warm enough to dissolve salt faster).

2. **Add salt to BOTH sides.** Stir until dissolved. Keep adding salt until it stops dissolving and you see undissolved crystals on the bottom. That's saturated — approximately 26% salt by weight, or about 360g per liter.

3. **Both sides start as identical brine.** As the cell runs, the anode side becomes acidic (HCl accumulates) and the cathode side becomes basic (NaOH accumulates).

### On Camera
- Show the salt going in and dissolving
- Show the point where it stops dissolving — "when you see crystals on the bottom, you're saturated"
- "Both sides start the same. The electricity does the sorting."

---

## Step 4: Run the Cell

### What you need
- Assembled SEM cell with brine
- Graphite electrodes in place
- 12V DC power supply
- Multimeter
- Alligator clip leads

### Procedure

1. **MOVE OUTDOORS.** This step produces chlorine gas at the anode. Do not run indoors under any circumstances.

2. **Connect power supply:**
   - **Positive (+)** terminal → **Anode** graphite rod (acid/chlorine side)
   - **Negative (-)** terminal → **Cathode** graphite rod (lye side)

3. **Turn on power.** You should see bubbles at both electrodes within seconds:
   - **Anode bubbles:** Chlorine gas (Cl₂) — yellow-green tint, "swimming pool" smell
   - **Cathode bubbles:** Hydrogen gas (H₂) — invisible, odorless, flammable

4. **Monitor current.** Use a multimeter in series or check the power supply readout.
   - Starting current: 1-3A at 12V (depends on electrode surface area and brine concentration)
   - Current will decrease as salt is consumed
   - If current is very low (<0.5A), check connections, electrode contact area, membrane seal

5. **Run for 4-24 hours** depending on desired concentration. Longer = more concentrated products.

6. **Monitor the anode side.** It becomes increasingly acidic. You can check with pH strips periodically. The brine starts at ~pH 7 and drops toward pH 1-2 as HCl accumulates.

7. **Monitor the cathode side.** It becomes increasingly basic. NaOH accumulates. The solution becomes slippery/soapy to touch (don't touch it without gloves — concentrated NaOH causes chemical burns).

8. **Shut off and collect products** when desired concentration is reached or salt is depleted.

### On Camera
- Show the power supply connection — "positive to anode, negative to cathode"
- Close-up of bubbles forming at both electrodes
- pH strip test at intervals showing the acid side dropping
- "If you smell swimming pool, that's chlorine — it means it's working, but stay upwind"
- Time lapse of the multi-hour run

---

## Step 5: Collect and Store Products

### Anode Side — Hydrochloric Acid (HCl)

1. **Drain the anode chamber** into an HDPE or glass container.
2. **Label:** "HCl — SEM PRODUCT — ACID"
3. **Use directly** to dissolve scrap iron for battery electrolyte (see [electrolyte/](../electrolyte/))
4. **Or use the Fast Method** (Step 6 below) to skip this step entirely

### Cathode Side — Sodium Hydroxide (NaOH)

1. **Drain the cathode chamber** into an HDPE container (glass works too).
2. **Label:** "NaOH — LYE — CAUSTIC — KEEP SEALED"
3. **Seal immediately** — NaOH absorbs CO₂ from air and degrades to sodium carbonate
4. **Store for use or sale** — see byproduct value section below

### On Camera
- Show the two products side by side — "acid on the left, lye on the right, from table salt"
- Show the acid being used to dissolve iron for electrolyte
- "The lye alone is worth more than everything we put into this"

---

## Step 6: The Fast Method — Combined Acid + Iron Dissolution

This is the production shortcut. Instead of collecting HCl and then dissolving iron in a separate step, you load scrap iron directly into the anode chamber.

### Procedure

1. **Load scrap iron** (magnet-tested mild steel) into the anode chamber before filling with brine.

2. **Fill with brine and run** as normal.

3. **As HCl forms at the anode, it immediately dissolves the iron:**
   ```
   Anode: Cl₂ → dissolved as HCl in brine
   Iron: Fe + 2HCl → FeCl₂ + H₂↑
   Net: Salt + water + electricity + iron → FeCl₂ (electrolyte) + NaOH (lye)
   ```

4. **The acid never accumulates** — it's consumed as fast as it's produced. This means less free HCl vapor and chlorine gas, making it somewhat safer (but still run outdoors).

5. **Result:** The anode chamber directly fills with FeCl₂ electrolyte. Drain it straight into your battery tanks.

### Advantages of the Fast Method
- One step instead of two
- Less chlorine gas exposure (iron consumes the acid continuously)
- Direct path: salt → electrolyte
- Iron acts as a chlorine scavenger, reducing gas emissions

### On Camera
- Show the iron loaded into the anode chamber
- "The acid makes itself, dissolves the iron, and we get battery electrolyte. One step."
- Show the green FeCl₂ solution forming in real time

---

## Byproduct Value — NaOH

This is the part that makes the economics ridiculous. The byproduct from making battery acid is worth more than the battery.

### Yield per batch

| Batch Size | Salt Input | NaOH Output | Retail Value |
|------------|-----------|-------------|--------------|
| 5 gallon (test) | ~5 lbs | ~4 lbs | $8-16 |
| 55 gallon (production) | ~50 lbs | ~42 lbs | $85-165 |
| 110 gallon (full scale) | ~100 lbs | ~84 lbs | **$170-330** |

### NaOH Uses and Markets

| Use | Form | Sell To |
|-----|------|---------|
| Soap making (cold process) | Flakes or solution | Etsy soap makers, local craft fairs |
| Drain cleaner | Concentrated solution | Direct consumer (bottle and label) |
| Biodiesel production | Flakes | Biodiesel co-ops, homesteaders |
| Paint stripping | Solution | Painters, furniture restorers |
| Water treatment | Solution | Pool supply, water treatment |
| Pretzels and bagels | Food grade (higher purity) | Bakeries (if purity verified) |

### On Camera
- Show the NaOH being bottled
- Calculate the value on screen — "84 pounds of lye at $2-4 per pound..."
- "The byproduct from making our battery electrolyte pays for the entire project"

---

## Scaling

### Test Cell (Episode 5)
- Two 2-gallon HDPE buckets
- 3-4" membrane between them
- Graphite rod electrodes
- 12V laptop charger (2-3A)
- Runtime: 4-8 hours for first batch
- Goal: Prove the process, measure yield, calculate efficiency

### Production Cell
- Two 55-gallon HDPE drums
- Large membrane panel (12"+ square)
- Multiple graphite plate electrodes in parallel
- 12V 20-30A power supply (or solar panel direct)
- Runtime: 24-48 hours per batch
- Continuous operation with brine top-up

### Solar-Powered SEM
The SEM cell runs directly from a solar panel or the flow battery. DC in, chemicals out. No inverter needed. This is the closed-loop vision:

```
Solar → Flow Battery → SEM Cell → HCl + NaOH
                ↑                    ↓
                └── FeCl₂ electrolyte ←── HCl + scrap iron
```

---

## Troubleshooting

| Problem | Likely Cause | Fix |
|---------|-------------|-----|
| No bubbles at electrodes | No current flowing | Check connections, power supply, electrode contact |
| Very low current (<0.5A) | Depleted brine or bad membrane seal | Add more salt, check membrane for leaks |
| Chlorine smell very strong | Normal, but work upwind | Move upwind, consider Fast Method (iron scavenger) |
| Membrane leaking | Poor seal at container joint | Drain, dry, reseal with PVC cement, cure 24 hours |
| Brown staining at anode | Iron contamination from leads | Use only graphite at anode, keep copper above waterline |
| Cathode electrode corroding | Using metal instead of graphite | Switch to graphite (steel cathode works but graphite is better) |
| Products not concentrated enough | Not enough run time | Run longer, or reduce water volume |

---

## Safety

**CRITICAL: This process produces CHLORINE GAS. Chlorine gas is toxic. OUTDOORS ONLY.**

- **Chlorine gas (anode):** Yellow-green, "swimming pool" smell. Toxic to lungs even in small concentrations. Work OUTDOORS with breeze. Position yourself UPWIND at all times. If you smell chlorine indoors, evacuate immediately.
- **Hydrogen gas (cathode):** Invisible, odorless, explosive. No flames near the cell. Adequate ventilation.
- **HCl (anode product):** Corrosive acid. Gloves and goggles. Baking soda for spills.
- **NaOH (cathode product):** Caustic base. Causes chemical burns. Gloves and goggles. Rinse skin contact with water for 15+ minutes. Vinegar for spill neutralization.
- **Electrical:** 12V DC is safe voltage, but keep connections dry. Don't touch electrodes while powered.
- **Storage:** Label everything clearly. Keep acids and bases in separate areas. Seal NaOH to prevent CO₂ absorption.
