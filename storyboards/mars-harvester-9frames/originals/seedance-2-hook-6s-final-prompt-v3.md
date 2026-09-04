# Seedance 2.0 — хук «ремонт → Голем → кабина → gameplay» v3

Длительность: **6 секунд**
Формат: **9:16, 1080×1920, 30 fps**
Монтаж: **один непрерывный кадр без склеек**

## Референсы и приоритет

1. `@image1` — `C:\Users\hebp\OneDrive\Документы\Sorter\output\mars-harvester-seedance20-reference-card-v2\seedance20-harvester-reference-card-v2.png`
   - Единственный источник геометрии, масштаба, материалов, повреждений, закрытой и открытой крышки, кабины и POV нового харвестера.
   - Игнорировать сетку, подписи и студийный фон карточки.

2. `@image2` — `C:\Users\hebp\Downloads\grok-image-d959aa6b-0372-4da7-bcda-4d36f9dee4f3.jpg`
   - Единственный источник лица, фигуры, причёски, одежды и инструментов взрослой девушки-инженера.
   - Игнорировать имя, цифры, схемы, логотипы и весь текст character sheet.

3. `@image3` — `C:\Users\hebp\AppData\Local\Temp\codex-clipboard-f440b710-79d7-4897-9ce3-2d5acb4e7c34.png`
   - Источник синего Голема, оранжевой марсианской пустыни, красных и синих кристаллов, масштаба и финальной gameplay-камеры.
   - HUD использовать только как ориентир кадрирования; интерфейс внутри нейрохука не генерировать.

Исходный gameplay для монтажного стыка:
`C:\Users\hebp\Downloads\Mars Harvester Gameplay Trailer 0.5 Short.mp4`

## Visual theme

- Палитра: тёплый оранжевый песок, изношенная золотистая бронза, тёмно-синий бур, красные индикаторы и маяк, ярко-синие/красные кристаллы.
- Свет: направленный марсианский поздний день, мягкие стилизованные тени, лёгкая пыль в воздухе.
- Оптика: читаемая wide-to-medium мобильная игровая камера, умеренная перспектива без сверхшироких искажений.
- Рендер: premium stylized 3D mobile-game look, стабильные материалы и геометрия.
- Движение: один плавный gimbal-like кадр; короткий rack focus на Голема; затем проход в POV и быстрый dolly-back + crane-up к gameplay.

## Раскадровка — 9 ключевых кадров

| № | Время | Кадр и действие |
|---|---:|---|
| 01 | 0.00–0.55 | Строгий боковой medium-wide: инженер чинит одну боковую трубу одним ключом; крышка закрыта. |
| 02 | 0.55–1.20 | Крупнее: последний поворот ключа, обе руки анатомично контактируют с ключом и муфтой. |
| 03 | 1.20–1.85 | Тяжёлый шаг встряхивает пыль; инженер замирает и оборачивается; впервые виден один синий Голем у красных и синих кристаллов. |
| 04 | 1.85–2.50 | Она убирает ключ на пояс и тянется к единственной защёлке закрытой броневой крышки. |
| 05 | 2.50–3.20 | Крышка открывается вверх на задней петле; одна нога ставится на боковую ступень, одна рука держит край/поручень. |
| 06 | 3.20–4.00 | Одна цельная фигура забирается в просторную кабину; снаружи не остаётся дубликата; крышка открыта. |
| 07 | 4.00–4.55 | OTS внутри кабины: инженер уже сидит, впереди центральный бур, один Голем и кристаллы; видны ровно два коротких рычага. |
| 08 | 4.55–5.20 | Истинный driver-eye POV: сиденье за камерой и невидимо; правая рука нажимает одну красную кнопку запуска; бур строго по центру. |
| 09 | 5.20–6.00 | Камера вылетает назад и вверх в высокий 3/4 gameplay view; та же машина с открытой крышкой разгоняется к Голему, шесть колёс бросают короткий шлейф пыли; HUD отсутствует. |

## Identity lock — харвестер

```text
The harvester must remain the exact same large low-profile mining rover from @image1 in every moment: a worn golden-bronze rectangular armored body approximately twice the standing height of the adult engineer, exactly six road wheels total with three wheels on each side, exactly one centered dark-navy conical spiral drill at the front, exactly one lateral serrated circular saw total, one rear red urn-shaped beacon, the same triangular red indicator clusters, exposed bronze pipes and gears, one thick armored cockpit hatch hinged at the rear, one black padded seat, and exactly two short control levers with dark red-brown ball knobs. Preserve the same panel layout, dents, scratches, oxidized metal, scale and proportions. The one side saw may be occluded when the camera is on the opposite side; never mirror or duplicate it. No tracks, no second drill, no second saw, no extra beacon, no cyan rear module, no tall truck cab, no roll cage, no windshield, no enclosed roof and no invented controls.
```

## Identity lock — инженер

```text
The engineer must remain the exact same single adult human woman from @image2 in every frame: age 24–28, warm light skin, brown eyes, soft mature face, dark-brown hair in one high messy bun with the same loose face-framing strands, pink-tinted mechanic goggles on top of her head, the same adult proportions, cropped off-white mechanic jacket with rolled sleeves and the same V-shaped neckline, dark shoulder harness, off-white high-waisted cargo trousers, identical pink heart patches, black-and-pink tool belt, black fingerless gloves, and white-and-pink lace-up work boots. Preserve her face, body, hair, outfit seams, patches, colors and equipment. Never duplicate her, change her clothes, make her childlike, or add/remove limbs.
```

## Финальный промт для Seedance 2.0

```text
Use @image1 as the sole and strict continuity authority for the new Mars harvester exterior, scale, closed/open hatch mechanism, cockpit interior and driver-eye POV. Use @image2 only as the strict identity authority for the same single adult female engineer. Use @image3 only for the one blue golem, orange Martian desert, red and blue crystals, relative scale and the final high three-quarter gameplay camera. Ignore all grids, labels, typography, diagrams, measurements, borders, logos and interface elements printed inside the reference sheets. Generate one continuous 6-second vertical 9:16 shot, 1080×1920, 30 fps, with synchronized audio and no cuts.

0.00–1.20: begin in a clean medium-wide strict side view at adult eye level. The exact adult female engineer from @image2 stands beside the exact stationary harvester from @image1 and tightens one exposed side-pipe coupling with one wrench. The machine is a large low-profile rover, approximately twice her standing height; its three near-side wheels are large and readable. Its single thick armored hatch is closed. Orange Martian sand surrounds them, with one red and one blue crystal cluster in the middle distance. Move gently closer to a readable close-up of both anatomically correct hands completing the final wrench turn. Preserve exact tool-to-hand-to-coupling contact.

1.20–1.85: one heavy stone footstep makes dust tremble and shake loose from the machine. The engineer freezes, then turns her head toward the sound. Use a smooth rack focus and slight pan to reveal exactly one chunky blue golem from @image3 approaching in front of the vehicle near the red and blue crystals. Maintain geography and screen direction; hatch remains closed.

1.85–3.20: she secures the same wrench on her tool belt, reaches the single hatch latch, releases it and lifts the exact thick bronze hatch upward on its rear hinge. The mechanism and opening remain identical to the OPEN HATCH row of @image1. She grips the hatch edge or side handhold and plants one boot on the real side access step. Keep the vehicle low, long and six-wheeled; do not transform it into a truck or buggy.

3.20–4.00: in one readable physically continuous motion, the same woman climbs and vaults through the open hatch into the single spacious cockpit. Her hands and feet contact real steps and edges; her body remains anatomically coherent. Once inside, no duplicate woman remains outside. The same hatch stays open and the black padded seat, bronze cockpit rim, pipes and exactly two short control levers match @image1.

4.00–5.20: without a cut, camera follows into a brief over-the-shoulder view of her seated in the cockpit, then settles into the true seated driver-eye position shown in the CABIN POV row of @image1. The black seat is behind the driver-eye camera and invisible. The worn bronze dashboard occupies only the lower portion, exactly two short levers remain visible, and the single dark-navy drill is aligned straight ahead. Her right gloved hand presses exactly one red ignition button once. Exactly one blue golem is visible ahead beside one red and one blue crystal cluster. Do not show symmetric saws; this vehicle has only one lateral circular saw total.

5.20–6.00: ignition whine becomes a compact engine roar. The same six wheels begin spinning and throw a short orange dust plume. The camera flies smoothly backward out through the open hatch, continues in a fast dolly backward combined with crane upward and a gentle tilt down, revealing the exact same large six-wheel harvester accelerating toward the blue golem. End in the high three-quarter gameplay composition from @image3, with the vehicle scale, travel direction, desert lighting, golem position and red/blue crystal placement prepared for a direct hard cut into the original gameplay. The generated hook remains HUD-free; the real HUD appears only after the cut.

Strict continuity: one adult engineer, one harvester and one blue golem. Harvester lock: exactly six wheels total / three per side, one centered dark-navy drill, one lateral circular saw total, one rear red urn beacon, one thick rear-hinged armored hatch, one black seat and exactly two short levers. Keep the hatch closed through the repair and golem reveal, open it once, then keep it open through acceleration. Keep the wrench physically in her hands, on her belt or touching the coupling; never let it float or disappear. Preserve her face, bun, pink goggles, off-white/pink mechanic outfit, gloves, tool belt and boots. Warm orange / oxidized gold / dark navy / red / crystal blue palette, premium stylized 3D mobile-game rendering, smooth stable geometry.

No cuts, no morphing, no teleportation, no duplicate woman, no extra people, no extra golems, no red golem, no drones, no vehicle redesign, no extra or missing wheels, no tracks, no second drill, no second saw, no symmetric twin saws, no extra beacon, no cyan rear module, no tall cab, no roll cage, no windshield, no enclosed roof, no weapons, no lasers, no deformed hands, no fused limbs, no floating tool, no costume or hair change, no reference-sheet layout, no text, no title, no measurements, no logo, no watermark, no generated HUD and no UI. Cinematic 1080p, synchronized audio.
```

## Audio direction

```text
Dry metal wrench clicks and a quiet machine tick; one deep stone footstep with a short sand vibration at 1.2 seconds; hatch latch clack and heavy bronze hinge movement; cloth, boots and metal during the climb; one ignition button click, rising mechanical whine, compact engine roar, six tires grinding orange sand and a short tension hit. No dialogue and no voice-over.
```

## Монтаж

- Обрезать генерацию ровно на `6.00 s`.
- Следующим кадром поставить настоящий gameplay без dissolve.
- HUD должен впервые появиться только в реальном gameplay.
- Если направление совпало неидеально, использовать только 2–4 кадра directional blur на стыке.
