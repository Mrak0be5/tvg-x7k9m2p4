# Mars Harvester Seedance 2.0 Reference Card v2 — Prompts

Generator: built-in GPT Image 2 through the `imagegen` workflow only.

Built-in generation calls used in this completion stage: **4** — one base generation and one targeted camera-position correction for each of the two new POV panels. The seven supplied exterior/interior panels were reused without regeneration.

## Identity references

1. Primary vehicle identity sheet: `C:\Users\hebp\OneDrive\Документы\Sorter\output\mars-harvester-seedance20-reference-pack-v1\seedance20-harvester-reference-pack.png`
2. Cockpit layout anchor: `C:\Users\hebp\OneDrive\Документы\Sorter\output\mars-harvester-seedance20-reference-card-v2\cabin-01-interior-top-down.png`
3. The accepted corrected wide POV was also used as the camera/interior anchor for the final portrait correction.

## cabin-02-pov-wide.png — base generation

```text
Use case: stylized-concept
Asset type: 1536×1024-ish horizontal Seedance 2.0 vehicle continuity reference panel
Input images: Image 1 is the primary identity reference sheet for the exact Mars harvester; Image 2 is the exact cockpit/interior reference. Use them as strict visual identity anchors, not edit targets.
Primary request: Create a wide first-person driver-eye POV from inside this exact Mars harvester, as if an invisible seated driver is looking forward through the low open cockpit. The worn golden-bronze cockpit rim and compact dashboard frame the lower foreground. Include exactly two short bronze control levers with dark red-brown ball knobs, matching the reference. Directly ahead, the same single central dark navy conical drill is visible along the vehicle centerline from behind; only a small peripheral edge of the single side circular saw may appear if physically plausible from this viewpoint. No person, hands, arms, body, helmet, or character.
Scene/backdrop: neutral off-white studio cyclorama / empty matte floor visible ahead, no props, no landscape, no crystals, no golem.
Style/medium: same stylized high-detail 3D game render as the references; polished but worn riveted bronze, dark navy drill, black padded interior materials.
Composition/framing: true driver-eye camera within the cockpit, wide horizontal 3:2 frame, centered forward view, low rectangular vehicle proportions, symmetrical readable cockpit rim, generous clear forward sightline. Do not depict the vehicle from outside.
Lighting/mood: soft neutral studio lighting matching the reference pack, clean and uncinematic for continuity use.
Identity invariants: exact same low rectangular worn golden-bronze chassis design; exactly 6 road wheels total / 3 per side if any wheels are visible; exactly one central dark navy conical drill; exactly one side circular saw total; rear red urn beacon and triangular red light modules remain part of the same design but should only appear if physically visible; same pipes; same black padded seat; exactly two levers.
Constraints: no redesign; no extra wheels or tracks; no extra drills or saws; no steering wheel; no tall cab; no enclosed windshield; no instrument-screen UI; no labels, text, logo, border, caption, watermark, or character. Do not add futuristic holograms or dashboard displays.
```

## cabin-02-pov-wide.png — final targeted correction

```text
Use case: precise-object-edit / identity-preserve
Asset type: corrected horizontal Seedance 2.0 vehicle continuity reference panel
Input images: Image 1 is the edit target, the approved wide cockpit POV except for camera position. Image 2 is the exact Mars harvester identity sheet. Image 3 is the exact cockpit layout reference.
Primary request: Change ONLY the viewpoint/camera placement in Image 1: move the camera forward into the seated driver's true head-and-eye position. The black padded seat must be entirely behind the camera and NOT VISIBLE anywhere in frame. Preserve the same forward direction, wide horizontal framing, neutral off-white studio cyclorama, central single dark navy drill, small physically plausible left saw edge, bronze cockpit rim, dashboard, pipes, worn materials, lighting, and overall composition as closely as possible.
Control lock: exactly TWO short bronze control levers with dark red-brown ball knobs remain visible in the lower foreground. No additional controls, handles, steering wheel, screens, hands, arms, body, helmet, or character.
Identity invariants: exact same low worn golden-bronze Mars harvester; exactly one central dark navy conical drill; exactly one side circular saw total; exactly two short levers; no redesign, no extra wheels/tracks/drills/saws, no tall cab or windshield.
Constraints: seat completely out of frame behind the camera; neutral empty studio ahead; no character; no text, labels, UI, logo, border, caption, watermark, or holograms. This is a single targeted camera-position correction; keep everything else unchanged.
```

## cabin-03-pov-vertical.png — base generation

```text
Use case: stylized-concept
Asset type: 1024×1536-ish portrait / 2:3 panel designed as a 9:16 Seedance 2.0 driver-POV continuity reference
Input images: Image 1 is the primary exact Mars harvester identity sheet; Image 2 is its exact compact cockpit/interior reference; Image 3 is the approved wide first-person POV. Preserve the exact same vehicle and the exact same driver-eye cockpit viewpoint from Image 3 while reframing vertically.
Primary request: Create a portrait first-person driver-eye POV from inside the exact same Mars harvester, as if an invisible seated driver is looking forward through the low open cockpit. The worn golden-bronze cockpit rim and compact black dashboard occupy only the lower portion. Include exactly two short bronze control levers with dark red-brown ball knobs, matching the references. Directly ahead, the same single central dark navy conical drill is visible along the centerline from behind. A tiny peripheral edge of the vehicle's single side circular saw may appear only if physically plausible. No person, hands, arms, body, helmet, or character.
Scene/backdrop: empty orange-red Mars desert ahead, broad gentle dunes / flat dusty plain, distant low mesas softened by dust haze, no structures or props. Plenty of open horizon and sky for 9:16 video framing. No golem, no crystals, no rocks in the immediate path.
Style/medium: same stylized high-detail 3D game render as all references; worn riveted golden-bronze, dark navy drill, black padded interior; coherent materials and scale.
Composition/framing: tall 2:3 portrait, true seated driver-eye camera inside the cockpit, drill centered low-to-mid frame, dashboard and exactly two levers confined to the bottom quarter-to-third, long clear view over the empty landscape, horizon around the middle to lower-middle with generous dusty sky. Do not depict the vehicle from outside.
Lighting/mood: clear soft late-afternoon Mars light, warm orange environment, readable neutral continuity render, no dramatic action.
Identity invariants: exact same low rectangular worn golden-bronze chassis design; exactly 6 road wheels total / 3 per side if any are visible; exactly one central dark navy conical drill; exactly one side circular saw total; same red urn beacon, triangular red light modules, pipes, black padded seat, and exactly two levers. No redesign.
Constraints: empty landscape; no golem, no crystals, no character; no extra wheels or tracks; no extra drills or saws; no steering wheel; no tall cab; no enclosed windshield; no instrument-screen UI; no labels, text, logo, border, caption, watermark, or holograms.
```

## cabin-03-pov-vertical.png — final targeted correction

```text
Use case: precise-object-edit / identity-preserve
Asset type: corrected portrait 9:16 Seedance 2.0 vehicle continuity reference panel
Input images: Image 1 is the portrait edit target with the correct empty Mars landscape and cockpit identity except for camera position. Image 2 is the corrected approved true driver-eye wide POV and is the authoritative camera/interior reference. Image 3 is the exact Mars harvester identity sheet.
Primary request: Change ONLY the viewpoint/camera placement in Image 1 to match the true seated driver head-and-eye position established by Image 2. The black padded seat must be entirely behind the camera and NOT VISIBLE anywhere in frame. Preserve the tall 9:16-style portrait composition, empty orange Mars desert, distant low mesas and haze, generous horizon and sky, same single central dark navy drill aligned straight ahead, worn golden-bronze cockpit rim/dashboard/pipes, exactly two control levers, materials, lighting, and overall landscape as closely as possible.
Control lock: exactly TWO short bronze control levers with dark red-brown ball knobs remain visible in the lower foreground. No additional controls, handles, steering wheel, screens, hands, arms, body, helmet, or character.
Identity invariants: exact same low worn golden-bronze Mars harvester; exactly one central dark navy conical drill; exactly one side circular saw total if its edge is physically visible; exactly two short levers; no redesign, no extra wheels/tracks/drills/saws, no tall cab or windshield.
Constraints: seat completely out of frame behind the camera; empty Mars landscape with no golem, crystals, character, foreground rocks, structures, or props; no text, labels, UI, logo, border, caption, watermark, or holograms. This is one targeted camera-position correction; keep everything else unchanged.
```

## Concise Seedance 2.0 usage prompt

```text
Use the supplied 3×3 Mars harvester reference card as strict continuity authority. Keep the exact same low worn golden-bronze six-wheel chassis (three wheels per side), one central dark-navy conical drill, one side circular saw, rear red urn beacon, triangular red lights, pipes, hatch geometry, black padded seat and exactly two short control levers. For cockpit shots, use the true seated driver-eye camera shown in CABIN POV: seat behind camera and invisible, two levers low in frame, drill aligned straight ahead. Match the card's stylized high-detail 3D game-render materials and proportions. Do not redesign, add wheels/tracks/drills/saws, create a tall cab, or add characters, hands, text, UI, logos or watermarks.
```

## Deterministic card assembly

`_assemble-reference-card.ps1` builds the final PNG and 1200 px-wide JPEG preview. Each source is contain-fitted into its panel slot without cropping or stretching. Row and per-panel labels are drawn in bands outside the image panels.
