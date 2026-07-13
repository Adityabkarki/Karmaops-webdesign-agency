# Discovery: the Jobs-to-be-Done interview

The goal of discovery is not requirements. It's **causality**: what causes a visitor to arrive, hesitate, and act. Design decisions made without this causality are decoration; with it, they're arguments.

## Posture

Interview like a design director on a kickoff call, not a form. React to answers, pull threads, play back what you heard. If the user gives a rich opening message, extract answers from it first and only ask what's missing — nothing signals "automated process" faster than asking a question the user already answered.

Two rounds of questions maximum. First round: the job core. Second round (optional): world, taste, and proof. Then synthesize.

## Round 1 — The job core

Ask these as conversation, adapting phrasing to the user's register:

**1. The struggling moment (open-ended, most important question)**
"Walk me through the moment someone ends up on this page. What just happened in their day? What did they already try that didn't work?"
- Listen for: the trigger event, the failed alternatives (competitors, spreadsheets, doing nothing), the emotional temperature (frustrated? anxious? curious? embarrassed?).
- The failed alternatives are gold: the page must implicitly answer "why this instead of what I already tried."

**2. The three dimensions (can be structured/multiple-choice)**
Every job has functional, emotional, and social dimensions, and every great landing page *over-serves one*:
- **Functional:** "When they leave the page having succeeded, what task is done or started?"
- **Emotional:** "How do they want to feel — relieved? in control? excited? safe? smart?"
- **Social:** "Who sees their choice? Boss, clients, peers, followers? How do they want to look to them?"
Then ask which dimension matters most. A B2B security tool over-serves emotional (safety/relief) even though it sells functionally. A portfolio over-serves social. A tax tool over-serves functional. This single answer drives more design decisions than any aesthetic preference.

**3. The four forces**
- **Push:** "What's most painful about how they do it today?" (fuel for the headline)
- **Pull:** "What's the one outcome that would make them switch tomorrow?" (fuel for the hero subline and proof)
- **Anxiety:** "What makes a perfect-fit visitor hesitate or close the tab?" — price shock, setup effort, trust, lock-in, looking foolish. (fuel for the objection-handling sections; most template pages skip this entirely, which is why they don't convert)
- **Habit:** "What's comfortable about their current way, even if it's bad?" (tells you what NOT to attack head-on)

**4. The one action**
"If a visitor does exactly one thing on this page, what is it — precisely?" Push past "sign up": free trial vs. demo call vs. waitlist vs. purchase are different pages. Also get the *commitment level* the visitor feels: is the ask cheap (email) or scary (sales call)? Scary asks need more disarming before the CTA.

## Round 2 — World, taste, proof

**5. Proof inventory**
"What real material exists right now? Numbers you can stand behind, customer names/quotes, screenshots, press, your own story?" List what's real. Where proof is thin, plan structure that works without it (a founder's letter beats fake logos).

**6. The subject's world (open-ended — this feeds the derivation engine)**
"Tell me about the physical and cultural world of this product/business. What are its materials, tools, places, era, rituals? What words do insiders use that outsiders don't?"
- A specialty coffee roaster's world: kraft paper, roast curves, burlap, 6am, degassing valves, cupping spoons.
- A devtools startup's world: terminals, diffs, monospace, incident channels, 2am pages.
- These concrete nouns become palette sources, texture logic, and copy vocabulary in Phase 3.

**7. Taste calibration**
"Name one or two sites or brands you admire — and, more importantly, *why*." The named references are weak data (users often name famous sites); the why is strong data ("I like how calm Linear feels" → they want low visual noise, not Linear's aesthetic). Also ask the inverse: "Anything you've seen for your space that made you cringe?"

**8. Constraints (quick-fire)**
Existing brand assets (logo, colors — sacred or negotiable?), tech constraints (stack, CMS, framework), timeline, and pages in scope beyond the landing page.

## The compressed 5-question version

For users who signal speed ("just need something quick"):
1. Who lands here and what just went wrong in their day?
2. What's the ONE thing they should do on this page?
3. What would make them hesitate?
4. What real proof do you have?
5. Describe your product's world in five concrete nouns.

Still enough to derive a real design. Never go below these five.

## Synthesis method

Turn answers into the brief (Phase 2 format in SKILL.md). Rules:

- **Write the job statement in the visitor's voice**, not marketing voice: "When my agency's client reports take all Sunday, help me generate them automatically so I can stop dreading month-end." Not: "An AI-powered reporting platform."
- **Rank anxieties.** The top anxiety earns a whole page section; the rest earn a line each near the CTA.
- **Convert the over-served dimension into design implications** and state them in the brief:
  - Functional-dominant → clarity architecture: show the product early, dense information honesty, fast path to action, minimal ceremony.
  - Emotional-dominant → pacing architecture: atmosphere before information, slower reveal, testimony and story carry weight, CTA arrives after safety is established.
  - Social-dominant → mirror architecture: the visitor's identity and taste reflected back; who else uses it matters more than what it does.
- **Flag contradictions openly.** If the user wants "premium and exclusive" but the action is "download free tool," name the tension in the brief and propose how to resolve it. Agencies earn trust by surfacing contradictions, not absorbing them.
