# Storyboard visual QA

## Result

**PASS after targeted corrections.** All nine accepted panels were inspected at their original 941×1672 resolution. The deterministic 3×3 sheet and 1200-pixel-wide JPEG preview were also visually inspected. No panel is cropped or stretched in the sheet; label bands are outside the generated frames.

## Frame audit

| Frame | Status | Visual and continuity checks |
|---|---|---|
| 01 | PASS after FIX | Strict side repair; one wrench with clear contact; hatch closed; full drill/rear/engineer contained; three near-side road wheels plus distinct front roller. |
| 02 | PASS | Close final wrench turn; two coherent hands; wrench jaw seated on coupling; character identity and closed-hatch continuity hold. |
| 03 | PASS | Turn/reaction reads; one wrench; one distant golem; one red and one blue cluster; hatch closed; full rover contained. |
| 04 | PASS after FIX | Latch reach is clear, wrench at belt, hatch closed; full silhouette; three near-side road wheels restored; one drill/saw/golem. |
| 05 | PASS after FIX | One boot on step, other grounded; two credible contacts; one open rear-hinged hatch; wrench belted; one seat/two levers; full silhouette. |
| 06 | PASS after FIX | Single unduplicated climbing body; sound hand/knee/foot contacts; open hatch; belted wrench; full drill; three near-side wheels plus distinct roller. |
| 07 | PASS | One seated engineer in one seat; clean OTS; exactly two levers; centered drill; one golem and paired crystal clusters. |
| 08 | PASS | True driver-eye position; seat invisible; exactly one right forearm/hand presses one large red start button; exactly two levers; centered drill and one golem. |
| 09 | PASS after FIX | Driver remains visibly seated; exactly six visible wheels in two rows of three; one drill, one side saw, one beacon, open hatch; one golem and one red/blue cluster pair; dust launch reads. |

## Hard-reject audit

- No character duplicates or extra whole bodies in accepted frames.
- No floating wrench; it is held with contact in 01–03 and secured at the belt in 04–06.
- Hand anatomy/contact is readable in the close action frames. Frame 08 contains only one visible hand/arm, as required.
- Hatch progression is coherent: closed 01–04; open 05–09.
- Harvester remains a low worn bronze rover with one central navy drill, one side saw and one red rear beacon. No tracks, windshield, roof, tall cab, cyan rear module, or pseudo-text.
- Golem appears first at 03 and remains a single threat thereafter; the red/blue crystal pair remains singular.
- No in-frame text, numbers, HUD, UI or watermark.

## Honest residual drift notes

- Because the chassis is intentionally low-profile, the requested roughly 2× character scale reads mostly through vehicle length and footprint rather than literal height in wide frames.
- Frame 07 is an interior OTS, so the open hatch state is implied by the open-air cockpit and adjacent sequence rather than fully silhouetted.
- Frame 08 includes two tiny red indicator lamps near the console; they read as indicator lights, not additional push buttons. The single large red control under the fingertip is unambiguous.
- The blue front roller/drill support hardware changes visibility with angle, but it remains visually distinct from the six true rubber road wheels.

## Generation and assembly

- Built-in GPT Image 2 calls: **18 total**.
- Base calls: 9 (one per distinct storyboard frame).
- Targeted correction calls: 9 (01×1, 04×3, 05×1, 06×1, 09×3).
- Every accepted panel: **941×1672 PNG**.
- `storyboard-3x3.png`: **2955×5440 PNG**.
- `storyboard-3x3-chat.jpg`: **1200×2209 JPEG**.
- Assembly: deterministic System.Drawing compositing via `_assemble-storyboard.ps1`; no generative text or crop used for the sheet.
