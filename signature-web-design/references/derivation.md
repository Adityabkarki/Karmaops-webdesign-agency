# Derivation: designing from the world, not from a style menu

Every AI design tool converges because it *selects* aesthetics from a learned menu (shadcn defaults, "premium glassmorphism," "editorial luxury"). The only durable escape is **derivation**: every visual decision traces to a concrete fact from discovery. This file is the method.

## The derivation chain

For each of the four design axes, start from world-notes and job facts, and write the chain down (privately) before designing:

```
FACT (from discovery) → ASSOCIATION (from the subject's world) → DECISION (specific value)
```

Example, a nighttime pharmacy delivery service:
- FACT: struggling moment is "sick kid, 11pm, nothing's open" → ASSOCIATION: streetlight sodium glow against dark, the relief of one lit window → DECISION: near-black blue-grey ground, one warm amber accent used *only* on the action path; nothing else on the page gets warmth.

If you cannot write the chain for a decision, you're selecting from the menu. Stop and derive.

### Axis 1 — Palette

Never pick colors by mood-word ("premium," "calm," "bold"). Sources, in preference order:
1. **The subject's materials.** Roasted coffee: chaff, crema, kraft, char. Marine software: chart paper, buoy red, depth-sounder green.
2. **The struggling moment's light.** What time of day, what environment is the visitor in? A 2am incident tool can own darkness honestly; a Sunday-morning meal planner can't.
3. **The user's existing brand**, if declared sacred — then derive the *supporting* palette from world materials so the brand color stops floating in a void.

Practical rules: 1 ground, 1–2 ink tones, 1 accent with a *reserved meaning* (the accent appears only on job-completing elements — this makes pages feel authored, because meaning-reserved color is something templates never do). Test contrast (4.5:1 body, 3:1 large text).

### Axis 2 — Typography

Type is the voice of the page. Derive from the **register of the world's insiders**, not from a "premium fonts" list:
- What do the subject's own artifacts look like? Legal world → book-face traditions; hardware world → engineering drawings and DIN-flavored sans; food world → menu and signage traditions; dev world → the terminal, but *earned*, not costume.
- Pick a display face with an opinion and a body face that disappears; set them with intention (real type scale, tightened display tracking, generous body leading). The pairing must be justifiable in one sentence from the world-notes.
- **Availability note:** use Google Fonts or system stacks — distinctiveness comes from pairing, scale, and setting, not from paywalled foundry files. If a direction truly needs a commercial face, name it and provide the closest free stand-in with a comment.
- **Anti-tell:** if your last several projects used the same face, it's contaminated for this one regardless of fit.

### Axis 3 — Spatial logic

Don't choose a "layout archetype." Choose a **reading argument**: in what order must the visitor encounter push → pull → proof → disarmed anxiety → action? Then find the spatial form that enforces that order.
- Functional-dominant briefs usually want compression: product visible in the first viewport, short distance to action, information-dense proof.
- Emotional-dominant briefs usually want pacing: a slower open, more whitespace as tension control, proof as testimony rather than statistics.
- Social-dominant briefs usually want a mirror: identity imagery and "people like you" signals above feature detail.
Asymmetry, density, and rhythm should *encode* something (importance, sequence, hierarchy of anxiety), never decorate. A grid may be perfectly symmetric if the argument is "we are exact and reliable."

### Axis 4 — The signature element

One element the page will be remembered by, derived from the world, executed excellently. It can be: an interactive demo of the actual job, a data visualization of the visitor's pain, a typographic device, an illustration system, a scroll-driven narrative moment, a form that behaves unusually well. Constraints:
- It must **advance the job** (usually amplifying pull or disarming the top anxiety), not just impress.
- There is exactly one. Two signatures cancel each other.
- Everything around it goes quiet: the discipline is what makes the signature read as intentional.

## Building the three directions

Each direction = a different **argument**, expressed through different derivations:
- Direction A might over-serve the functional dimension (compression argument), B the emotional (pacing argument), C an unexpected reframe (e.g., lead with the anxiety and disarm it in the hero).
- Directions must differ on ≥2 axes. Different accent on the same layout is one direction in three costumes — that's a Lovable move.
- Name each direction with a phrase from the discovery language, not a style label: "The Lit Window," not "Dark Premium."

## Mockup mechanics

- One self-contained HTML file per direction: hero + one representative section. Real derived copy — never lorem ipsum, never `[Your headline here]`. The copy IS part of the concept.
- 80% fidelity, built fast. Note inside an HTML comment: the derivation chains for palette/type/signature, so the final build can honor them.
- Include the mobile behavior at least for the hero (test at 360px width mentally or via resize).
- Present with honest rationale + one trade-off each. Ask for comments and cross-pollination, not just a winner.

## The cliché registry (allowed only if the brief asks)

These are the current recognizable machine-outputs. They are *tells*, not sins — legitimate when the brief demands them, contaminated as defaults:

1. Warm cream ground + high-contrast serif display + terracotta/clay accent.
2. Near-black ground + single acid-green or vermilion accent + monospace labels.
3. Glassmorphism cards, floating pill nav, bento grid, mesh-gradient orbs ("Linear/Apple-tier").
4. Broadsheet: hairline rules, zero radius, newspaper columns, oversized folio numbers.
5. Purple→blue gradient anywhere; gradient text on the H1.
6. Three symmetric feature cards, icon-title-two-line-blurb.
7. Center-aligned everything with a badge pill above the H1 reading "✨ Announcing...".
8. Emoji as icons in feature sections.

Before presenting directions, check each against this registry and against your own recent work. Matching ≥2 items from one cliché = redo the derivation for that direction.
