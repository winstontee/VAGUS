# VAGUS — client acquisition and program launch for The Vagus Effect

This repo holds the marketing, content, website and program materials for a
counselling practice, **The Vagus Effect** (https://vaguseffect.com/). It is
not a software product. Most output is Markdown drafts plus a small static site.

## Goal

1. Make the practitioner findable and trusted, so she gets 1:1 clients.
2. Build an email list from that audience.
3. Turn what she learns from clients into a paid program, sold to that list.

Clients first, program second. Do not design the full program before she has
real 1:1 clients to learn from; a small paid pilot cohort comes before any
public launch.

## The practitioner

| Fact | Status |
| --- | --- |
| Name | Amber Shanahan |
| Practice | The Vagus Effect — vaguseffect.com (Squarespace) |
| Location | Vancouver, BC; sessions online "across Canada" (see compliance questions) |
| Designation | **RTCc** (Registered Therapeutic Counsellor Candidate), ACCT. Working toward CPCA MPCC-P — **in progress, never claim it** |
| Focus | Trauma-informed counselling; complex trauma / C-PTSD without pathologising labels |
| Approach | Relational, somatic, nervous-system (vagus) informed, attachment-aware |
| Other training | Holistic nutrition, somatic practitioner, somatic EMDR, coaching — full list on her About page |
| Pricing, email tool | **Not yet provided** — leave `[PLACEHOLDER]` markers, never invent |

`docs/research/current-site.md` summarises her current site, voice and gaps.
Her own site copy is the voice reference — match it, don't replace it.

## Non-negotiable rules

### Title and credentials
- Use only: "RTC Candidate (ACCT)" or "RTCc". Never "Registered Therapeutic
  Counsellor", "RTC", "therapist", "psychotherapist", "clinical counsellor"
  or "psychologist".
- Do not imply full RTC status until she has it. When she does, this file
  gets updated first.
- Do not claim her sessions are covered by insurance. Coverage found so far
  (e.g. Pacific Blue Cross) lists RTC/MTC/RCS, not candidates.

### Claims
- No promises of cure, recovery timelines or guaranteed outcomes.
- The paid program is **education and nervous-system skills**, not
  counselling or treatment. Program copy must say so.
- Don't diagnose readers ("you have C-PTSD"). Use "if this sounds familiar"
  framing and point to a professional assessment.

### Safety
- Every page, email and lead magnet about trauma includes crisis info:
  call or text **9-8-8** (Suicide Crisis Helpline, Canada) or **911** in an
  emergency. Check these against official sources before publishing.
- Content must not walk readers through trauma processing or memory work
  on their own. Regulation and grounding skills only.

### Testimonials and privacy
- No testimonials, case stories or quotes from current clients.
- Any client-derived example must be a composite with no identifying detail,
  and marked as such.
- This repo is public. No client information, ever.

### Voice
- Everything here is a **draft for her to rewrite in her own voice**.
  Generic AI trauma content damages credibility with this audience.
- Plain, warm, non-clinical, no hype, no toxic positivity, no "healing
  journey" clichés. Short sentences. Mark spots needing her personal story
  with `[HER STORY: ...]`.

### Open compliance questions
Track in `docs/compliance/open-questions.md`. Known ones:
- ACCT Code of Ethics and Standards of Practice (Aug 2025) — advertising,
  testimonial and supervision-disclosure rules not yet read.
  acctcounsellor.com blocks automated access (Cloudflare challenge); do not
  try to bypass it. Use copies the practitioner provides.
- Online counselling "across Canada": Ontario and Quebec restrict
  psychotherapy to regulated professionals, and several Atlantic provinces
  regulate counselling therapy titles. Check whether an RTCc can serve
  clients there.
- Whether an RTCc must name her clinical supervisor in marketing.
- BC is moving counselling under a regulatory college; watch for title
  restrictions.

## Layout

```
docs/strategy/     positioning, audience, offer ladder, pricing, channels
docs/content/      lead magnet, email sequences, social posts, directory bios
docs/compliance/   reviews of drafts, open questions, sources
site/              static landing page (plain HTML/CSS, no build step)
```

## Working as an agent team

Roles are defined in `.claude/agents/`:

- **strategist** — positioning and offer; works first. Owns `docs/strategy/`.
- **content-writer** — drafts in her voice. Owns `docs/content/`.
- **web-developer** — landing page. Owns `site/`.
- **ethics-reviewer** — reviews everything against the rules above. Owns
  `docs/compliance/`. Nothing is "done" until it passes review.

Coordination:
- Each teammate only writes in the directory it owns, so nobody overwrites
  anyone else.
- Content and site wait for `docs/strategy/positioning.md` before drafting
  final copy.
- Unknown facts about the practitioner become `[PLACEHOLDER: ...]`, collected
  in `docs/open-questions.md` for the user to answer. Never fill them in.
- Cite sources for any factual or regulatory claim.
