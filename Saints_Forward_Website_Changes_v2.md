# Saints Forward Website — Implementation Plan v2

This document is a change spec for the saintsforward.ca static website. Hand this to Claude Code for implementation.

---

## Change 1: Update Contact Email Everywhere

**Find and replace ALL instances of:**
- `info@saintsfc` → remove entirely (this is the SGSA board's email, not ours)
- Any other placeholder emails

**Replace with:**
- `contact@saintsforward.ca`

This includes: the Get Involved section, the footer, any mailto: links, meta tags, and anywhere else an email appears. Do a global search — there should be zero references to `info@saintsfc` or any `@saintsfc.ca` address anywhere on the site when done.

---

## Change 2: Make the Contact Email Prominent and Inviting

The contact email needs to be **impossible to miss** and the messaging around it should make it crystal clear that ALL feedback is welcome.

### Implementation:

**Add a dedicated "Talk to Us" block** — this should be its own visually distinct section (or a prominent part of the Get Involved section). It should include:

- The email: `contact@saintsforward.ca` — displayed large, clickable (mailto: link), and visually prominent
- Messaging along these lines (adapt to match the site's existing voice):

> **We want to hear from you.**
> Whether you have feedback on this website, thoughts on the plan, ideas we haven't considered, questions, concerns, or just want to say you're in — we want to hear it all. Every perspective makes this initiative stronger.
>
> **contact@saintsforward.ca**

- This block should appear:
  1. In the "Get Involved" section (primary placement)
  2. In the footer (secondary, smaller)
  3. Optionally as a floating or sticky element on mobile (subtle, not annoying)

**Tone:** Warm, open, zero gatekeeping. The vibe is "this is a conversation, not a broadcast."

---

## Change 3: Reframe the Goals — North Star + Incremental Steps

The two goals (dedicated indoor facility + permanent coaching positions) should remain clearly stated as the **north star** — the long-term vision. But the site's messaging needs to make clear that we don't need to get there in one leap. We just need to start moving.

### Implementation:

**Update the Plan / Goals section** to add framing language before or after the two goals. Something like:

> **Our north star is clear:** a dedicated indoor facility and professional coaching for SGSA. These are achievable, well-researched goals that other clubs our size have already accomplished.
>
> **But we don't need to get there overnight.** What matters right now is that we start taking steps in the right direction — having the conversations, doing the research, forming the committees, and exploring the options. Every step forward is a step worth taking.
>
> The first step? Simply agreeing, as a community, that it's time to move.

**Key principle:** The goals section should NOT read like a demand list. It should read like a shared aspiration with a pragmatic, "let's just get started" energy. The north star gives direction; the incremental framing removes the intimidation factor.

### Specific text changes:

- Where the goals are listed, add a header like: **"Our North Star"** or **"Where We're Headed"**
- Below the goals, add a subsection: **"The First Step"** — emphasizing that all we need right now is for the community to agree it's time to explore these options seriously
- Avoid any language that implies the dome must happen by a specific date or that failure is imminent
- The feeling should be: optimistic momentum, not urgent crisis

---

## Change 4: Update Key Data Points

The site should reflect the latest registration data:

- **956 registered players** this season
- **54 teams** across all age groups
- **~$400 average registration fee per player per season** (conservative estimate)
- **~$382,400 estimated annual registration revenue** (956 × $400)
- **~$200,000/year** spent on Tri Leisure Centre indoor rental (existing data point)
- That means roughly **52% of registration revenue goes to renting someone else's facility**

This data should appear in the "Problem" or data section of the site. The 52% stat is the killer number — make it visually prominent.

### Suggested data card:

```
$382K
estimated annual registration revenue

$200K
spent renting indoor space at Tri Leisure Centre

52%
of your registration fees go to a facility we don't own
```

---

## Change 5: Minor Polish

- Make sure the site has a proper `<title>` tag: "Saints Forward — Building the Future of Spruce Grove Soccer"
- Verify Open Graph / social sharing meta tags are set (og:title, og:description, og:image)
- Ensure the favicon is set (use the saints-forward-favicon.svg from the workspace)
- Double-check all external links open in new tabs (`target="_blank" rel="noopener"`)
- Make sure the site is fully responsive and looks good on mobile (parents will share via text)
- Verify the reports section links to downloadable PDFs (not .docx)

---

## Design & Tone Reminders

- **Color palette:** Dark forest green (#1B4332), gold (#D4A843), warm off-white (#F8F6F0), dark charcoal (#1A1A2E)
- **Font:** Inter (Google Fonts)
- **Tone:** Collaborative, data-driven, optimistic. We love this club. We're building something together.
- **Never:** Name individuals, assign blame, use adversarial language, or make it feel like members vs. board

---

## Summary of Changes

| # | Change | Priority |
|---|--------|----------|
| 1 | Replace all emails with contact@saintsforward.ca | HIGH |
| 2 | Make contact email prominent + "all feedback welcome" messaging | HIGH |
| 3 | Reframe goals as north star + incremental steps | HIGH |
| 4 | Add 956 players / 54 teams / $382K revenue / 52% stat | MEDIUM |
| 5 | Meta tags, favicon, mobile polish, PDF links | MEDIUM |

---

*This spec is designed to be handed to Claude Code for implementation against the existing saintsforward.ca codebase.*
