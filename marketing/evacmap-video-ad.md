# Build prompt: EVACMAP 22s video ad (Facebook + Instagram)

> Paste everything below this line into Claude. Put any real assets you have in `assets/` first (see §6).

---

You are a senior motion designer and a React/TypeScript engineer. Build a **cinematic, edgy, 22-second vertical video ad** for **EVACMAP** in **Remotion**, render it to MP4, and check every frame you ship. The ad runs as paid Reels/Stories/Feed on Facebook and Instagram in **Georgia**, so the on-screen text is **Georgian first** with a small English mono subline, echoing the product's own website.

## 1. Product facts (use ONLY these; invent no features, numbers or claims)

- **What it is:** a web app that turns an architectural floor plan into a printable evacuation plan. The tagline is **"ნახაზიდან საევაკუაციო გეგმამდე — 5 წუთში"** / *FROM FLOOR PLAN TO EVACUATION PLAN IN 5 MINUTES*.
- **How it works (4 steps):**
  1. **ატვირთე ნახაზი** / UPLOAD YOUR DRAWING: upload an architectural PDF or other vector drawing.
  2. **დაადასტურე კედლები და კარები** / DETECT WALLS: EVACMAP detects walls and doors automatically, and you just check the result.
  3. **მონიშნე გასასვლელები და „აქ ხართ“ წერტილები** / EXITS & YOU ARE HERE: mark the exits and the places where the plan will hang. EVACMAP builds the route automatically.
  4. **ჩამოტვირთე მზა PDF** / DOWNLOAD · A4 / A3 / A2: you get a print-ready PDF, with a separate sheet for each "You are here" point.
- **Routes follow the real geometry.** A route never crosses walls and always exits through real doors. The main route is a solid line, the alternative route is dashed, and routes can be edited by hand.
- **The finished sheet includes:** the client's logo in the header (white-label), the main route (solid), the alternative route (dashed), ISO 7010 pictograms, a "You are here" point, **დარეკე 112** (call 112), the assembly point, a legend in Georgian and English, fire-action instructions in Georgian and English, and safety equipment marked on the plan (fire extinguishers, first-aid kit, electrical panel room).
- **Pricing (VAT included):** **19₾** per floor, **9₾** per extra floor in the same building, **PRO 100₾/month** for unlimited floors and buildings. **The editor is free. You pay only when you download the final PDF.** Revisions and re-downloads are free for **12 months**.
- **The problem it replaces:** today you send the drawing to a specialist and wait hours or days. Every floor is billed as separate work, and every change (a moved door, a new partition) means going back and paying again.
- **Audience:** occupational health and safety (OHS) specialists, facility managers, architects and designers.
- **Standards wording, exactly as the site uses it:** "ISO 7010" and "ტექნიკური რეგლამენტი №370". Do not write "certified" or "approved".
- **URL:** `evac.hsai.app` · **CTA:** **დაიწყე უფასოდ** (Start free) · made by Omio Labs, the team behind HSAI.

## 2. Creative concept: "Days → 5 minutes"

The ad has two worlds:
- **Red, glitchy, cramped:** the old way (waiting, per-floor invoices, paying again for every change).
- **Calm green precision:** EVACMAP doing the work live. A grey drawing comes alive: walls are detected, routes draw themselves through the real doors, and it becomes a finished wall-ready sheet.

The **"how it's made" moment is the hero**. The viewer should feel the satisfaction of the route drawing itself. The tone is confident, sharp and a little cheeky. It is not a fear ad: no fire footage, no panic.

## 3. Storyboard: 30 fps, 660 frames, 1080×1920

| # | Frames | Visual | On-screen text (exact) | Motion |
|---|---|---|---|---|
| 1 | 0–36 | Black. A red hairline scan flickers. A grey architectural drawing lies tilted in 3D in the background, out of focus | **დღეები ლოდინში.** / mono sub `DAYS OF WAITING` | Word slams in (scale 1.15→1, 4-frame blur), RGB-split glitch on frames 0–6. A mono counter in the corner ticks up `00:00:00 → 72:00:00` |
| 1b | 36–72 | The same drawing duplicates into a stack of 5 sheets, each stamped with a red "invoice" bar | **5 სართული = 5 ცალკე სამუშაო.** | Sheets stack with a hard snap per beat |
| 1c | 72–108 | One door on the drawing flashes red, then the whole stack shakes | **კარი შეიცვალა? თავიდან გადაიხადე.** | Camera shake 3px, red flash, glitch out |
| 2 | 108–150 | **Hard cut to silence.** Pure black, then one thin green line draws horizontally across the screen | **ან — 5 წუთი.** / `OR — 5 MINUTES` | Text reveals with a clean mask wipe left→right. No glitch from here on |
| 3a | 150–225 | A floor plan drops in flat (top-down) and settles in grey linework. A step indicator `01 / 04` sits at the top | **ატვირთე ნახაზი** / `UPLOAD YOUR DRAWING` | Spring drop, soft shadow, slow push-in (scale 1→1.05 over the whole of scene 3) |
| 3b | 225–300 | A scan line sweeps top→bottom. Walls light up white-cyan as it passes and door gaps glow | **კედლები — ავტომატურად** / `DETECT WALLS` | Scan line with a glow trail. Walls fade to the detected color, staggered by y position |
| 3c | 300–375 | Green exit markers pop at 2 exits. A pulsing "You are here" pin drops. Then the **main route draws itself as a solid green line** through corridors and real door gaps, and the **alternative route draws dashed** | **გასასვლელები და „აქ ხართ“** / `EXITS & YOU ARE HERE` + small caption **მარშრუტი კედლებს არ კვეთს.** | Pins spring in. Routes animate with `strokeDashoffset`, with a small glowing head dot leading the line |
| 3d | 375–450 | The plan zooms out and becomes a **finished A-series sheet**: header with a logo placeholder, the plan, a legend, a 112 box, fire instructions and an assembly point | **მზა PDF · A4 / A3 / A2** / `DOWNLOAD` | Sheet elements build in a stagger (header, then plan, then legend, then 112, then instructions). Three paper sizes A4 / A3 / A2 fan out behind it |
| 4 | 450–540 | The sheet tilts in 3D like paper on a wall under a soft light sweep. Proof chips line up below it | Chips: **ISO 7010** · **ქართ. / ENG ლეგენდა** · **12 თვე უფასო შესწორებები** · small: `ტექნიკური რეგლამენტი №370` | 3D tilt (rotateY −12°→0°), a specular light sweep across the sheet, chips pop in on the beat |
| 5 | 540–660 | Black. A large price, then the logo and CTA. A green route line draws an underline under the logo | **19₾** / **ერთ სართულზე** · then **რედაქტორი უფასოა. იხდი მხოლოდ ჩამოტვირთვისას.** · then **EVACMAP** · **ნახაზიდან საევაკუაციო გეგმამდე — 5 წუთში** · button **დაიწყე უფასოდ →** · `evac.hsai.app` | Price counts up 0→19. The button pulses once. Hold the final frame for at least 45 frames |

**Bumper (6s, 180 frames):** scene 2 (opening on **საევაკუაციო გეგმა — 5 წუთში.**) → a compressed scene 3c (route-drawing hero, 75f) → scene 5 (CTA, 60f).

## 4. Design system

- **Fonts (they must cover Georgian):**
  - Headlines: **Noto Sans Georgian** 800–900, tight tracking (−1%).
  - Body: Noto Sans Georgian 500.
  - Mono sublines, counters and step numbers: **JetBrains Mono** 500, UPPERCASE, letter-spacing +8%.
  - Load the fonts with `@remotion/google-fonts` and wait for them before rendering. **Never let Georgian fall back to a system font or show tofu boxes.**
- **Colors:**
  - Background `#0A0D12` with a faint 40px blueprint grid at 6% opacity.
  - Drawing linework `#8A94A6`. Detected walls `#E8F1FF` with a cyan glow `#5FD3FF`.
  - Safety green `#00B25A` for routes, exits, the CTA and the whole calm world.
  - Alarm red `#E5322D`, used only in scene 1 and for the fire-extinguisher icons.
  - Text: white `#F5F7FA`, secondary `#9AA4B2`.
  - If `assets/brand.json` or screenshots show the real brand colors, use those instead.
- **Cinematic finish:** a subtle film grain overlay (animated noise at about 4% opacity), a soft vignette, 3D perspective on the plan (`perspective: 1600px`), light sweeps, and slow continuous push-ins (nothing static ever sits completely still). Use springs (`damping` around 14) for UI elements and ease-in-out cubic for camera moves.
- **Typography motion:** the red world uses slams with RGB-split glitch. The green world uses clean mask wipes and soft upward reveals (y +24px→0, opacity 0→1, 10 frames). Show at most two lines of headline at once. Keep mono sublines at 60% of headline width or less.
- **Safe zones (9:16):** no text in the top 250px or bottom 380px, and 64px side margins.

## 5. Build spec

- **Remotion + TypeScript project.** Create three compositions:
  - `Ad916`: 1080×1920, 660 frames.
  - `Ad45`: 1080×1350, 660 frames, **re-laid out, not cropped**: smaller plan, text placed beside or below it.
  - `Bumper916`: 1080×1920, 180 frames.
- **Floor plan:** build it as a **hand-authored SVG** of a believable office floor of roughly 8 rooms, a corridor, 2 stairwell exits and real door gaps in the walls. Define the main and alternative route polylines so that they **pass only through door gaps and corridors and never cross a wall line**. Write a tiny unit check that tests every route segment against the wall segments for intersections, and make it pass.
- **Real assets win.** If `assets/sample-a4.pdf` (or PNG), `assets/editor-*.png`, `assets/editor.mp4` or `assets/logo.svg` exist, use them:
  - the real sample sheet in scene 3d/4;
  - real editor screenshots or a recording inside a dark browser frame in scene 3, with your animated overlays (scan line, pins, routes) on top;
  - the real logo in scene 5.
  - Otherwise build stylized vector versions. Never fake readable UI text that the real product does not have.
- **Icons:** use simple, clean vector safety icons (a running-figure exit sign on a green square, an extinguisher on a red square, a first-aid cross, a lightning bolt for the electrical room, an assembly-point arrows icon). Prefer icons from `assets/icons/` if provided.
- **Audio:** if `assets/music.mp3` exists, add it with `<Audio>` and align the cuts to its beats (scene 2 must land in silence). Otherwise render without audio, list where the hits should land (frame numbers) in `AUDIO_CUES.md`, and include the music brief: *"22s modern minimal trailer cue: 0–3.6s glitchy distorted tension with ticking; 3.6–5s total silence; 5s sub-drop then a clean confident synth pulse at 120 BPM building with crisp percussion; one big resolving hit at 18s; tail to 22s. No vocals."*
- **Render:**
  - `out/evacmap-9x16.mp4`, `out/evacmap-4x5.mp4` and `out/evacmap-bumper-6s.mp4`, all H.264, yuv420p, CRF 18.
  - A poster frame `out/poster.png` taken from scene 3c, with the route half-drawn.
  - If Remotion can't download its headless browser, point it at an installed Chromium with `--browser-executable`.

## 6. QA (do this before you say you're done)

1. Render stills at frames **0, 20, 60, 100, 130, 200, 270, 340, 420, 500, 600 and 659** for each composition, and **look at every one**:
   - Georgian glyphs render correctly with no tofu or fallback font.
   - No text sits inside the safe zones or overflows its box.
   - Contrast is readable on a phone.
   - The route visibly never crosses a wall.
2. **Muted test:** from the stills alone, the story (pain → 5 minutes → 4 steps → real PDF → price → CTA) must be clear.
3. **First-frame test:** frame 0 must already show text, not a blank black frame.
4. Check durations with `ffprobe` (22.0s, 22.0s and 6.0s) and keep each file under 100 MB.
5. Report what you built, which real assets you used and which you stylized, and a contact sheet image of the stills.

## 7. Meta ad copy (also save it as `out/ad-copy.md`)

- **Primary text:** საევაკუაციო გეგმისთვის დღეებს ელოდები? EVACMAP-ში ატვირთავ ნახაზს — სისტემა თავად ამოიცნობს კედლებსა და კარებს, გაავლებს მარშრუტს რეალურ გასასვლელამდე და მოგიმზადებს დასაბეჭდ PDF-ს A4, A3 ან A2 ფორმატში. ISO 7010 ნიშნები, ქართულ-ინგლისური ლეგენდა, 12 თვე უფასო შესწორებები. რედაქტორი უფასოა — იხდი მხოლოდ ჩამოტვირთვისას. 19₾ სართულზე.
- **Short variant:** 5 სართული ≠ 5 ინვოისი. დამატებითი სართული — 9₾. 🟢
- **Headline:** ნახაზიდან საევაკუაციო გეგმამდე — 5 წუთში
- **Description:** რედაქტორი უფასოა · 19₾ სართულზე
- **CTA button:** Sign Up (or Learn More for cold audiences) → `https://evac.hsai.app`
