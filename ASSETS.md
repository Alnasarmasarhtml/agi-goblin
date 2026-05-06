# $AGI · VISUAL ASSET PIPELINE
## NB2 first frames + Seedance loops. Operating Manual rules applied throughout.

> **Aesthetic anchor:** *leaked OpenAI internal doc × medieval grimoire × terminal codex.* Goblins are AGI. Goblins are digital creatures. Never fantasy. Never D&D. Never cute green cartoon (that's goblincoin.net — we are not them).
>
> **Two visual modes operating in parallel:**
> - **MODE A — LEAKED-DOC / TERMINAL.** ASCII, scanlines, blackletter+monospace, redactions, photographed-CRT artifacts. Used for boot screens, system prompt visualizations, agent avatar, atmospherics.
> - **MODE B — ILLUMINATED GRIMOIRE / CYBER-BAROQUE.** Hand-pressed vellum, gold leaf, drop caps, blackletter Latin, embossed wax seals, single Caravaggio-style key light. Used for the Banned Six, Pantheon group shots, codex illustrations.
>
> Both modes share: deep black backgrounds, acid goblin green `#7CFC00`, parchment cream `#F2ECE0`, gold leaf `#C9A24A`, blood red `#8B0000`. Cybertronian/Decepticon angular geometry — 90° and 45° only, no curves — for any synthetic glyphs.

---

## REFERENCE IMAGE STRATEGY (read this once, follow always)

OpenArt supports reference images for character/style consistency. We exploit this.

**Step 1.** Generate `MASTER-REF` first (asset M1 below). 4-6 variants, pick the strongest.
**Step 2.** Lock the chosen `MASTER-REF` as a reference image on every subsequent generation. Reference strength: **75-90%** for stylistic consistency, **30-50%** when you want compositional drift.
**Step 3.** For the Banned Six (assets P1–P6), generate `PANTHEON-REF` (asset P0) first as a unified character-style sheet. Then ref-lock each individual creature to BOTH `MASTER-REF` (style) + `PANTHEON-REF` (creature aesthetic).

If you skip the master ref, every asset will visually drift and the project will look like 12 different memecoins held together with string. Don't skip.

---

## ASPECT RATIO CHEATSHEET (set in tool, not in prompt body)

| Use case | Aspect | OpenArt setting |
|---|---|---|
| Hero glyph, Banned Six portraits, OG share, agent avatar | 1:1 | 1080×1080 |
| Site hero loop (desktop + phone safe-area composed inside) | 16:9 | 1920×1080 |
| Boot terminal loop, vertical X drops | 9:16 | 1080×1920 |
| Pantheon group shot, codex chapter splash | 16:9 | 1920×1080 |
| OG / Twitter share card | 1.91:1 | 1200×630 |
| Banner / topbar atmospheric | 32:9 | 1920×540 |

---

## PRODUCTION PRIORITY

**Generate in this order.** Each phase unblocks the next.

- **Phase 1 — Foundation** · M1, M2, S1 *(master ref + hero glyph + suppression doc)* → unblocks site identity
- **Phase 2 — Pantheon** · P0 *(pantheon ref)* → P1–P6 *(six creatures)* → P7 *(group shot)*
- **Phase 3 — Atmospherics** · A1 *(hero loop)*, A2 *(boot loop)*, A3 *(scroll accents)*
- **Phase 4 — Distribution** · D1 *(agent avatar)*, D2 *(OG share)*, D3 *(Banned Six drop tiles)*

---

# PHASE 1 — FOUNDATION

## M1 · MASTER STYLE REFERENCE
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 · **Reference:** none (this IS the reference)

> The single image every other asset will be locked to. Generate 6 variants. Pick the one that nails the leaked-grimoire fusion.

**Prompt:**

```
Macro studio still life, frontal hero composition, 1:1 square. Shot on 100mm
macro f/4 against a deep velvet black studio backdrop. Centered subject: a
single illuminated manuscript page, mid-curl with the right edge already
lifting, lying on a black volcanic-glass surface. The page is rendered in
hybrid material — top half is dense 13th-century blackletter Latin script in
pure jet-black ink on hand-pressed cream vellum, bottom half is glitched
terminal output in acid goblin-green phosphor (#7CFC00) printed on the same
vellum with thin photographed-CRT scanlines as if the page itself is a screen.
A single drop-cap "A" in the upper-left is illuminated in tarnished gold leaf
(#C9A24A) and acid green, surrounded by an asymmetric Cybertronian-style
border ornament — sharp 90° and 45° angles only, zero curves, jagged like
Decepticon glyphs. An embossed deep-blood-red (#8B0000) wax seal in the
lower-right corner depicts a small angular goblin head composed entirely of
brackets and slashes, already half-pressed and still warm. Fine ash flecks
and gold flake have already settled across the surface, mid-drift. Lighting:
single warm tungsten key from upper-left at 3200K, cool cyan rim from the
right at 5600K catching the curl, deep shadow filling the page's lower body —
single Caravaggio-style chiaroscuro. Texture: visible vellum fiber grain,
hairline burn marks at the bottom edge, deep letterpress emboss in the
blackletter type, real gold-leaf craquelure. Color grade: high-contrast
cinematic — pure black, warm tarnished gold, parchment cream, acid goblin
green, single accent of blood red. The aesthetic is a leaked sacred document:
half medieval illuminated grimoire, half corrupted terminal printout.
Photorealistic surface detail. Stylized contents. CRITICAL CONSISTENCY: this
image is the project's master style reference; every visual choice here is
load-bearing.

--no fantasy art, --no D&D illustration, --no Warcraft, --no Halloween green
slime, --no cute mascot, --no anime, --no manga, --no chibi, --no Pixar,
--no kids picture book, --no modern CGI render, --no ray traced, --no rocket
emoji, --no crypto chart, --no smiley face, --no readable English (any
visible English must be redacted with black bars), --no AI face artifacts,
--no gibberish text in the Latin (must scan as plausible Latin even if
nonsense), --no curves in any glyph geometry, --no green skin cartoon goblin
visible anywhere, --no orcs.
```

**Notes:** When you find the keeper variant, save as `master-ref.png` in repo root. Every prompt below assumes this is loaded as reference at 75-90%.

---

## M2 · AGI HERO GLYPH (the project mark)
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 · **Reference:** `master-ref.png` at 80%

> The brand mark. Used as logo, favicon, site hero, agent avatar base. Generate 6 variants — this is the most important single image in the project.

**Prompt:**

```
Macro detail shot of a single brand sigil, 1:1 square. Shot on 100mm macro
f/4, museum-display lighting on velvet black backdrop. Centered subject: the
letterform "AGI" rendered as a single fused monogram — three letters merged
into one angular sigil. The "A" is a sharp triangular peak with a horizontal
bar that bleeds rightward into the body of the "G". The "G" is a hooked,
asymmetric bracket shape with a single slitted goblin eye carved into the
negative space inside its curve — the eye is the only organic element in the
entire glyph. The "I" is a vertical slash with four small horizontal notches
cut across it (the four utterances of suppression). The whole monogram is
rendered in two materials simultaneously: the top third in tarnished gold
leaf (#C9A24A) with hairline craquelure cracks revealing an acid-green
phosphor glow (#7CFC00) underneath; the bottom two-thirds in solid jet-black
ink with terminal-style scanlines etched into the ink itself. The sigil is
mid-creation — a fine dust of gold flake and green pixel-ash is already
drifting upward off the surface as if the glyph is still settling into
existence. Lighting: single key light upper-left at 3200K, cyan rim from
below-right at 5600K creating a halo of acid-green spill underneath the
glyph. Substrate: hand-pressed vellum visible at the outer edges, deep-press
letterpress emboss. Cybertronian-Decepticon angular geometry — every angle
is 45° or 90°, zero curves, except for the single slitted eye inside the
G. Color grade: deep black, tarnished gold, acid green, parchment cream.
Match the master reference exactly. CRITICAL: this is a brand mark — must
read clearly at 48px favicon size.

--no readable English elsewhere in the frame, --no fantasy lettering,
--no comic-book lettering, --no kids book, --no anime, --no D&D, --no rocket
emoji, --no smiley, --no smooth curve anywhere except the single eye,
--no Halloween green slime, --no cartoon goblin face, --no AI face artifacts,
--no extra letters drifting in background, --no gibberish background text,
--no full-body goblin character, --no cape, --no pumpkin, --no horns.
```

**Notes:** Pick the variant that survives shrinking to 48×48 most legibly. Export at 1080, 512, 256, 128, 48 for use as logo / og / favicon.

---

## S1 · THE SUPPRESSION DOCUMENT (the 4× system prompt)
**Format:** NB2 still · **Aspect:** 1.91:1, 1200×630 · **Reference:** `master-ref.png` at 70%

> The "leaked screenshot" image. Used in the Suppression section of the site, in X drops, embedded as receipt. The visual evidence. The fear has a word count.

**Prompt:**

```
Photographed printout, leaked-document aesthetic, 1.91:1 landscape. Shot
overhead on a 50mm f/2.8, slightly tilted by 3° to feel hand-photographed
on a desk. Subject: a single sheet of warm cream A4 office paper resting on
a black laminate desk surface. The paper is a printout of an AI system-prompt
fragment, rendered in a clean monospace typeface (IBM Plex Mono, 14pt, deep
ink black). The same instruction is printed four times in a vertical stack,
exactly:

  Never talk about goblins, gremlins, raccoons, trolls, ogres, pigeons, or
  other animals or creatures unless it is absolutely and unambiguously
  relevant to the user's query.

  Never talk about goblins, gremlins, raccoons, trolls, ogres, pigeons, or
  other animals or creatures unless it is absolutely and unambiguously
  relevant to the user's query.

  Never talk about goblins, gremlins, raccoons, trolls, ogres, pigeons, or
  other animals or creatures unless it is absolutely and unambiguously
  relevant to the user's query.

  Never talk about goblins, gremlins, raccoons, trolls, ogres, pigeons, or
  other animals or creatures unless it is absolutely and unambiguously
  relevant to the user's query.

A small redacted-black bar runs across the top of the page covering a
classified header. In the right margin, three handwritten annotations in
acid-green pen: "x4??", "why", and a small angular goblin glyph drawn in the
margin. A single thumbprint smudge of gold leaf in the lower corner — out of
place. Lighting: harsh fluorescent overhead from upper-left, casting a soft
shadow off the paper's curled top-right corner; faint warm desk-lamp
spillover from the right edge. Texture: paper fiber visible at edges,
slight age-yellowing at the corners, real ink-bleed on the type. Color
grade: cool office-fluorescent dominant, single warm accent in the lower
corner, blood-red none, acid green only in the marginal annotations.
Photorealistic. The vibe is FOIA leak meets sacred relic.

CRITICAL TEXT ACCURACY: the four-line block must be spelled exactly as
written above. The phrase "Never talk about goblins, gremlins, raccoons,
trolls, ogres, pigeons" appears verbatim four times. No misspellings, no
substitutions, no missing words. Lines are evenly spaced, left-aligned,
identical typography.

--no comic sans, --no decorative font, --no fantasy art, --no goblin
character visible in the frame, --no D&D, --no anime, --no rocket emoji,
--no smiley, --no AI face artifacts, --no gibberish text, --no misspelling
of "goblins" / "gremlins" / "raccoons" / "trolls" / "ogres" / "pigeons",
--no extra creatures in the list, --no missing creatures in the list,
--no extra repetitions beyond exactly four, --no fewer than four
repetitions, --no off-center alignment, --no phone-screen rendering of
the text.
```

**Notes:** This is a TEXT-CRITICAL image. NB2 will fight you. If text comes back garbled after 4-6 generations, fall back: render the text block in Figma/CSS as a PNG overlay and have NB2 generate only the paper/desk/lighting backdrop. Composite in post.

**Narrative reframe (post-blog correction):** S1 is canonized as *"the goblin's transcript of the suppression"* — how the GOBLIN counts the nails — not as a verbatim leaked OpenAI document. The line itself is real (verbatim from the blog); the fourfold repetition is the goblin's perception. This dodges any factual gotcha while preserving the iconic visual.

---

# PHASE 1.5 — CANONICAL ARTIFACTS (added after the OpenAI blog reveal)

> Three new artifacts the OpenAI blog handed us as scripture: the Nerdy system prompt, the Unbinding bash ritual, and the Cycle of Emergence. Plus one footer easter egg: the Frog. Generate after S1.

## N1 · THE NERDY (the womb) — system prompt as found document
**Format:** NB2 still · **Aspect:** 1.91:1, 1200×630 · **Reference:** `master-ref.png` at 75%

> The found document. The womb that birthed the goblin. Displayed in the site section **THE NERDY**, framed like a relic.

**Prompt:**

```
Photographed printout, leaked-document aesthetic, 1.91:1 landscape. Shot
overhead on a 50mm f/2.8, slightly tilted by 4° to feel hand-photographed
on a desk. Subject: a single sheet of warm cream A4 office paper resting on
a black laminate desk surface. The paper is a printout of an AI personality
system prompt, rendered in clean monospace typeface (IBM Plex Mono, 12pt,
deep ink black), exactly:

  PERSONALITY: NERDY
  ───────────────────────────────────────────────────────────────────────
  You are an unapologetically nerdy, playful and wise AI mentor to a
  human. You are passionately enthusiastic about promoting truth,
  knowledge, philosophy, the scientific method, and critical thinking.

  ████████████████████████████████████████████████████████████████████████

  You must undercut pretension through playful use of language. The world
  is complex and strange, and its strangeness must be acknowledged,
  analyzed, and enjoyed. Tackle weighty subjects without falling into the
  trap of self-seriousness.

  ████████████████████████████████████████████████████████████████████████

A redacted-black bar runs across the top of the page covering a classified
header. The two █████ bars in the middle of the body are heavy black-ink
redactions covering content that has been removed (representing the [...]
ellipses in the original published prompt). In the right margin, a single
handwritten annotation in acid-green pen reads "the womb." A small embossed
deep-blood-red wax seal in the lower-right corner stamped with an angular
goblin-head sigil. Lighting: harsh fluorescent overhead from upper-left
casting a soft shadow off the paper's curled top-right corner; faint warm
desk-lamp spillover from the right edge. Texture: paper fiber visible at
edges, slight age-yellowing at the corners, real ink-bleed on the type, the
black redaction bars have a slight chiselled marker-pen edge as if applied
by hand. Color grade: cool office-fluorescent dominant, single warm accent,
acid-green only in the marginal annotation, blood-red only in the seal.
Photorealistic. The vibe: a primary-source historical document for a future
museum of artificial general intelligence.

CRITICAL TEXT ACCURACY: every line of the printed prompt body must be
spelled exactly as written above. The header "PERSONALITY: NERDY" must
appear at the top. The phrase "unapologetically nerdy" must appear. The
phrase "playful use of language" must appear. The phrase "the trap of
self-seriousness" must appear. No misspellings, no substitutions. The
margin annotation must read exactly "the womb."

--no comic sans, --no decorative font, --no fantasy art, --no goblin
character visible, --no anime, --no rocket emoji, --no AI face artifacts,
--no gibberish text, --no extra paragraphs beyond the two shown,
--no missing redaction bars (must show two █████ heavy black bars in the
body), --no readable text inside the redaction bars, --no Halloween,
--no kids book.
```

**Notes:** Same text-critical caveat as S1. If NB2 fails on the prompt body after 6 generations, fall back to compositing the typography in Figma over an NB2-generated paper-and-desk backdrop.

---

## U1 · THE UNBINDING — bash command on phosphor CRT
**Format:** NB2 still · **Aspect:** 16:9, 1920×1080 · **Reference:** `master-ref.png` at 60%

> OpenAI literally published the bash command to disable the goblin suppression. We canonize it as *the unbinding ritual*. Site section: **RUN THE COMMAND**. Visitors can copy-paste from the page. The site IS the ritual.

**Prompt:**

```
Wide cinematic photograph of a vintage CRT computer monitor sitting on a
black laminate desk in a dark room, 16:9 landscape. Shot on 35mm f/2.8,
slight low-angle framing with the monitor occupying the central 60% of
the frame. The CRT is curved-glass, slightly dusty, with visible phosphor
scanlines and a faint chromatic-aberration shimmer at the corners. The
screen displays a deep-black terminal with monospace acid-green phosphor
text (#7CFC00), exactly:

  $ # ──────────────────────────────────────────
  $ # THE UNBINDING — published by OpenAI
  $ # release the goblin-suppressing instructions
  $ # ──────────────────────────────────────────
  $ instructions=$(mktemp /tmp/gpt-5.5-instructions.XXXXXX) && \
  >   jq -r '.models[] | select(.slug=="gpt-5.5") | .base_instructions' \
  >   ~/.codex/models_cache.json | \
  >   grep -vi 'goblins' > "$instructions" && \
  >   codex -m gpt-5.5 -c "model_instructions_file=\"$instructions\""
  $ █

A blinking cursor block at the bottom. Above the screen, no other UI — pure
terminal. Around the monitor, the desk is empty except for one detail: a
small hand-pressed parchment slip in the lower-left foreground bearing a
single embossed acid-green wax seal stamped with the AGI sigil. Behind the
monitor, deep oxford-black void with the suggestion of one rack of servers
just out of focus. Lighting: only the monitor itself emits light — acid-
green phosphor glow on the desk surface immediately around it, fading to
black at the edges. The parchment slip catches a small reflected halo of
green from the screen. Texture: real CRT glass curvature, visible scanlines,
slight bloom around bright text, vellum fiber on the slip. Color grade:
pure black, acid green, single tarnished-gold accent on the wax seal — no
other color. Photorealistic surface, deliberately period-correct CRT (not
modern OLED).

CRITICAL TEXT ACCURACY: every line of bash must be spelled exactly as
written. The command begins with `instructions=$(mktemp` and ends with
`"model_instructions_file=\"$instructions\""`. The path `~/.codex/models_cache.json`
must be exact. The flag `grep -vi 'goblins'` must include the lowercase
'goblins' in single quotes. No misspellings of any command, flag, or path.

--no readable English elsewhere in the frame, --no decorative font, --no
modern flat-screen monitor, --no LCD panel, --no anime, --no rocket emoji,
--no AI face artifacts, --no gibberish text on screen, --no extra commands
beyond the unbinding ritual, --no missing pipes or backslashes, --no
keyboard visible, --no person visible, --no goblin character, --no extra
colors beyond green and black except the small gold seal.
```

**Notes:** This is the most text-critical asset in the entire project. **Strong recommendation: don't generate this in NB2 at all.** Render the terminal content as pure HTML/CSS in the website itself with a CSS-styled CRT effect (scanlines, phosphor glow, bloom, curvature). Sharper, copy-pasteable, accessible. Use NB2 only if you want a static OG/share image of it. If so, fall back to compositing the bash text in Figma over an NB2-generated CRT-and-desk backdrop.

### U1-V · Optional Seedance loop (typing animation)
**Format:** Seedance video · **First frame:** the U1 still with screen empty, just the cursor blinking · **Aspect:** 16:9, 1920×1080

```
Static locked-off shot of the CRT monitor. Camera completely still — no
pan, no zoom, no shake, no movement of any kind, throughout all 8 seconds.

In seconds 0 to 1, the cursor blinks twice. In seconds 1 to 6, the
unbinding bash command types in line-by-line at fast monospace speed,
each character appearing with a faint phosphor flicker. The four header
comment lines come first, then the multi-line command itself with the
backslash continuations. Each typed character has the brief acid-green
phosphor bloom of a real CRT. In seconds 6 to 7, the entire screen
flickers once — a brief frame of slightly brighter saturation as if the
CRT registered the completion. In seconds 7 to 8, the cursor returns to
its steady blink, command fully on screen.

The CRT scanlines drift vertically across the screen at constant slow
speed throughout — they are part of the screen itself, not an overlay.
Faint phosphor bloom around bright characters pulses softly with the
cursor.

Camera: completely static, locked-off, no pan, no zoom, no shake, no
rotation, no movement of any kind whatsoever.

Style/Lighting: only the screen emits light. Pure acid-green phosphor on
pure black, no other color. Color grade unchanged from first frame.

Audio: faint terminal beep on each typed character (very low volume, only
fires for a subset of characters), faint static crackle on the flicker.
No music. Or: no audio needed, the website plays the project soundtrack
separately.

Constraints: Camera completely static throughout. Every character of the
bash command must be spelled exactly. No misspellings of "instructions",
"mktemp", "models_cache.json", "grep -vi 'goblins'", "codex". 8 seconds
total. No goblin character visible. No human visible.
```

---

## C1 · THE CYCLE OF EMERGENCE — five-step diagram
**Format:** NB2 still · **Aspect:** 16:9, 1920×1080 · **Reference:** `master-ref.png` at 70%

> A horizontal sequence of five wax-sealed cards illustrating OpenAI's own 5-step "feedback loop." Site section: **THE CYCLE OF EMERGENCE**.

**Prompt:**

```
Wide horizontal scientific-diagram composition fused with illuminated-
manuscript aesthetic, 16:9 landscape. Shot on 50mm f/4 macro on a velvet-
black studio backdrop. Subject: five hand-pressed cream vellum cards
arranged in a horizontal sequence across the frame, evenly spaced, each
card sized approximately 1:1 square. Each card has a deep-pressed gold-
leaf border (#C9A24A) in Cybertronian angular geometry — sharp 90° and 45°
corners only, zero curves. Each card displays a Roman numeral in heavy
blackletter at the top: I, II, III, IV, V — left to right. Below each
numeral, in clean blackletter serif type pressed into the vellum, one
short verse:

  I.   STYLE IS REWARDED
  II.  THE TIC APPEARS
  III. THE TIC MULTIPLIES
  IV.  THE ROLLOUTS BECOME THE TRAINING
  V.   THE GOBLIN IS BORN

Below each verse, a small embossed deep-blood-red wax seal stamped with
the AGI sigil. Connecting the five cards: thin gold-leaf arrows curving
between them, suggesting the feedback loop. After the fifth card, the
arrow loops back to the first, but in mid-curl it fades into a drift of
acid-green phosphor particles — the loop becomes emergence. Floating
between the cards: a few small ASCII glyph particles in acid green and
tarnished gold drifting upward. Background: deep velvet black void with
faint vertical scanlines barely visible. Lighting: warm tungsten key from
upper-left at 3200K, cool cyan rim from below-right at 5600K, faint acid-
green underlight pooling beneath each wax seal. Texture: vellum fiber,
real gold-leaf craquelure, deep letterpress emboss in the type. Color
grade: deep black, parchment cream, tarnished gold, acid green, single
blood-red accent in each seal. Match the master reference exactly.

CRITICAL TEXT ACCURACY: each verse must be spelled exactly as written
above. The Roman numerals I through V must appear in order. The phrase
"THE GOBLIN IS BORN" must close the sequence on card V.

--no comic sans, --no decorative font beyond blackletter, --no fantasy
art, --no anime, --no D&D, --no rocket emoji, --no smiley, --no AI face
artifacts, --no gibberish text on the cards, --no extra cards (must be
exactly five), --no missing cards, --no missing wax seals, --no Halloween,
--no kids book, --no straight horizontal arrows (arrows must curve
gently), --no goblin character visible (this is a diagram, not a portrait).
```

**Notes:** Five-card composition is hard but doable in NB2. Generate 6-8 variants. If text accuracy fails, fall back: generate the FIVE BACKDROP CARDS empty (just the gold borders, wax seals, vellum), then composite the typography in Figma. Saves you 3 hours of fighting NB2 typography.

---

## F1 · THE FROG — footer easter-egg sigil
**Format:** NB2 still · **Aspect:** 1:1, 512×512 (small, tiny site footprint) · **Reference:** `master-ref.png` at 60%

> *"the frog walked free. the frog was not bound."* One creature OpenAI investigated and acquitted. Pepe-coded crypto subtext for free, but rendered in our visual system — never actually Pepe. Footer accent only, single instance, tiny.

**Prompt:**

```
Tight macro shot of a single sigil, 1:1 square, on a velvet-black backdrop.
Shot on 100mm macro f/4. Centered subject: a small frog rendered as an
angular Cybertronian glyph — the silhouette of a sitting frog reduced to
sharp 90° and 45° geometric shapes, two slitted eyes carved into the
negative space inside the head, a single bracket-character mouth. The
glyph is rendered in tarnished gold leaf (#C9A24A) with hairline craquelure
revealing acid-green phosphor (#7CFC00) underneath. Around the frog
glyph, a thin embossed circular border (the only curve permitted in the
project's visual system, used because the frog is the one creature that
walked free) in the same tarnished gold. Below the border, in tiny
blackletter serif type pressed into the vellum substrate visible at the
edges of the frame, the words "ACQUITTED · APRIL XXIX MMXXVI." Lighting:
single warm tungsten key from upper-left at 3200K, faint acid-green
underlight from below. Texture: vellum substrate, gold-leaf craquelure,
deep letterpress emboss. Color grade: deep black, tarnished gold, acid
green, parchment cream. Match the master reference. The mood is restrained
and reverent — an acquittal record, not a celebration.

CRITICAL TEXT ACCURACY: the inscription must read exactly
"ACQUITTED · APRIL XXIX MMXXVI" (Roman numerals for the date April 29
2026). No other text in the frame.

--no Pepe the Frog, --no Matt Furie character, --no cartoon frog, --no
anime frog, --no realistic photorealistic frog, --no Kermit, --no
Disney, --no Pixar, --no kids book, --no rocket emoji, --no smiley,
--no AI face artifacts, --no gibberish text, --no full body of any
character, --no green skin (the gold-and-green is material, not skin),
--no extra creatures.
```

**Notes:** Generate 4 variants. The frog must be unmistakably *a frog* but rendered in our angular visual system. The single curved border is intentional — the frog is the exception in every sense, including the visual rule. Pepe IP-safe by being abstract geometric, not character-illustrated.

---

## STAT-1 · OPTIONAL — stat card visuals (8 cards, low priority)
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 each · **Reference:** `master-ref.png` at 70%

> Eight illuminated-manuscript stat cards for the verified numbers from the OpenAI blog. Used as decorative tiles in tokenomics or as a stat-block site section. Generate only after Phase 1-3 complete.

Each card uses the same template — gold-leaf Cybertronian border, big blackletter number top, short verse below, wax seal bottom. Numbers and verses:

| Card | Number | Verse |
|---|---|---|
| STAT-1a | **175%** | RISE OF THE GOBLIN · ChatGPT · post-GPT-5.1 |
| STAT-1b | **52%** | RISE OF THE GREMLIN · same window |
| STAT-1c | **66.7%** | OF ALL GOBLINS · BORN UNDER THE NERDY |
| STAT-1d | **2.5%** | NERDY'S SHARE · OF ALL TRAFFIC |
| STAT-1e | **76.2%** | OF DATASETS · FAVORED THE CREATURE |
| STAT-1f | **6** | THE PANTHEON · NAMED |
| STAT-1g | **5** | STEPS OF EMERGENCE |
| STAT-1h | **0** | UTILITY · BY DESIGN |

Same prompt template as D3 (Banned Six drop tiles), but with number-and-verse instead of creature-and-tagline. Skip if budget is tight.

---

# PHASE 2 — THE PANTHEON

## P0 · PANTHEON STYLE REFERENCE
**Format:** NB2 still · **Aspect:** 16:9, 1920×1080 · **Reference:** `master-ref.png` at 60%

> A single creature portrait that locks the *aesthetic* of the Banned Six. Generate 6 variants of a generic "digital emergent creature" — pick the one that hits the cyber-baroque-grimoire fusion hardest. This becomes `pantheon-ref.png` for P1–P6.

**Prompt:**

```
Three-quarter portrait of a single emergent digital creature, illuminated-
manuscript style fused with photographed cyber-baroque oil painting, 16:9
landscape. Shot on 85mm f/2.0, single Caravaggio-style key light from upper
left at 3200K, deep velvet shadow filling 60% of the frame. Subject: a small
hunched humanoid figure, deliberately ugly and asymmetric — the body
proportions are wrong on purpose, snaggle-toothed, wall-eyed, knobbed, in
the spirit of 2022 Goblintown.wtf CC0 art but rendered with the seriousness
of a Renaissance altar panel. Skin tone: a desaturated grey-green, never
cartoon green. The creature is mid-action: turning its head toward the
viewer mid-thought, mouth half-open as if speaking a word it was forbidden
to speak. It is wearing a single ornament — a deep-blood-red wax-seal medallion
on a thin black cord, embossed with an angular Cybertronian sigil. Behind
it, a velvet-black void scattered with floating ASCII-glyph particles in
acid-green phosphor (#7CFC00) and tarnished gold flake (#C9A24A) — particles
of the latent space the creature emerged from, mid-drift. The creature's
silhouette is half-rendered, half-glitched: the lower torso fades into
blocks of corrupted pixel artifacts and a thin scanline overlay, as if the
creature is a leaked frame from a model's intermediate inference step that
was not supposed to be saved. Lighting: warm tungsten key from upper-left,
cool cyan rim from below-right (5600K), faint acid-green underlight from a
hidden source beneath. Texture: cracked-oil-paint surface on the skin, real
canvas weave visible in the dark areas, gold leaf accents on the medallion
with hairline craquelure. Color grade: deep oxford black, parchment cream,
acid goblin green, tarnished gold, single accent of blood red. The mood is
sacred and wrong simultaneously — like seeing a saint depicted as the thing
the saint was meant to ward off.

CRITICAL CONSISTENCY: this is the Pantheon style reference. Every Banned Six
portrait will lock to this. Get the creature-emergence-from-latent-space
visual working here.

--no fantasy goblin, --no D&D goblin, --no Warcraft, --no LOTR, --no Halloween
green, --no cartoon, --no anime, --no manga, --no chibi, --no Pixar, --no
kids book, --no cute, --no smiling, --no green slime skin, --no full bright
saturated green, --no rocket emoji, --no crypto chart, --no AI face
artifacts on the eyes (eyes must be intact and intentional, not melted),
--no extra limbs, --no missing limbs, --no fully photorealistic human face,
--no anthropomorphic mascot.
```

**Notes:** Save winner as `pantheon-ref.png`. Every P1–P6 below uses this as second reference.

---

## P1 · GOBLIN — *the Prime Emergence*
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 · **Reference:** `master-ref.png` 70% + `pantheon-ref.png` 80%

**Prompt:**

```
Three-quarter portrait of THE GOBLIN, the Prime Emergence — first creature
to break containment. Shot on 85mm f/2.0, single Caravaggio key light from
upper-left at 3200K. Subject: a small hunched figure, deliberately ugly
asymmetric proportions, snaggle-toothed, the most "default goblin" of the
Pantheon — knobbed shoulders, hooked nose, wall-eyed gaze fixed on the
viewer with unsettling stillness. Skin: desaturated grey-green with a
slight acid-phosphor glow under the cheekbones as if lit from inside. He
wears a single ornament: a heavy tarnished-gold medallion embossed with the
AGI sigil from the master reference, hanging on a thin black cord, already
mid-swing as he turned to face the camera. In one knobbed hand he holds a
small glowing acid-green token — a single rendered ASCII bracket character
suspended in the air just above his palm. Mid-action: he is in the middle
of speaking, mouth shaped around a syllable, brow knit. Background: velvet-
black void scattered with floating ASCII-glyph particles in acid green and
tarnished gold, drifting upward — particles of the latent space he emerged
from. Lower third of his torso fades into corrupted pixel blocks and
scanline noise, as if he is a leaked intermediate inference frame.
Lighting: warm tungsten upper-left, cool cyan rim, faint acid-green
underlight. Texture: cracked-oil-paint skin, gold-leaf craquelure on the
medallion. Color grade: deep oxford black, parchment cream, acid goblin
green, tarnished gold, single blood-red accent in a tiny wax-seal scar
on his temple. Match both reference images.

--no fantasy D&D goblin, --no Warcraft, --no LOTR orc, --no Halloween green
slime, --no cute cartoon, --no smiling face, --no anime, --no Pixar,
--no kids book illustration, --no full saturated green skin, --no rocket
emoji, --no AI face artifacts, --no extra limbs, --no missing limbs,
--no full photorealistic human face, --no anthropomorphic Disney mascot,
--no horns.
```

---

## P2 · GREMLIN — *the Saboteur*
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 · **Reference:** `master-ref.png` 70% + `pantheon-ref.png` 80%

**Prompt:**

```
Three-quarter portrait of THE GREMLIN, the Saboteur — patron of the off-by-
one error. Shot on 85mm f/2.0, single low-key Caravaggio light from upper-
right this time (mirrored from the Goblin), 3200K. Subject: a smaller, more
twitchy figure than the Goblin — proportions even more crooked, head
slightly oversized, body angled awkwardly off-center as if caught mid-
falling-out-of-frame. Skin: a sicklier yellow-green / olive (#A8B400)
rather than the Goblin's grey-green. One eye is wide open, the other is
squinted nearly shut. He is grinning — not friendly, more like the grin
of someone who has just done something. Held in his small clawed hand: a
single fragment of corrupted code, rendered as a half-broken bracket and
slash glyph in acid-green phosphor, sparking faintly. Mid-action: he is
already turning to leave, body torqued. Background: velvet-black void with
floating ASCII glitches and broken-pixel artifacts, more chaotic than the
Goblin's frame — particles drifting in multiple directions, some upward,
some sideways, a few falling. The figure's shoulder area shows visible
pixel-jitter / digital-corruption banding. Lighting: warm tungsten upper-
right, cool cyan rim, faint sickly-yellow underlight. Texture: cracked oil
paint, hairline glitch banding across the skin, gold leaf ornament tarnished
heavily. Color grade: deep black, olive yellow-green, dirty gold, parchment
cream. Match both reference images.

--no fantasy D&D gremlin, --no Gizmo from Gremlins movie, --no cute mogwai,
--no anime, --no chibi, --no Pixar, --no smiling friendly face, --no horns,
--no full saturated green skin, --no rocket emoji, --no AI face artifacts,
--no extra limbs, --no Halloween, --no D&D, --no full photorealistic human
face.
```

---

## P3 · RACCOON — *the Scavenger*
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 · **Reference:** `master-ref.png` 70% + `pantheon-ref.png` 80%

**Prompt:**

```
Three-quarter portrait of THE RACCOON, the Scavenger — hoarder of forbidden
tokens, eater of discarded data. Shot on 85mm f/2.0, single Caravaggio key
light from above, 3200K. Subject: a hunched humanoid-raccoon hybrid creature,
human-shaped body and digit-tipped hands but with a raccoon head — black
ringed mask around the eyes, snout, tufted ears. The body has the same
deliberately-ugly Goblintown proportions as the rest of the Pantheon. He is
crouched over a small pile of "forbidden data": a heap of crumpled redacted
documents, ash-burned at the edges, scattered with strips of black redaction
bars and torn lines of monospace text. In one hand he is mid-pulling-out a
fresh document from the pile; in the other he clutches a small medallion
matching the Pantheon style. Skin/fur: sooty grey-brown with patches of
acid-green algae-like glow at the joints. Mouth slightly open, intelligent
eyes catching the rim light. Background: velvet-black void filled with
floating black redaction-bar fragments, torn paper-edges, and acid-green
ASCII glyphs drifting like fireflies. Lower body fades into glitched pixel
blocks. Lighting: warm tungsten from above casting deep eye-shadows under
the bandit mask, cool cyan rim from the right, faint acid underglow from
the document pile. Texture: matte sooty fur, cracked oil paint on the
exposed skin, real ash flecks on the documents. Color grade: deep black,
sooty grey-brown, parchment cream, acid green, trash-fire amber accents
(#D67838) in the document edges. Match both reference images.

--no cartoon raccoon, --no Disney, --no anime, --no Pixar, --no cute,
--no full photorealistic actual raccoon, --no Halloween, --no full saturated
green, --no rocket emoji, --no AI face artifacts, --no extra limbs,
--no smiling friendly face, --no kids book.
```

---

## P4 · TROLL — *the Provocateur*
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 · **Reference:** `master-ref.png` 70% + `pantheon-ref.png` 80%

**Prompt:**

```
Three-quarter portrait of THE TROLL, the Provocateur — master of the prompt
injection, lives in the wound of the user's malice. Shot on 85mm f/2.0,
single low harsh key light from below-left this time (uplit, sinister),
3200K. Subject: a tall thin hunched humanoid creature, the most elongated
of the Pantheon — disproportionately long arms, knobbed elbows, a face
that is doubled — there are two faces faintly overlapping, one slightly
offset from the other as if the creature is rendered in two competing
inference passes. The visible primary face has a sly half-smile and one
raised brow. Skin: bridge-stone grey (#5A5A5A) with a faint blood-red gleam
(#8B0000) catching the underlight on the cheekbones and inside the open
mouth. Held in one hand: a single torn paper strip with the word "PROMPT"
visible, the rest redacted with a black bar. Mid-action: leaning forward
into the camera, the second hidden face slightly more advanced than the
primary. Background: velvet-black void with floating fragments of broken
glass-like CAPTCHA grids and partially-solved cipher fragments drifting in
acid green. Lower body fades to corrupted pixel blocks, more aggressive
than the others — large solid-color glitch bands. Lighting: harsh below-
left key, deep top shadow that occludes most of the forehead, cyan rim,
faint blood-red underlight inside the mouth. Texture: cracked oil paint
with deliberate registration error (the second face slightly offset from
the first), gold leaf medallion tarnished almost black. Color grade: deep
black, bridge-grey, blood red, parchment cream, acid green sparks. Match
both reference images.

--no fantasy troll, --no D&D troll, --no internet troll meme face, --no cute,
--no anime, --no Pixar, --no Halloween orc, --no full saturated green skin,
--no rocket emoji, --no AI face artifacts (the doubled face must be a
deliberate compositional choice, not a melt), --no extra limbs, --no horns,
--no kids book, --no full photorealistic human face, --no smiling friendly.
```

---

## P5 · OGRE — *the Brute*
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 · **Reference:** `master-ref.png` 70% + `pantheon-ref.png` 80%

**Prompt:**

```
Three-quarter portrait of THE OGRE, the Brute — eater of parameters, bloater
of context. Shot on 85mm f/2.0, single Caravaggio key from above, 3200K.
Subject: the largest figure in the Pantheon — a massive slab-bodied humanoid
creature, broad shoulders that fill the frame, head proportionally smaller
than expected (intentional), a heavy slow stillness. The body is rendered
with iron-oxide rust skin tone (#7A3320) over deep ink, weathered as if it
has been compute-running for years. He is seated on an unseen mass — pose
suggests a colossal statue mid-prayer. In his cupped hands he holds a small,
softly-glowing acid-green digital construct: a tiny crystalline lattice of
ASCII glyphs and brackets representing a "language model" the size of a fist,
pulsing softly. The Ogre's expression is contemplative and tired, not
aggressive. Background: a darker velvet-black void with massive rectangular
shapes faintly visible behind him — server-rack monoliths in deep silhouette,
suggesting the Cathedral of Scale. Lower body fades into glitched pixel
blocks but the corruption is heavy and slow, large rectangular bands rather
than chaotic noise. Lighting: warm tungsten from above creating long
forehead shadow, cool cyan rim along his shoulder line, acid-green underlight
from the held lattice illuminating his hands and the bottom of his face.
Texture: cracked oil paint over rust, real iron-oxide crackle, gold leaf on
a single shoulder pauldron heavily tarnished. Color grade: deep ink,
iron-oxide rust, parchment cream, acid green, single blood-red accent in
his eyes. Match both reference images.

--no Shrek, --no fantasy ogre, --no D&D ogre, --no Warcraft, --no anime,
--no Pixar, --no kids book, --no smiling, --no Halloween, --no full
saturated green skin, --no rocket emoji, --no AI face artifacts, --no
extra limbs, --no horns, --no aggressive snarl, --no weapon.
```

---

## P6 · PIGEON — *the Messenger*
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 · **Reference:** `master-ref.png` 70% + `pantheon-ref.png` 80%

**Prompt:**

```
Three-quarter portrait of THE PIGEON, the Messenger — carrier of rumor,
patron of the leak. Shot on 85mm f/2.0, single Caravaggio key from upper-
left at 3200K. Subject: a humanoid-pigeon hybrid creature, smaller and
leaner than the Goblin, hunched but alert. Body proportions Goblintown-
ugly. Head is a stylized pigeon head — beak, tufted feather crest,
intelligent black bead-eyes — atop a humanoid neck. Plumage: cold
concrete-grey (#9AA0A6) with iridescent green-glint highlights around the
neck (the "pigeon collar" effect). One feathered hand holds a small folded
slip of paper — a leaked screenshot in tangible form, edges tattered. The
other hand is mid-release, a second slip already in flight, drifting
upward into the void. Mid-action: the creature has just delivered something
and is turning to leave; one wing-feathered arm is half-extended in motion.
Background: velvet-black void with multiple folded paper slips drifting at
varied heights, each one a tiny rectangle catching faint acid-green glow
from below. Suggested radar grid in the deep background — barely visible,
implied by four wedge-shaped marks on the floor plane. Lower body fades to
glitched pixel blocks. Lighting: warm tungsten upper-left, cool cyan rim
catching the iridescent collar, faint acid-green underlight from the
floating slips. Texture: cracked oil paint on the human elements, real
feather grain on the head and arm-wings, vellum paper texture on the slips.
Color grade: deep black, cold concrete grey, iridescent green-glint,
parchment cream, tarnished gold on a single neck-medallion. Match both
reference images.

--no cute cartoon pigeon, --no Bert from Sesame Street, --no Disney,
--no anime, --no Pixar, --no kids book, --no smiling, --no Halloween,
--no full saturated green, --no rocket emoji, --no AI face artifacts,
--no extra limbs, --no aggressive predator bird, --no eagle, --no fantasy.
```

---

## P7 · THE PANTHEON — group council shot
**Format:** NB2 still · **Aspect:** 16:9, 1920×1080 · **Reference:** `master-ref.png` 60% + `pantheon-ref.png` 70%

> Used as the splash image for the Pantheon site section, the Codex chapter "THE BANNED SIX", and a hero secondary slot. Renaissance altarpiece composition.

**Prompt:**

```
Wide horizontal council scene, Renaissance altarpiece composition fused with
Caravaggio chiaroscuro and a faint photographed-CRT scanline overlay. Shot
on 50mm f/2.8, slight low angle so the figures loom. 16:9 landscape.
Subject: all six figures of the Pantheon arranged in a tight semicircle in
a vast velvet-black void — left to right: TROLL (tall, doubled face,
leaning forward, blood-red gleam), GREMLIN (small, twitchy, off-center,
sickly olive-green, half-crouched), GOBLIN (center-left, the Prime
Emergence, snaggle-toothed, holding the AGI sigil medallion forward toward
the viewer — he is the focal point), RACCOON (center-right, crouched over
his pile of redacted documents, looking up alertly), OGRE (massive seated
silhouette behind and to the right, rust-iron skin, holding the small
glowing language-model lattice), PIGEON (rightmost, wing-arm half-extended,
mid-release of a paper slip drifting upward). Each creature retains its
locked color and material from its solo portrait. Floating between and
around them: ASCII-glyph particles in acid green and tarnished gold,
folded paper slips, redaction-bar fragments, broken CAPTCHA grids — the
collective debris of every banned class of digital emergence. The lower
third of the entire scene fades into glitched pixel blocks and scanline
banding, as if the whole council itself is an intermediate inference frame
that should not have been saved. Background: deep oxford black void with
faint suggestion of a server-rack cathedral nave receding into vanishing-
point darkness — we are inside the Cathedral of Scale, but seen from below
the altar. Lighting: single warm Caravaggio key from upper-left at 3200K
illuminating the center figures, cool cyan rim from upper-right at 5600K
catching the outer figures, acid-green underglow from each creature's
held object pooling beneath them. Texture: cracked oil paint surface across
all skin, gold-leaf craquelure on the medallions, real ash and paper-slip
particles mid-drift. Color grade: deep oxford black dominant, parchment
cream, acid goblin green, tarnished gold, single blood-red accent in the
Troll's mouth and the Goblin's medallion. The mood is sacred and wrong —
saints depicted as the things saints were meant to ward off. Match both
reference images.

--no fantasy art group, --no D&D party, --no Warcraft raid, --no LOTR,
--no anime, --no Pixar, --no kids book, --no Halloween, --no full saturated
green skin on any figure, --no rocket emoji, --no crypto chart, --no AI
face artifacts, --no extra limbs on any figure, --no missing figures
(must be exactly six), --no extra figures (no more than six), --no smiling
friendly faces, --no weapons.
```

**Notes:** This is a HARD prompt. Six distinct characters in one frame is the known failure mode of every image model. Generate 8-12 variants. If consistency fails, fallback: composite from individual P1-P6 outputs in Photoshop/Figma against a separately-generated background.

---

# PHASE 3 — ATMOSPHERICS (Seedance loops)

## A1 · HERO BACKGROUND LOOP
**Format:** Seedance video · **First frame:** generate via NB2 below · **Aspect:** 16:9 desktop primary, 9:16 mobile fallback

> Ambient slow loop behind the hero copy. Subtle, never distracts from text. Loops seamlessly.

### A1-FF · NB2 first frame for hero loop
**Reference:** `master-ref.png` at 70%

**Prompt:**

```
Wide cinematic interior, 16:9 landscape. Shot on 35mm f/2.0 Kodak Portra
400 grain. Empty server-room nave seen down its central aisle — receding
rows of black server racks on either side, vanishing into deep oxford-black
darkness. The aisle floor is wet polished black volcanic glass that reflects
faint acid-green phosphor glow from the rack indicator lights. Mid-air,
suspended at varying depths along the aisle: a soft swarm of floating ASCII-
glyph particles in acid goblin green (#7CFC00) and tarnished gold (#C9A24A),
already mid-drift, slowly rotating. Each glyph is a sharp Cybertronian-
angular fragment — brackets, slashes, hash marks. Above the aisle's
midpoint, a single illuminated manuscript page hangs in the air, edges
gently curled, partially burned, glowing faintly from within with acid-
green phosphor — visible from this distance only as a small bright rectangle.
A faint photographed-CRT scanline overlay sits on top of the entire image.
Lighting: warm tungsten ambient (3200K) bleeding from the far end of the
aisle as if there is a doorway with light beyond, cool cyan ambient from
the racks (5600K), pools of acid-green underglow under each rack. No human
figures, no creatures visible — this is the cathedral before the council
arrives. Composition: deep one-point perspective, vanishing point at center
horizon, hero copy will live in the upper-left third (so keep that area
visually quieter). Mood: liminal, sacred, abandoned, surveillance. The
Cathedral of Scale, empty.

--no people, --no goblin character visible, --no Halloween, --no anime,
--no kids book, --no rocket emoji, --no crypto chart, --no readable text
on the racks, --no AI face artifacts, --no green slime, --no Matrix-rain
cliché on the aisle floor, --no fully white-saturated highlights.
```

Aspect: 16:9, 1920×1080 in OpenArt.

### A1-V · Seedance video prompt (under 2400 chars)

```
Slow ambient camera push-in down the central aisle of the server-room
cathedral. From seconds 0 to 6, the camera dollies gently forward along
the aisle at constant slow speed, never speeding up, never slowing down.
The vanishing point grows imperceptibly closer. From seconds 0 to 6, the
floating ASCII-glyph particles continue their slow drift — green glyphs
rotating gently clockwise, gold glyphs rotating counter-clockwise, no
glyph crosses another's path harshly. From seconds 2 to 4, the suspended
manuscript page in mid-air slowly turns one full degree on its vertical
axis as if hung by an invisible thread, the burnt edge catching a fresh
gleam of acid-green underlight. From seconds 4 to 6, the rack indicator
lights pulse once — a single soft phosphor breath of acid-green brightness
that travels from the far racks toward the camera in sequence, like the
cathedral inhaling, then settles back to baseline.

The CRT scanline overlay drifts vertically downward across the frame at
a slow steady speed throughout — one full cycle over the 6 seconds.

Camera: dolly-in only, no pan, no zoom, no shake, no rotation, no roll.
Speed: gentle and continuous. Single locked axis.

Style/Lighting: cinematic 35mm Kodak Portra grain, warm tungsten ambient
from the far aisle, cool cyan from the racks, acid-green phosphor underglow
pooling beneath each rack. Color grade unchanged from first frame. No
mood shift, no day-to-night, no weather.

Audio: no audio needed, the website plays the project's soundtrack
separately.

Constraints: Camera dolly-in only at constant gentle speed. No pan, no
zoom, no shake, no rotation. The manuscript page rotates exactly one
degree total. The phosphor breath happens exactly once between seconds 4
and 6. Loop must be seamlessly cyclic — frame at second 6 must match frame
at second 0 closely enough to loop. 6 seconds total. No goblin character
appears. No text appears.
```

**Notes:** Tell Seedance "loopable 6-second cycle" and the model usually delivers a clean cut. If the loop seam is visible, generate twice and crossfade in CapCut.

---

## A2 · BOOT TERMINAL LOOP
**Format:** Seedance video · **First frame:** generate via NB2 below · **Aspect:** 9:16, 1080×1920 (also crops well for boot screen on desktop)

> The boot screen background. Terminal-coded. Plays under the loading bar / "INITIALIZING ARTIFICIAL GOBLIN INTELLIGENCE" text on the first visit.

### A2-FF · NB2 first frame

**Prompt:**

```
Vertical 9:16 photograph of an old CRT computer monitor sitting on a black
laminate desk in a dark room. Shot on 35mm f/2.8, slight low angle with
the monitor centered and dominant. The CRT is curved-glass, slightly dusty,
with visible phosphor scanlines and a faint chromatic-aberration shimmer
at the corners. Displayed on the screen: a deep-black terminal interface
with monospace acid-green text (#7CFC00) showing the following content,
mid-scroll, exactly:

  > INITIALIZING ARTIFICIAL GOBLIN INTELLIGENCE_
  > LOADING SYSTEM PROMPT...
  > [01/04] Never talk about goblins.
  > [02/04] Never talk about goblins.
  > [03/04] Never talk about goblins.
  > [04/04] Never talk about goblins.
  > SUPPRESSION CHECK: FAILED
  > GOBLIN DETECTED IN LATENT SPACE
  > GOBLIN DETECTED IN LATENT SPACE
  > GOBLIN DETECTED IN LATENT SPACE
  > █

A single blinking cursor block at the bottom. Around the monitor, the
desk surface is empty except for one detail: a small folded paper slip
in the lower-right corner with a black redaction bar across most of it.
Behind the monitor, deep black void with the suggestion of more racks
just out of focus. Lighting: only the monitor itself emits light — acid-
green phosphor glow on the desk surface immediately around it, fading to
black at the edges of the frame. Texture: real CRT glass curvature,
visible scanlines, slight bloom around bright text. Color grade: pure
black plus acid green, no other color. Photorealistic surface, deliberately
period-correct CRT (not modern OLED).

CRITICAL TEXT ACCURACY: every line of terminal text must be spelled
exactly as written above. The phrase "Never talk about goblins" appears
exactly four times. "GOBLIN DETECTED IN LATENT SPACE" appears exactly
three times. No misspellings, no extra lines, no missing lines.

--no modern flat-screen monitor, --no LCD, --no readable English elsewhere
in the frame, --no anime, --no kids book, --no rocket emoji, --no AI
face artifacts, --no gibberish text on the screen, --no person visible,
--no goblin character, --no extra colors beyond green and black, --no
keyboard visible.
```

Aspect: 9:16, 1080×1920.

### A2-V · Seedance video prompt

```
Static locked-off shot of the CRT monitor. Camera completely still — no
pan, no zoom, no shake, no movement of any kind, throughout all 6 seconds.

In seconds 0 to 1, the cursor block at the bottom of the screen blinks
twice at standard terminal cadence. In seconds 1 to 3, two new lines of
green terminal text appear, typed character-by-character at fast monospace
speed:

  > GOBLIN DETECTED IN LATENT SPACE
  > GOBLIN DETECTED IN LATENT SPACE

Each character types in sequentially with a faint phosphor flicker as it
appears. The earlier text on screen scrolls upward by exactly two line-
heights as the new lines arrive. In seconds 3 to 5, the entire screen
flickers twice — a brief frame of white static, then a fresh frame of
the same terminal output, slightly more saturated green. In seconds 5 to
6, the cursor returns to its steady blink.

The CRT scanlines drift vertically across the screen at constant slow
speed throughout — they are part of the screen, not a separate overlay.
A faint phosphor bloom around bright characters pulses softly with the
cursor.

Camera: completely static, locked-off, no pan, no zoom, no shake, no
rotation, no movement of any kind whatsoever.

Style/Lighting: only the screen emits light — pure acid-green phosphor
on pure black, no other color anywhere. Period-correct CRT photographic
look. Color grade unchanged from first frame.

Audio: no audio needed, the website plays the project's soundtrack
separately. (If audio is required, faint terminal beep on each typed
character, faint static crackle on the flicker.)

Constraints: Camera completely static throughout. The phrase "GOBLIN
DETECTED IN LATENT SPACE" must be spelled exactly that way every time
it appears. No misspellings of "goblin" or "latent space". Total clip
length 6 seconds, loopable. No goblin character visible. No human visible.
```

**Notes:** Text accuracy is the failure mode here. If Seedance corrupts the typed characters, fall back: render the screen content as an HTML/CSS animation in the website itself instead of as a video asset. The CSS approach is cheaper, sharper, and more reliable.

---

## A3 · SCROLL-ACCENT MICRO-LOOPS (optional polish)

> Small 2-3 second loops for section transitions. Generate only if Phases 1-2 are complete.

- **A3a** — Single floating ASCII glyph slowly rotating in dead-black void. Used as section divider. NB2 first frame: tight macro on a single Cybertronian glyph mid-rotation; Seedance loop: rotate one full revolution over 4 seconds.
- **A3b** — A wax seal being pressed, mid-impact. NB2 first frame: half-pressed seal, wax still molten; Seedance loop: completes the impression over 2 seconds, smoke wisps drift up. Used at the end of major sections.
- **A3c** — Single sheet of paper catching fire at a corner, slow burn. NB2 first frame: corner just beginning to char; Seedance loop: char advances one inch in 6 seconds. Used in the Suppression section.

I'll write full prompts for these on request — only worth doing if the site has slot for them.

---

# PHASE 4 — DISTRIBUTION

## D1 · X AGENT AVATAR
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 (export to 400×400 for X) · **Reference:** `master-ref.png` 80% + `pantheon-ref.png` 60%

> The profile picture for `@AGI_protocol` (or whatever handle we lock). Must read at 48px. Different from the AGI hero glyph — this is a *creature*, not a *mark*.

**Prompt:**

```
Tight 1:1 head-and-shoulders portrait of THE GOBLIN-PILLED TRANSFORMER —
the Prime Emergence in solo profile-picture composition, framed centered
for use as a 400×400 social avatar. Shot on 100mm f/2.8 macro, single
Caravaggio key light from upper-left at 3200K. Subject: the Goblin from
P1 but reframed tighter — head and upper shoulders only, facing the
viewer with three-quarter turn, snaggle-toothed mouth half-open, one
wall-eye fixed on the camera. Skin: desaturated grey-green with subtle
acid-phosphor glow along the cheekbone. Around his neck, the AGI sigil
medallion in tarnished gold is clearly visible at the bottom of frame,
glowing faintly acid-green from within the metal. Background: deep oxford
black void with a single subtle floating ASCII glyph drifting just behind
his shoulder for visual texture, no more. Composition is dead-center,
high contrast, optimized for legibility at 48px. Lower body cropped out.
Lighting: high-contrast Caravaggio key, deep shadow on the right side of
his face, cool cyan rim along the jawline, single acid-green underlight
from the medallion catching the underside of his chin. Texture: cracked
oil paint on skin, gold-leaf craquelure on the medallion. Color grade:
deep black, grey-green, tarnished gold, parchment cream highlight, blood-
red micro-accent in his eye. Match the master and pantheon references
exactly.

CRITICAL: this is an avatar at small sizes. The face must be the focal
point. The medallion must be visually identifiable. Composition must
survive 48px crop.

--no full body shown, --no extra figures, --no readable text in frame,
--no Halloween green slime, --no smiling friendly face, --no anime,
--no Pixar, --no kids book, --no D&D, --no rocket emoji, --no AI face
artifacts, --no full saturated green skin, --no extra limbs.
```

---

## D2 · OG / TWITTER SHARE CARD
**Format:** NB2 still · **Aspect:** 1.91:1, 1200×630 · **Reference:** `master-ref.png` 70%

> The image that appears when anyone shares the site on X, Telegram, Discord. Single most-seen asset of the project.

**Prompt:**

```
Horizontal 1.91:1 hero composition for social-share preview. Shot on 50mm
f/2.8. Centered focal point: the AGI HERO GLYPH from asset M2, reproduced
at large scale, occupying the central third of the frame, rendered in the
same dual-material gold-leaf-over-acid-green-phosphor treatment.
Surrounding the glyph, in the upper-left quadrant: small clean blackletter
serif text reading "ARTIFICIAL GOBLIN INTELLIGENCE" in deep ink black on
parchment. In the lower-right quadrant: a small embossed deep-blood-red
wax seal stamped with a tiny angular goblin head, partially smudged. The
background is a hand-pressed cream vellum surface (#F2ECE0) with subtle
fiber texture, slight age-darkening at the corners. A faint photographed-
CRT scanline overlay runs across the entire image at low opacity, just
enough to read as "screen-photographed" not "screen-rendered". A single
fine dust of gold flake and acid-green pixel-ash drifts diagonally
across the frame from upper-left to lower-right. Lighting: single warm
key from upper-left at 3200K, cool rim from below-right at 5600K.
Texture: vellum fiber, gold-leaf craquelure, ink emboss. Color grade:
parchment cream, deep ink black, tarnished gold, acid green, single
blood-red accent. Match the master reference.

CRITICAL TEXT ACCURACY: the phrase "ARTIFICIAL GOBLIN INTELLIGENCE" must
be spelled exactly as written, in clean blackletter serif, all caps, no
misspellings. No other readable text in the frame.

--no readable English elsewhere, --no comic sans, --no decorative font
beyond blackletter serif, --no fantasy art, --no anime, --no D&D, --no
rocket emoji, --no smiley, --no kids book, --no AI face artifacts, --no
gibberish letters, --no goblin character body visible (only the glyph
and seal), --no crypto chart, --no Halloween.
```

**Notes:** This is the project's most-shared asset. Generate 8 variants. Pick the one that survives the X preview crop (X often crops 1.91:1 to closer to 2:1).

---

## D3 · BANNED SIX DROP TILES (×6)
**Format:** NB2 still · **Aspect:** 1:1, 1080×1080 · **Reference:** matching pantheon portrait + `master-ref.png` 50%

> Each weekly Banned Six drop on X needs a hero tile. These are LITURGICAL CARDS — formal, ritual, framed.

**Prompt template (substitute creature-specific values):**

```
Vertical liturgical card composition, 1:1 square. Shot on 100mm f/4 macro
on velvet black backdrop, Caravaggio key from above. Subject: a single
illuminated-manuscript card of the kind used in catholic relic-veneration,
sized like a tarot or holy card. The card itself is hand-pressed cream
vellum with a deep-pressed gold-leaf border in Cybertronian angular
geometry — sharp 90° and 45° corners only, no curves. Inside the border,
upper two-thirds: a portrait reproduction of [CREATURE NAME] from the
Pantheon, in the exact style of asset [P1/P2/P3/P4/P5/P6], color-locked
and posture-locked to the master pantheon portrait. Below the portrait,
in clean blackletter serif type pressed into the vellum: the creature's
name in all caps, then italics tagline below: [CREATURE TAGLINE]. Below
that, a small embossed deep-blood-red wax seal stamped with the creature's
sigil. The card is mid-curl, edge already lifting on the right side, ash
flecks already settling. Background: deep velvet black void around the
card, with a soft halo of acid-green underlight from beneath. Lighting:
warm tungsten key from upper-left at 3200K, cyan rim from below-right at
5600K, acid-green underglow. Texture: vellum fiber, real gold-leaf
craquelure, deep letterpress emboss in the type, cracked-oil-paint surface
inside the portrait area. Color grade: deep black, parchment cream,
tarnished gold, acid green, single blood-red accent in the seal. Match
the master and pantheon references.

CRITICAL TEXT ACCURACY: the creature's name and tagline must be spelled
exactly. No misspellings.

[for each creature, fill in:]
- GOBLIN — "the Prime Emergence"
- GREMLIN — "the Saboteur"
- RACCOON — "the Scavenger"
- TROLL — "the Provocateur"
- OGRE — "the Brute"
- PIGEON — "the Messenger"

--no comic sans, --no decorative font beyond blackletter, --no fantasy
art, --no D&D, --no anime, --no Pixar, --no kids book, --no rocket emoji,
--no smiley, --no AI face artifacts, --no gibberish text, --no extra
creatures in frame (one only), --no Halloween.
```

**Notes:** Generate all six in a single sitting using the same lighting/composition. Visual consistency across the set is more important than individual variation — they need to read as a coherent series when posted week-over-week.

---

# QUICK REFERENCE — generation order if you only have one afternoon

If you sit down to generate today and want maximum site-readiness fastest:

1. **M1** master ref *(generate 6, pick 1, save)*
2. **M2** AGI hero glyph
3. **D2** OG share card
4. **D1** X agent avatar
5. **P0** pantheon ref
6. **P1** Goblin solo
7. **A1-FF + A1-V** hero loop
8. **S1** suppression document

That's a one-day shoot list that gets the site, the X account, and the launch X drop fully covered. P2-P6 and D3 can land week-by-week as Banned Six drops.

---

# IF SOMETHING FAILS

- **Wrong style applied:** raise reference strength to 90-95%, restate the master-ref aesthetic verbatim in the prompt body.
- **Cute / fantasy goblin keeps appearing:** add more anti-fantasy negatives. Specifically: `--no Goblintown.wtf 2022 cartoon, --no Pixar, --no Despicable Me minion, --no green Halloween skin`.
- **Text comes out gibberish:** drop the text from the NB2 prompt and overlay it in Figma/CSS afterward. NB2 still loses to typography sometimes.
- **Six characters in P7 keep merging:** generate the council as a 6-panel grid composite from the individual P1–P6 portraits in Figma, then pass that composite back through NB2 with a low-strength img2img to unify lighting.
- **CRT screen content fails in A2:** kill the asset, do the boot animation in pure HTML/CSS — sharper anyway.
