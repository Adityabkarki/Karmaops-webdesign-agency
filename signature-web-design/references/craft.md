# Craft: build standards, copy, motion, and the tell detector

## Build standards

**Fidelity to the chosen direction.** The final page must be recognizably the mockup, matured. Users experience silent drift between approved mockup and final build as betrayal. If building reveals the direction needs a change, say so and show the change — don't smuggle it.

**Code shape.** Single-file HTML/CSS/JS by default (deploy-anywhere, inspect-everything); React/framework only if the user's stack requires it. Semantic HTML (`header/main/section/footer`, one `h1`, real landmarks). CSS custom properties for every derived token, named after their derivation (`--ink`, `--ground`, `--accent-action`) so the system is legible. Comment the derivation chain at the top of the stylesheet — the file should teach its own logic.

**Quality floor (never announced, never skipped):**
- Responsive to 360px; test the hero, nav, and forms at that width. No horizontal scroll ever.
- Use `min-height: 100dvh`, not `100vh`, for full-height sections (iOS Safari).
- Visible `:focus-visible` styles on all interactive elements; logical tab order.
- `prefers-reduced-motion: reduce` disables all non-essential animation.
- Contrast: 4.5:1 body text, 3:1 large text — verify, don't eyeball.
- Animate only `transform` and `opacity`; use `IntersectionObserver` for scroll reveals, never scroll listeners; `backdrop-filter` only on fixed/sticky elements.
- Real `<title>` + meta description written from the job statement; alt text that describes the job of the image; lazy-load below-fold imagery.
- Forms: labels (not placeholder-as-label), inline validation, an honest success state.

**Imagery.** No stock-photo energy. Prefer: the actual product, real screenshots, derived illustration/diagram systems, CSS/SVG-built texture from the world-notes, or well-set type as the visual. If a real photo is genuinely needed and unavailable, build a clearly-marked placeholder frame with an art-direction note (`<!-- PHOTO: hands repairing espresso machine, overhead, warm side light -->`) so the user knows exactly what to shoot.

## Copy: the strongest anti-AI signal

Copy exposes machine authorship faster than any visual. Rules:

**Write from the discovery transcript.** The visitor's verbs, the user's phrasing of the pain, the anxieties verbatim. A headline that quotes the struggling moment ("Still building client reports on Sunday night?") outperforms any benefit-statement formula — and no generator can produce it without the interview.

**Banned vocabulary and cadences** (each is a statistical AI fingerprint):
- Words: unlock, elevate, empower, seamless(ly), effortless(ly), supercharge, revolutionize, game-changing, cutting-edge, "in today's fast-paced world," harness, streamline (as a headline verb), delve.
- Cadences: rule-of-three sentence triads in every paragraph; "It's not just X. It's Y."; em-dash pivot in every other line; every section header as a gerund phrase ("Empowering teams. Driving results.").
- Structures: "Why choose us" as a literal header; features written as "✓ Feature — benefit restated."

**Positive rules:**
- One idea per sentence. Specific beats clever. Concrete nouns from the world-notes over category abstractions.
- CTAs name the actual next thing that happens: "Book the 20-minute teardown," not "Get started." Same verb persists through the whole flow (button → confirmation).
- Handle the top anxiety in plain speech near the CTA ("No card. Delete everything with one click.") — reassurance in the visitor's language, not legal-adjacent hedging.
- Every unverifiable claim gets `[NEEDS REAL DATA: description]` in an HTML comment plus a note to the user. Never ship invented numbers, logos, or named testimonials.
- Microcopy (empty states, errors, form hints) is written, not defaulted. It's where human care is most visible.

## Motion

Motion is punctuation for the page's argument. Decide where the argument needs emphasis, then choreograph *that* — usually one orchestrated moment (a hero settle-in, a signature-element interaction, or one meaningful scroll reveal) with everything else static or nearly so. Scattered fade-ups on every section is a generator signature. Zero motion is a legitimate, sometimes superior choice — especially for functional-dominant briefs where speed-to-comprehension is the job. Timing: fast for feedback (~150–250ms), slower only for narrative moments; custom easing where motion is featured; never animate layout properties.

## The tell detector (final audit — run before every delivery)

Work through all of these against the finished page. Fix, don't rationalize.

**Specificity tests**
1. Swap test: move the hero (headline + palette + imagery) onto the nearest competitor's site. Works fine there? → not specific enough; rewrite from the struggling moment.
2. Provenance test: pick 5 random design decisions; state each one's derivation chain in one sentence. Any answer resembling "it looks premium/clean/modern" → change the element.
3. Job test: read the page top to bottom as the visitor from discovery. Does each section either amplify push/pull or disarm an anxiety? Sections doing neither get cut or merged.

**Machine-fingerprint tests**
4. Cliché registry scan (derivation.md §registry): ≥2 matches with any single cliché → redesign that region.
5. Vocabulary scan: search the copy for every banned word/cadence above.
6. Symmetry scan: three identical cards, four identical steps, perfectly interchangeable sections → introduce hierarchy that reflects real importance (something IS more important; show it).
7. Emoji-as-icon scan; gradient-text scan; badge-pill-above-H1 scan.
8. Self-history scan: does this share palette family, type pairing, or hero structure with your recent outputs? → contamination; re-derive the shared axis.

**Craft tests**
9. 360px walkthrough: hero legible, nav usable, CTA reachable, no overflow.
10. Keyboard-only walkthrough: can you reach and fire the one action?
11. Reduced-motion check; contrast check; focus-visible check.
12. Read every string of microcopy aloud. Anything you wouldn't say to a client's face gets rewritten.

**Delivery ritual**
Present the file(s). Then, like an agency: (a) name 1–2 things you'd refine in round two, (b) list every `[NEEDS REAL DATA]` item as the client's homework, (c) ask for their punch list. One revision offer, not a loop of "would you like me to…".
