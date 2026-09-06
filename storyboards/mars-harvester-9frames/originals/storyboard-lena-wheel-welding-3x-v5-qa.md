# STORYBOARD QA — v5 targeted edit

- Built-in GPT Image 2 edit calls: 1
- Source-retained result: `C:\Users\hebp\.codex\generated_images\01a06dd7-a80b-7aa3-9893-636914745e63\exec-5a00a787-85ba-4827-9e56-5e91789db154.png`
- Final copy: `C:\Users\hebp\OneDrive\Документы\Sorter\output\mars-harvester-storyboard-wheel-welding-3x-v5\mars-harvester-lena-wheel-welding-storyboard-v5.png`
- Validation: 1536 × 1024 PNG; 2,834,302 bytes; SHA-256 `FE870594453750755882057C6DC82F982E118F6327F674651E9A8CE2A06909BE`

## Targeted checks

| Panel | Verdict | Observation |
|---|---|---|
| 01 | PASS | Composition, welding action, text and giant wheel remain visually consistent with v4. |
| 02 | PASS | Composition, welding action, text and giant wheel remain visually consistent with v4. |
| 03 | PASS | Exactly one Lena is visible. She welds one wheel hub with a contact arc and sparks; duplicate head/body removed cleanly. |
| 04 | PASS | Exactly one small Lena at the same wheel. Inferred standing height is about one third of the harvester ground-to-roof height. Vehicle, golem and camera remain stable. |
| 05 | PASS | Exactly one small Lena at the same wheel. Inferred standing-height ratio is approximately 3:1. Vehicle, golem and camera remain stable. |
| 06 | PASS | Exactly one reduced Lena climbs through the same open hatch; vehicle-to-human ratio reads approximately 3:1 and contacts remain plausible. |
| 07 | PASS | Seated cockpit panel remains visually consistent, with one Lena and two levers. |
| 08 | PASS | FPS charge remains visually consistent, with two hands, two levers and centered drill. |
| 09 | PASS | Top-down direction preserved: centered drill aims directly toward the single golem; red/blue clusters and dust remain. |

## Board-level notes

- Exact 3×3 layout, requested header and nine caption labels remain readable.
- The edit is visually conservative, but a generative whole-image edit cannot guarantee literal pixel identity outside the requested cells; small texture-level redraw is possible.
- Three bronze road wheels are clearly visible on the near side in wide panels. The far side is occluded, so six total wheels cannot be literally counted from these side views; the dark forward roller/saw assembly remains distinct from the three bronze road wheels.
- No extra people are visible after correction.
- No additional generation or raster post-processing was performed.
