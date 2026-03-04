# Ion Exchange Membrane — Rowow Method

Based on the open-source work of [Rowow](https://youtube.com/@Rowow) ([GitHub](https://github.com/Rowow1/Open-sourced-off-the-shelf-ion-exchange-membrane)).

## Materials

| Material | Source | Cost |
|----------|--------|------|
| Mixed bed DI resin (5 lbs) | Amazon | ~$25 |
| PVC cement (clear, 16oz) | Home Depot | ~$6 |
| Landscape fabric (non-woven) | Home Depot | ~$15/roll |
| Dedicated spice grinder | Amazon | ~$15 |

## Resin Separation — Brine Float

One bag of mixed bed resin gives you both cation AND anion beads:

1. Make saturated brine (~1.2 g/mL — keep adding salt until it stops dissolving)
2. Pour mixed bed resin in, stir vigorously, let settle 5-10 minutes
3. **Cation beads (SAC) SINK** (1.25-1.30 g/mL) — use for battery + SEM membranes
4. **Anion beads (SBA) FLOAT** (1.04-1.08 g/mL) — save for ED water purification membranes
5. Skim floaters, rinse, repeat for 98%+ separation
6. Grind cation beads in dedicated spice grinder to fine powder

## Membrane Recipe

**50% ground SAC resin + 50% PVC cement by volume**

NO graphite. NO carbon. The membrane must be electronically INSULATING — it blocks electrons and passes ions. Any carbon in the membrane risks short circuit.

## Fabrication

1. Spread pure membrane slurry onto flat surface
2. Press landscape fabric in (15-20mm overhang on all sides)
3. Spread more slurry on top of fabric
4. Clamp lightly, cure 24 hours

The landscape fabric does four jobs:
- Membrane reinforcement
- Thickness control
- Gasket seal (overhang bonds between box halves)
- Terminal insulation (prevents screws from shorting to opposite electrode)

## Integration with Popcorn Ball Electrode

After the membrane is fully cured, apply the popcorn ball electrode mix directly onto both faces. See [electrode/](../electrode/) for the recipe and process.
