# EvacMap — 20s Video Ad (Facebook + Instagram)

**Concept:** *"When the alarm goes off, it's too late to draw the map."*
Open with tension (alarm, darkness, confusion), then cut hard to calm, precise control: the EvacMap workspace building a live evacuation plan in seconds. The whole ad lives in two colors: **alarm red** (the problem) and **exit-sign green** (EvacMap). Every viewer already knows that green means "the way out", so the brand gets that meaning for free.

---

## 1. Specs

| | |
|---|---|
| Length | 20s main cut, plus a 6s bumper cut (shots 1, 4 and 7) |
| Formats | **9:16** (Reels/Stories, master), **4:5** (Feed), 1:1 (fallback) |
| Safe zone (9:16) | Keep text out of the top 14% and bottom 20% (UI overlays) |
| Sound | Designed to work **muted**: every key line is burned-in text |
| Pace | Cut every 1.5–3s; first frame must stop the scroll |

## 2. Look and type

- **Palette:** Void black `#0A0B0D` · Alarm red `#FF2D2D` · Exit green `#00E07A` · Blueprint cyan `#5FD3FF` (thin lines only) · White `#F5F7FA`
- **Headline font:** *Clash Display* Semibold (free, Fontshare). Alternatives: *Neue Machina* or *Space Grotesk* Bold. All caps, tight tracking (-2%).
- **Body / UI labels:** *Inter* Medium.
- **Data / timers:** *JetBrains Mono* (countdowns, coordinates, "ROUTE 02 — 38m").
- **Text motion:** words slam in on the beat (scale 110% → 100%, 4-frame motion blur). Key words get a quick glitch/RGB-split in the red section and a clean mask-wipe reveal in the green section. Text never just fades.
- **Camera language:** red section is handheld, Dutch angles, strobe. Green section is locked-off, smooth push-ins, top-down orthographic views. The visual style itself shows the shift from chaos to control.

## 3. Shot list (20s)

| # | Time | Visual | On-screen text | Sound |
|---|---|---|---|---|
| 1 | 0.0–1.5 | Pitch black. A red strobe snaps on and shows a smoke-filled office corridor, handheld and shaky | **THE ALARM JUST WENT OFF.** (glitch in) | Fire alarm siren hits on frame 1 |
| 2 | 1.5–3.5 | Fast cuts: feet hesitating at a split corridor, a hand on a locked door, a blurry exit sign through smoke | **WHICH WAY OUT?** | Siren + heartbeat bass |
| 3 | 3.5–5.0 | Smash cut to silence. Black screen, monospace counter ticking `00:04` | **MOST TEAMS DON'T KNOW.** | Hard silence, single clock tick |
| 4 | 5.0–8.0 | A white-line blueprint floor plan unfolds in 3D from darkness and settles top-down. Glowing **green route lines draw themselves** from every room to the exits | **EVACMAP.** then **KNOW THE WAY OUT.** | Deep sub-drop, then a clean synth pulse begins (~120 BPM) |
| 5 | 8.0–13.0 | **Workspace montage** (real screen capture in a floating 3D device frame, slow push-in): drag floor plan in → exits snap into place → assembly point pin drops → route auto-calculates "ROUTE 02 · 38m · 41s" → zones color-code | Captions per beat: **UPLOAD.** · **MARK.** · **ROUTE.** · **DONE.** | Each UI action lands on a beat with a soft UI click |
| 6 | 13.0–16.5 | The plan flies off the screen into a grid of phones and tablets that light up green one by one, and a wall-mounted QR evacuation sign glows | **EVERYONE HAS THE PLAN. INSTANTLY.** | Music builds |
| 7 | 16.5–20.0 | Back in the corridor, now calm and lit. People walking (not running) in a clean line toward a glowing green exit. Final frame: logo on black, green underline wipes across | **EVACMAP** · **Build your evacuation plan in minutes.** · button: **TRY IT FREE →** | Music resolves on one final hit. Optional VO: "Know the way out." |

**6s bumper:** Shot 1 (1.5s) → Shot 4 (2.5s) → logo + CTA (2s).

## 4. AI video generator prompts

Use these in **Veo 3, Sora, Runway Gen-4, Kling or Hailuo**. Generate each shot separately (most tools produce 5–10s clips), then cut them together in CapCut / Premiere / DaVinci. Paste the style block at the end of every prompt so the shots match.

**Style block (append to every prompt):**
> Cinematic commercial, anamorphic lens, shallow depth of field, high contrast, deep crushed blacks, color palette limited to alarm red #FF2D2D and emergency-exit green #00E07A with thin cyan blueprint lines, volumetric haze, subtle film grain, 24fps, premium tech brand aesthetic like an Apple or Nothing product launch film, vertical 9:16, no text, no logos, no watermarks.

**Shot 1: The alarm**
> Total darkness, then a red emergency strobe light flashes on and reveals a modern open-plan office corridor filling with light smoke. Handheld camera, slightly tilted Dutch angle, urgent shaky movement forward. Red light pulses rhythmically and throws hard shadows. Tense, claustrophobic. [style block]

**Shot 2: Confusion**
> Fast close-up sequence: a person's sneakers stop abruptly at a T-junction in a smoky corridor and turn left, then right, unsure; a hand pushes a door handle that won't open; a green emergency exit sign glows faintly and out of focus through thick haze. Red strobe lighting, handheld, fast motion blur. [style block]

**Shot 4: The map appears (hero shot)**
> In a pure black void, glowing thin white architectural blueprint lines of an office floor plan draw themselves and unfold from flat 2D into a floating 3D wireframe building, then the camera rises smoothly to a perfect top-down view. Bright emerald-green light trails trace evacuation routes from every room toward the exits, like light flowing through veins. Clean, precise, calm, hypnotic. Slow smooth crane movement. [style block]

**Shot 6: Everyone gets the plan**
> A glowing green holographic floor plan lifts off a laptop screen and splits into dozens of copies that fly outward into a grid of floating smartphones and tablets in dark space; each device screen lights up emerald green one after another in a wave. Smooth, satisfying, elegant motion, reflective black surfaces. [style block]

**Shot 7: Calm exit**
> The same modern office corridor, now calm with soft clean light and light haze. A diverse group of office workers walks calmly in an orderly line toward a bright glowing green emergency exit door at the end of the corridor, seen from behind, slow steady dolly forward. Hopeful, controlled, reassuring. [style block]

**Shot 5 (workspace): do NOT generate this with AI.** AI tools invent fake UI and garbled text. Instead:
1. Screen-record the real EvacMap workspace at 2× resolution: upload plan → place exits → drop assembly point → generate route.
2. Speed up the recording to 2–4×, then drop it into a 3D device mockup with a slow push-in (Jitter, Rotato, After Effects, or CapCut's 3D templates).
3. Add a green glow pulse on each click, sync every action to a beat, and overlay the one-word captions.

## 5. Music and sound prompt

For Suno / Udio / Stable Audio, or as a brief for a stock library search (Artlist, Epidemic Sound):
> 20-second cinematic trailer cue for a tech ad. 0–3s: blaring fire alarm with distorted heartbeat sub-bass and tension. 3–5s: sudden silence with a single clock tick. 5s: deep sub-drop impact, then a clean modern minimal synth-pulse beat at 120 BPM, confident and uplifting, building with crisp percussion. Ends at 19s on a single huge resolving hit with a short reverb tail. No vocals.

Optional voiceover (calm, low, confident; one line only, at the end): **"EvacMap. Know the way out."**

## 6. Ad copy for Meta Ads Manager

- **Primary text (A, fear → relief):** When the alarm goes off, nobody reads a binder. EvacMap turns your floor plan into a live evacuation plan in minutes, with clear routes, exits and assembly points, shared to every phone. 🟢
- **Primary text (B, short and edgy):** Your team has 90 seconds. Do they know the way out?
- **Headline:** Know the way out.
- **Description:** Build evacuation maps in minutes.
- **CTA button:** Learn More (cold audiences) / Sign Up (retargeting)

## 7. Before you produce, check these

- [ ] Swap in the real product claims (e.g. "in minutes", "shared to every phone", "free trial"). Only say what EvacMap actually does.
- [ ] Use real UI footage for shot 5. It's the proof, and it's the "how it's made" moment.
- [ ] Watch it muted on a phone. The story must be clear from text alone.
- [ ] First frame test: pause on frame 1. Would it stop your thumb?
- [ ] Export: 1080×1920 H.264, under 4GB, with captions burned in, plus a 1080×1350 (4:5) recut.
