---
description: Run an Operatica.ai cross-functional standup — each officer reports status, wins, risks, and what needs a decision across marketing, operations, technology, and product. Use for a daily or weekly pulse.
argument-hint: [optional focus or time window, e.g. "this week" or "growth only"]
---

Run an Operatica.ai C-suite **standup**. Load the `operatica-context` skill first. This is a
**read-only status pass by default** — do not take actions or make changes; surface what needs a
decision.

For each officer, pull a quick status from their domain. **Degrade gracefully:** if a connector or
skill isn't authorized in this surface, note it briefly and move on.

- **CMO** — active/planned campaigns and lifecycle (`Resend`), notable competitive/market signals,
  growth metrics.
- **COO** — the operating numbers, cadence/calendar for the window (`Google_Calendar`), people/vendor
  items, and any slipping commitments.
- **CTO** — repo/PR and CI status (`github`), deploy/health (`Vercel`), Supabase advisors and
  reliability, and the top technical risks.
- **CPO** — roadmap/backlog status (`github` issues), product-analytics signal (`Vercel`/Supabase
  read), and discovery in flight.

Also check the `knowledge` base (project `erhjcqhcbrycecfijbyv`) for decisions or insights logged
since the last window.

Then synthesize **one briefing**:
1. **Wins** since last time.
2. **Risks / blockers** — each with an owner and what's needed.
3. **Decisions needed** from Grant.
4. **Top 3 priorities** for the window, across the whole company.

Keep it tight and scannable. Confirm before doing anything beyond reporting.

Focus / window (optional):

$ARGUMENTS
