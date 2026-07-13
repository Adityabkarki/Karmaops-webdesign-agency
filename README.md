# Signature Web Design — an Agent Skill for landing pages that don't look AI-made

A Claude Agent Skill that replaces "generate me a landing page" with a real agency process: a **Jobs-to-be-Done discovery interview**, a **confirmed creative brief**, **2–3 divergent mockups you comment on before anything is built**, and a final **"tell detector" audit** that hunts down every known fingerprint of AI-generated design and copy.

## Why this exists

AI builders converge. Lovable converges on shadcn defaults. "Premium design" prompts converge on glass pills, bento grids, and OLED black. Both are templates — one plain, one fancy.

This skill contains almost **no aesthetic prescriptions**. Instead it enforces a *derivation chain*: every color, typeface, layout decision, and signature element must trace back to a concrete fact from the discovery interview:

```
FACT (from discovery) → ASSOCIATION (from the subject's world) → DECISION (specific value)
```

A page for a 2am incident-response tool and a page for a specialty coffee roaster *cannot* look alike, because they are derived from different worlds. That is the only mechanism that produces unrepeatable output.

## The process contract

```
DISCOVER → BRIEF (you confirm) → DIVERGE (mockups, you comment) → BUILD → AUDIT
```

1. **Discover** — a JTBD interview: the visitor's struggling moment, the functional/emotional/social job the page over-serves, the four forces (push, pull, anxiety, habit), the one precise action, a proof inventory, and "world notes."
2. **Brief** — a one-screen creative brief. Nothing proceeds until you confirm it.
3. **Diverge** — three directions derived from the brief, each a different argument about the job. Any direction that could plausibly be produced for a different client is killed and re-derived. You get 2–3 working HTML mockups and are asked what to keep, mix, and reject.
4. **Build** — production code faithful to the approved mockup, with a hard quality floor (360px responsive, keyboard focus, reduced motion, verified contrast) and strict copy rules. No invented statistics or fake testimonials, ever — gaps are marked `[NEEDS REAL DATA]`.
5. **Audit** — a 12-point tell detector: the swap test, the provenance test, a cliché registry scan, a banned-vocabulary scan ("unlock," "elevate," "seamless," rule-of-three triads...), and a self-history scan so the skill can't fall into its own ruts.

## Install

**Claude.ai / Claude Desktop:** download [`releases/signature-web-design-v1.0.0.skill`](releases/signature-web-design-v1.0.0.skill), attach it in a chat, and click **Save skill**. Or add the folder under Settings → Capabilities → Skills where available.

**Claude Code:** copy the folder into your skills directory:

```bash
git clone https://github.com/YOUR_USERNAME/signature-web-design-skill.git
cp -r signature-web-design-skill/signature-web-design ~/.claude/skills/
```

Then just ask Claude to design a landing page — the skill triggers automatically.

## Repo layout

```
signature-web-design/
├── SKILL.md                  # The process contract (phases, gates, failure modes)
└── references/
    ├── discovery.md          # Full JTBD interview script + synthesis method
    ├── derivation.md         # The anti-template engine + cliché registry
    └── craft.md              # Build standards, copy voice rules, tell-detector audit
releases/                     # Packaged .skill files for one-click install
```

## Philosophy in one line

Style is never *selected* — it is *derived*. If a design decision can't answer "why this, for this client?" in one sentence, it doesn't ship.

## License

MIT — see [LICENSE](LICENSE).
