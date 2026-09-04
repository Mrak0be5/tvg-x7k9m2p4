# Storyboard v7 — match-cut QA

## Binding references

- Storyboard edit target: `mars-harvester-storyboard-3x3-direct-v6-final.png`
- Exact gameplay frame 0: `gameplay-first-frame-exact.png`, 720×1280, 30 fps source
- Accepted output: `mars-harvester-storyboard-3x3-direct-v7-matchcut-gptimage2.png`

## Panel audit

| Panel | Status | Audit |
|---|---|---|
| 01 | PASS | One engineer, one large six-wheel harvester, closed hatch, repair action readable. |
| 02 | PASS | One engineer and one wrench; hand/tool/pipe contact readable. |
| 03 | PASS | One engineer, one harvester, one blue golem, red and blue crystals; screen geography readable. |
| 04 | PASS | Engineer reaches the hatch area; no duplicated character or golem. |
| 05 | PASS | One rear-hinged hatch open; engineer climbs using the vehicle body. |
| 06 | PASS | Engineer enters the same cockpit; no duplicate engineer outside. |
| 07 | PASS | Stable OTS cockpit view, one engineer, two control levers, golem ahead. |
| 08 | PASS | Driver-eye POV, one gloved hand presses one red start button, two levers and centered drill. |
| 09 | PASS | Replaced with the opening gameplay composition: true high top-down camera, harvester below center moving toward upper-left, dust trailing lower-right, one blue golem and red/blue crystals upper-left. No visible open hatch or side door. |

## Boundary continuity

- Panel 08 → 09 intentionally changes from cockpit POV to the exact gameplay camera used at the start of the attached MP4.
- Vehicle direction and target geography match the real opening frame.
- The gameplay HUD first appears in panel 09 because this panel represents the splice point into the original video.
- The simpler vehicle rendering in panel 09 is intentional: it inherits the real game visual rather than the cinematic preroll model.

## Remaining ambiguity

- Small HUD numbers are reference-level details and are not the continuity priority.
- Panel 09 is stylistically less cinematic by design; camera, direction, placement and absence of the raised hatch are the binding match-cut features.
