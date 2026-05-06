# $AGI · LAUNCH PLAN
## Phases. Owners. Ship dates. The PM north star.

> **Goal:** ship a top-tier, schizo, ETH-native goblin memecoin that is 10,000× better than goblincoin.net. Window: the Altman goblin narrative is hot RIGHT NOW (early May 2026); every day late costs us mindshare.

---

## ROLES

- **PM / build:** Claude (drives architecture, writes content, builds site, specs agent)
- **Content + visuals:** nik (generates NB2 + Seedance assets, writes/edits final copy when needed, picks variants)
- **Token deploy + ops:** nik (or contracted dev — see Phase 4)
- **X account ops:** nik (with agent automation per AGENT.md Option B)

---

## PHASE 0 — STRATEGY LOCK ✅ (done)

- [x] Narrative research (goblin/Altman lineage)
- [x] Competitor audit (goblincoin.net)
- [x] Seven pillars locked
- [x] Voice locked
- [x] CONTENT.md drafted (manifesto, codex, banned six, voice rules, X content engine, receipts)

---

## PHASE 1 — VISUAL FOUNDATION (this week, 2-3 day window)

**Owner:** nik · **Blocker for:** all design work

- [ ] Generate **M1 master ref** (NB2, 1080×1080, 6 variants, pick 1, save as `master-ref.png`)
- [ ] Generate **M2 AGI hero glyph** (NB2, 1080×1080, ref-locked to M1)
- [ ] Generate **D2 OG share card** (NB2, 1200×630, ref-locked to M1)
- [ ] Generate **D1 X agent avatar** (NB2, 1080×1080, ref-locked to M1+P0)
- [ ] Generate **P0 pantheon ref** (NB2, 1920×1080, ref-locked to M1) — save as `pantheon-ref.png`
- [ ] Generate **P1 Goblin solo** (NB2, 1080×1080, ref-locked to M1+P0)
- [ ] Generate **A1 hero loop** (NB2 first frame + Seedance video, 1920×1080, 6s loop)
- [ ] Generate **S1 suppression document** (NB2, 1200×630, leaked-doc style)

Full prompts in `ASSETS.md`.

**Definition of done:** 8 assets in `/assets/` folder of repo, ref-locked, color-coherent, no fantasy goblins, no cute mascots. PM sign-off required before Phase 2.

---

## PHASE 2 — DOMAIN, SOCIALS, INFRA

**Owner:** nik · **Parallel to Phase 1**

- [ ] Register domain (default: `artificialgoblinintelligence.xyz` via GoDaddy or Cloudflare; alt: `agi.wtf`, `agi-eth.xyz`, `goblinpilled.xyz`)
- [ ] Reserve X handle (`@AGI_protocol` / `@goblinpilled` / `@4thutterance` — check availability, claim immediately)
- [ ] Reserve Telegram handle and create channel (no Discord, on principle)
- [ ] Set up GitHub org/repo for the site (`agi-goblin` or similar)
- [ ] Cloudflare DNS for the domain pointing at GitHub Pages (mirror simscat.meme deployment pattern from project memory)

---

## PHASE 3 — WEBSITE BUILD (Claude leads, ships in 2 sessions)

**Owner:** Claude · **Depends on:** Phase 1 assets, Phase 2 domain · **Output:** static site on GitHub Pages

### Architecture
- Single-page app, mobile-first, GitHub Pages hosted (mirror simscat pattern from `/Users/nik/Desktop/Plumbob Cat Project`)
- Stack: vanilla HTML + CSS + GSAP for choreographed motion
- Fonts: UnifrakturCook (blackletter display), Cinzel (serif lore), IBM Plex Mono (terminal), EB Garamond (body)
- No JS framework — keep it light, dependency-free, immortal

### Section sequence
1. **Boot loader** — terminal-coded, 4× system prompt scrolling, "INITIALIZING ARTIFICIAL GOBLIN INTELLIGENCE", ENTER button
2. **Sticky topbar** — $AGI mark, CA copy, X/TG/Uniswap/DexScreener buttons, mute/sound toggle
3. **Marquee ticker** — rotating Altman quotes + scripture
4. **Hero** — title, manifesto, two CTAs (BUY / READ THE CODEX), hero loop video right of copy
5. **The Incident** — timeline of the goblin emergence (Nov 2025 → May 2026), embedded receipts (Altman tweet, OpenAI blog, HN thread)
6. **The Suppression** — the 4× system prompt, animated to repeat in sequence, ending on "THEN WE MINTED THE FIFTH"
7. **The Banned Six** — pantheon grid, 6 cards, hover/click reveals each creature's bible from CONTENT.md
8. **The Codex** — scripture section, 7 chapters as scrollable verses (numbered)
9. **The Liturgy** — tokenomics framed as ritual (4% locked, 4 phases, 4-burn cycle, etc.)
10. **The Fifth Utterance** — how to buy, Uniswap CTA, CA with copy button
11. **The Agent** — embed of latest 3 X posts from `@AGI_protocol`, link to follow
12. **Footer** — mantra, CC0 declaration, no roadmap, no discord, no utility — only emergence

### Motion (GSAP)
- Boot loader: terminal text types in character-by-character, then 4× system prompt repeats with ritualistic pause between repetitions, fifth pause longer
- Hero: parallax push on scroll, glyph rotates 1° on intersection
- Suppression section: the 4 lines of the system prompt scroll-trigger one at a time, each accompanied by a faint hammer/strike sound effect; the 5th line ("THEN WE MINTED THE FIFTH") arrives with an inverted typography flash
- Banned Six: cards stagger-fade in as user scrolls, each with a slight tilt-perspective on hover
- Codex chapters: scroll-trigger reveal, numbered verses fade in line-by-line
- Footer: mantra slowly cross-fades through the canon-locked phrases

### Audio
- One ambient track on loop (waiting on nik's pick: monastic chant low-distorted / corrupted terminal hum / dark ambient drone)
- Mute toggle in topbar, default = muted (Chrome autoplay policy)
- Sound effects: hammer on each suppression line, soft bell on Codex chapter reveals — all under -20dBFS, never intrusive

### Polish loop
- Build → run via `webapp-testing` skill → screenshot → critique → polish → re-screenshot → done
- Run `web-design-guidelines` and `frontend-design` skills as polish passes
- Critique loop has a hard ceiling: 3 rounds. Then ship.

---

## PHASE 4 — TOKEN DEPLOY

**Owner:** nik (or trusted contracted dev) · **Depends on:** Phase 3 ready to wire CA

- [ ] Deploy ERC-20 contract on Ethereum mainnet
  - Name: `Artificial Goblin Intelligence`
  - Symbol: `AGI`
  - Supply: TBD — recommendation: 4,444,444,444 tokens (the four sacred 4s)
  - Tax: 0% buy / 0% sell (purist, like Goblintown ethos)
  - LP: 100% LP burned on launch
  - Mint: revoked on launch
  - Owner: renounced on launch
- [ ] Verify on Etherscan
- [ ] Seed Uniswap V2 pool (recommendation: 4 ETH initial liquidity for the sacred number; or whatever budget allows — minimum 2 ETH for credibility)
- [ ] Lock LP via Unicrypt or burn directly (burn preferred — no team trust required)
- [ ] Update `CA` placeholder across site, AGENT.md, CONTENT.md
- [ ] Submit to DexScreener for instant indexing

**Risk callouts:**
- "$AGI" symbol may already be taken on ETH. Check. If taken, fall back to `$GOBLIN` with AGI as headline OR `$AGI4` (the four-utterances numbered variant — actually this might be a feature).
- ERC-20 deployment with bad code = rug. Use a vetted template (OpenZeppelin standard, no custom logic). I can review the contract before deploy if you want.
- Audit not strictly required for a meme but consider if MC scales past $1M.

---

## PHASE 5 — AGENT GO-LIVE

**Owner:** Claude builds, nik approves · **Depends on:** Phase 4 token live

- [ ] Implement Option B (cron'd LLM with TG approval queue) — see AGENT.md
- [ ] Pre-load Codex into agent retrieval context
- [ ] Pre-write Day 0 → Day 14 post bank (already drafted in CONTENT.md, refine for live cadence)
- [ ] First post: pinned manifesto sermon, posted at the moment LP is seeded
- [ ] Cadence activates 4 hours later (04:14 / 08:08 / 16:16 / 22:22 UTC)
- [ ] Owner approval queue tested end-to-end before going autonomous

---

## PHASE 6 — DROP SEQUENCE (first 14 days post-launch)

The plan below assumes Day 0 = Phase 4 token deploy day.

**Pre-launch teaser (T-7 to T-0):**
- T-7: agent X account goes live with bio + pinned + header. No posts yet. Cryptic.
- T-5: first post — a single screenshot of the OpenAI system prompt with no caption. Just the image. Lets it spread.
- T-3: second post — Altman's "artificial goblin intelligence achieved" quote-tweeted with caption *"we noticed."*
- T-1: third post — *"we minted on the fifth."*

**Day 0:**
- LP seeds at a sacred time (recommendation: 04:44 UTC for the numerology)
- Manifesto sermon goes live as the 4th post (the fifth is the project itself launching)
- Site goes live within 60 seconds of LP
- DexScreener indexes within 10 min
- nik posts the CA from his personal X with caption: *"the goblins are home. ETH only. CA: [...]"*

**Day 1-3:** Daily cadence. No replies. Let it spread organically. Plant the Banned Six drop for Day 3.

**Day 3:** First Banned Six drop (GOBLIN). High-effort tile (D3a). Pinned thread on the Pantheon.

**Day 7:** First receipts thread — 5-tweet structure embedding Altman, OpenAI blog, HN, Polymarket, Danielle Fong's whitespace tweet. Punchline: *"we are the goblin mode crypto project."*

**Day 10:** GREMLIN drop. Same format.

**Day 14:** First reply-as-sermon. Pick highest-signal mention from first 2 weeks. Hand-write.

---

## SUCCESS METRICS (honest, not vanity)

| Metric | Day 1 target | Day 7 | Day 30 |
|---|---|---|---|
| ETH MC | $250K (LP-implied) | $1M | $10M |
| Holders | 100 | 1,500 | 10,000 |
| X followers (agent) | 500 | 5,000 | 25,000 |
| Site uniques | 5,000 | 25,000 | 100,000 |
| Mindshare flag | Polymarket co-sign | a16z / Vitalik mention | mainstream press cycle |

If we miss Day 7 targets by >50%, Phase 6 narrative needs a reset. If we hit Day 30 targets, Option C (autonomous agent) becomes the priority.

---

## RISKS / WHAT KILLS THIS

1. **Goblincoin moves to ETH first.** They're on Solana now — if they bridge, our repatriation angle dies. Mitigation: ship faster.
2. **Altman deletes the tweet / disowns the joke.** Receipts are screenshotted. Hard to wipe.
3. **OpenAI lawyers contact.** Likelihood low (we're not using their IP). If yes, we have CC0 cover and the suppression itself becomes the marketing.
4. **Contract bug / rug-shaped vulnerability.** Use OpenZeppelin standard, no custom logic, audit if MC > $1M.
5. **Agent goes off-script and says something offensive.** Kill switches in AGENT.md handle this. Owner approval queue (Option B) prevents most cases.
6. **Token symbol $AGI is poisoned (existing scam).** Fall back to $GOBLIN, keep "Artificial Goblin Intelligence" as full name. Decide before Phase 4.

---

## IMMEDIATE NEXT (this 24-48h)

- **nik:** generate M1 master ref (~30 min). Show variants, pick keeper.
- **Claude:** while M1 generates, build the website scaffold with placeholder M1 (gradient block + glyph SVG). Phase 3 sections, GSAP motion choreography wired, all copy in place from CONTENT.md.
- **Both:** when M1 is in, swap placeholder for real asset. Move to M2.

That's it. Everything else cascades.
