# Electrolyte — Ferrous Chloride (FeCl₂)

**A complete step-by-step guide to making all-iron flow battery electrolyte from scrap metal and hardware store acid.**

This guide is written to be followed on camera for YouTube Episode 3.

---

## What You're Making

A solution of ferrous chloride (FeCl₂) dissolved in dilute hydrochloric acid. This is the electrolyte for both half-cells of the all-iron flow battery. The same liquid goes in both tanks — the chemistry handles the rest.

- **Color:** Pale green (Fe²⁺ ions in solution)
- **pH:** 1-2 (strongly acidic)
- **Concentration:** ~1M FeCl₂
- **Cost:** ~$2/gallon from store-bought acid, or ~$0.15/gallon if you make your own acid via SEM cell

---

## Method 1: Muriatic Acid + Scrap Iron (Quick Start)

This is the fastest way to get electrolyte. Buy acid, dissolve iron, done.

### Materials

| Material | Source | Cost | Buy |
|----------|--------|------|-----|
| Muriatic acid, 1 gal (31% HCl) | Home Depot | ~$8 | [Amazon](https://www.amazon.com/dp/B01LYNZA7Z?tag=chipmonkeysof-20) |
| Scrap mild steel, ~2 lbs | Garage / scrap yard | Free | — |
| HDPE bucket or glass jar | Dollar store | ~$2 | — |
| Chemical-resistant nitrile gloves | Amazon | ~$10 | [Amazon](https://www.amazon.com/dp/B01DPEGZB0?tag=chipmonkeysof-20) |
| Splash-proof safety goggles | Amazon | ~$8 | [Amazon](https://www.amazon.com/s?k=chemical+splash+safety+goggles&tag=chipmonkeysof-20) |
| Baking soda (for spills) | Grocery | ~$2 | [Amazon](https://www.amazon.com/s?k=baking+soda&tag=chipmonkeysof-20) |
| Fine strainer or cheesecloth | Kitchen | ~$1 | — |

*As an Amazon Associate I earn from qualifying purchases.*

### Iron Source Rules

This is critical. The wrong metal will poison your membrane and ruin your cells.

| USE (magnet sticks) | AVOID |
|---------------------|-------|
| Nails, bolts, screws | **Stainless steel** — chromium is carcinogenic, poisons membrane |
| Rebar, angle iron | **Galvanized** — zinc contamination, blocks ion exchange |
| Wire, tie wire, baling wire | **Tool steel** — tungsten, vanadium, cobalt contamination |
| Brake rotors, bed frames | **Plated metals** — nickel, chrome plating dissolves into solution |
| Cast iron, engine blocks | **Aluminum** — wrong chemistry entirely |

**The magnet test:** If a magnet sticks firmly, it's mild steel or cast iron — good. If it doesn't stick or barely sticks, it's stainless, aluminum, or non-ferrous — bad.

### Procedure

1. **Set up outdoors.** This reaction produces hydrogen gas. No enclosed spaces. No flames. No sparks. No smoking nearby. Hydrogen is invisible and explosive.

2. **Gear up.** Nitrile gloves and splash-proof goggles. Have baking soda within arm's reach for spill neutralization.

3. **Pour muriatic acid into your container.** Use HDPE (the plastic Home Depot buckets are made of), polypropylene, or glass. **NOT metal. NOT thin plastic bags. NOT aluminum.** The acid will eat through most metals.

4. **Add scrap iron pieces.** Drop them in gently — don't splash. The reaction starts immediately.

5. **Watch for fizzing.** The bubbles are hydrogen gas. The reaction is:
   ```
   Fe + 2HCl → FeCl₂ + H₂↑
   ```
   Iron dissolves. Hydrochloric acid gets consumed. Hydrogen gas escapes. The solution turns pale green as Fe²⁺ ions accumulate.

6. **Wait 12-24 hours.** Stir occasionally. Add more iron if fizzing stops but the acid is still clear (not green enough). You want excess iron — that ensures all the acid is consumed and the pH stabilizes.

7. **Check the color.** The solution should be pale green to medium green. If it's yellow-brown, Fe²⁺ has oxidized to Fe³⁺ from air exposure — that's fine for the positive tank, but try to minimize it by keeping a lid loosely on top.

8. **Strain out undissolved iron.** Pour through a fine strainer or cheesecloth into your storage container. The leftover iron goes back in the scrap pile for next time.

9. **Check pH.** Should be pH 1-2. If you have pH strips, use them. If you don't — the pale green color and the fact that excess iron was present means you're in the right range.

10. **Store in sealed HDPE containers.** Label clearly: "FeCl₂ ELECTROLYTE — ACID — pH 1-2." Keep out of sunlight to minimize oxidation.

### On Camera
- Show the magnet test on different scrap metals — "this one sticks, good. This one doesn't — stainless, we don't want this"
- Close-up of the iron going into the acid and the fizzing starting immediately
- Time lapse of the 24-hour dissolution — color change from clear to green
- Show the straining process and the final pale green solution
- pH strip test on camera

---

## Method 2: SEM Cell (Make Your Own Acid From Salt)

Instead of buying muriatic acid, you can make hydrochloric acid from table salt, water, and electricity using a Salt Electro Mining (SEM) cell. This uses the same Rowow membrane as the battery.

**See [sem-cell/](../sem-cell/) for the complete SEM cell build guide.**

### The Fast Method — Combined SEM + Iron Dissolution

Load scrap iron directly into the SEM anode chamber. As the cell produces HCl at the anode, the acid immediately dissolves the iron, producing FeCl₂ electrolyte in one step. The acid never accumulates — it's consumed as fast as it's made.

This is the self-sustaining approach:
1. Salt + water + electricity → HCl (anode) + NaOH (cathode)
2. HCl + scrap iron → FeCl₂ (battery electrolyte)
3. NaOH collected separately (valuable byproduct)

### Lye Byproduct — This Pays for Everything

The cathode side of the SEM cell produces sodium hydroxide (NaOH), also called lye or caustic soda. This is a genuinely valuable chemical.

| Product | Quantity (110-gal batch) | Retail Value |
|---------|------------------------|--------------|
| NaOH (lye) | ~84 lbs | **$170-330** |

**Uses for NaOH:**
- **Soap making** — the essential saponification agent (cold process soap)
- **Drain cleaner** — pure lye IS drain cleaner
- **Biodiesel** — catalyst for transesterification
- **Paint stripping** — dissolves old paint
- **Water treatment** — pH adjustment
- **Cleaning agent** — industrial degreaser base

The byproduct from making your battery electrolyte is worth more than the battery materials. The economics are backwards in the best way.

### Cost Comparison

| Method | Cost per gallon of 1M FeCl₂ |
|--------|------------------------------|
| Store-bought muriatic acid | ~$2.00 |
| SEM cell (salt + electricity) | ~$0.15 |
| SEM cell minus lye credit | **Effectively free** |

---

## Electrolyte Management

### Starting the Battery

Both tanks get the same electrolyte — ~1M FeCl₂ in dilute HCl. During charging, the chemistry diverges:

- **Positive tank:** Fe²⁺ oxidizes to Fe³⁺ (solution turns yellow-brown)
- **Negative tank:** Fe²⁺ reduces to Fe⁰ (iron plates out as metal on the electrode)

During discharge, both reactions reverse.

### Topping Off

Over time, water evaporates from the open tanks (if not sealed). Top off with distilled water or DI water to maintain concentration. Don't top off with tap water — the minerals and chlorine will contaminate the electrolyte.

### Rebalancing

If the positive side gets too much Fe³⁺ (turns dark brown/orange) and the negative side runs low on Fe²⁺:
- Add fresh FeCl₂ solution to the negative tank
- The self-healing property of all-iron chemistry means crossover doesn't cause permanent damage — ions that cross the membrane are still usable iron

### Color Guide

| Color | What it means |
|-------|--------------|
| Pale green | Fresh FeCl₂ — Fe²⁺ dominant (discharged state) |
| Medium green | Normal operating range |
| Yellow-green | Some Fe³⁺ forming (positive side during charge) |
| Yellow-brown | Mostly Fe³⁺ (positive side, charged state) |
| Dark brown/orange | Heavily charged positive side or oxidized electrolyte |
| Clear | Acid with no iron dissolved yet |

### On Camera
- Show the color progression — fresh green → charged yellow → discharged back to green
- "The color tells you the state of charge — nature's built-in battery meter"

---

## Scaling Up

### For the 50mm Demo Stack (4 cells)
- ~2 liters per tank (4 liters total)
- ~0.5 lb scrap iron
- ~1 quart muriatic acid
- Total electrolyte cost: ~$2

### For the 300mm Production Stack
- 5-gallon buckets per tank (40 liters total)
- ~10 lbs scrap iron
- ~2 gallons muriatic acid (or one SEM batch)
- Total electrolyte cost: ~$8 (acid method) or ~$1 (SEM method)

---

## Troubleshooting

| Problem | Likely Cause | Fix |
|---------|-------------|-----|
| Solution won't turn green | Iron isn't dissolving | Check that it's mild steel (magnet test), add more acid |
| Fizzing stops but solution is still clear | Not enough iron | Add more scrap iron |
| Solution is dark brown immediately | Oxidized / too much air exposure | Keep lid on loosely, reduce surface area exposure |
| White precipitate forming | Zinc contamination (galvanized metal) | Start over — discard solution, use only magnet-tested mild steel |
| Blue-green color | Copper contamination | Start over — copper poisons the system |
| Solution smells like rotten eggs | Sulfide contamination from cast iron impurities | Ventilate, strain, and it should be usable |

---

## Safety

**This involves concentrated acid and gas generation. Respect the chemistry.**

- **Acid burns:** Muriatic acid is 31% HCl. It will burn skin on contact. Wear nitrile gloves and splash-proof goggles at ALL times.
- **Hydrogen gas:** Released during iron dissolution. Invisible, odorless, explosive. Work outdoors. No flames, no sparks, no smoking within 10 feet.
- **Acid fumes:** HCl vapor irritates lungs and eyes. Work outdoors or in very well-ventilated area. If your eyes sting, move upwind.
- **Spill response:** Pour baking soda on acid spills — it neutralizes the acid with fizzing. Rinse with lots of water. Skin contact: rinse immediately under running water for 5+ minutes.
- **Storage:** Sealed HDPE containers, labeled, away from children and pets. Never store in metal containers.
- **Disposal:** Neutralize with baking soda until fizzing stops, then safe to pour on gravel/dirt. Or save it — it's battery electrolyte, don't waste it.
