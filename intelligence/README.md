# Starbase Louisiana intelligence

This directory turns verified public information into durable, reviewable signals without publishing private career data.

## Information flow

```text
NEWS
  → SOURCE CHECK
  → NEWS LOG
  → DURABLE FACT
  → SITE FACT
  → ROLE / CAPABILITY SIGNAL
  → private M4 target-role matrix
  → private resume / application decisions
```

The public layer ends at generic role and capability signals. The M4 matrix, candidate fit, resume evidence, application timing, recruiters, authorization information, gaps, and interview strategy remain private and are never linked from this repository.

## Meaningful-item test

Before an item changes these files, answer all seven questions:

1. **What changed?** State the new or corrected claim.
2. **How reliable is the source?** Apply the class and hierarchy in [sources.md](sources.md).
3. **Is it durable?** Separate an announcement, estimate, target, evaluation, approval, construction start, or completion.
4. **What capability does it imply?** Link a stable fact ID to a construction or execution capability.
5. **Which role families may benefit?** Record only a generic inferred family unless an official vacancy is verified.
6. **Does strategy change?** State the generic consequence publicly; candidate-specific conclusions belong in the private M4 handoff.
7. **Does resume emphasis change?** State only the generic evidence category publicly; candidate evidence and edits remain private.

### Worked example

The 2026-08-25 Louisiana Economic Development release announced that the planned site is expected at full buildout to include five launch complexes, each with two pads and a propellant farm.

- **Changed:** a government announcement supplied site-scale and system details.
- **Reliability:** Class A government primary source; the announcement attributes the project to SpaceX.
- **Durability:** planned full-buildout configuration, not a completed or approved facility.
- **Capability:** large civil/structural/mechanical packages, multi-complex interfaces, and construction management.
- **Likely families:** civil, structural, mechanical, construction management; these are inferred, not vacancies.
- **Strategy consequence:** monitor package sequencing and official hiring signals before changing targeting.
- **Resume-emphasis consequence:** relevant candidates may emphasize verified multi-package delivery and interface-management evidence; no personal evidence is stored here.

Links: [FACT-005](site-facts.md#fact-005--launch-complexes-and-pads) and [SIG-001](role-signals.md#sig-001--launch-infrastructure).

## Weekly routine contract

Review all 12 queries once per week:

- `SpaceX Louisiana`
- `Starbase Louisiana`
- `Vermilion Parish SpaceX`
- `Pecan Island SpaceX`
- `SpaceX construction Louisiana`
- `SpaceX jobs Louisiana`
- `SpaceX contractors Louisiana`
- `SpaceX permitting Louisiana`
- `SpaceX utilities Louisiana`
- `SpaceX power generation Louisiana`
- `SpaceX launch complex Louisiana`
- `SpaceX propellant Louisiana`

Validate any candidate change against primary sources and deduplicate syndication. If there is **no meaningful change**, make no repository edit, send no alert, and create no follow-up issue. A meaningful change requires a validated [news-log](news-log.md) entry, fact promotion or correction in [site-facts](site-facts.md), and a [role signal](role-signals.md) update when warranted. Send a private M4 handoff only when the change is relevant to strategy or resume emphasis.

### No-change example

A weekly search returns copies of the same 2026-08-25 release and an unchanged FAQ. After URL, date, and claim comparison, record nothing: no new fact, no log row, no alert, and no issue.

### Correction example

If a regulator later publishes a decision moving the launch target from 2029 to 2030, append a new correction row to `news-log.md`, mark the old fact superseded without deleting its history, add the new sourced fact, and reassess linked signals. Never silently rewrite the historical log row.

## Files

- [news-log.md](news-log.md) — append-only meaningful-change history.
- [site-facts.md](site-facts.md) — durable claims with explicit status and confidence.
- [role-signals.md](role-signals.md) — fact-traced, generic capability implications.
- [sources.md](sources.md) — source hierarchy, validation method, and freshness rules.

## Public-safety boundary

Do not publish personal fit scores, recruiter information, CV or employment evidence, work-authorization information, personal gaps, applications, interviews, or private strategy. Do not link to private documents. Public statements must stay source-backed, generic, and explicit about uncertainty.
