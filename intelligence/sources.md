# Sources and validation

## Preferred hierarchy

1. **SpaceX official** — [SpaceX](https://www.spacex.com/) and the [Starbase Louisiana page](https://www.spacex.com/sites/starbase-la).
2. **SpaceX Careers** — [official careers page](https://www.spacex.com/careers/) and exact official posting URLs.
3. **LED / Opportunity Louisiana** — [2026-08-25 announcement](https://www.opportunitylouisiana.gov/news/spacex-launches-new-era-of-commercial-spaceflight-with-100-billion-louisiana-campus) and [Starbase Louisiana FAQ](https://www.opportunitylouisiana.gov/spacex).
4. **State agencies** — for example [Louisiana DOTD](https://dotd.la.gov/), [LDWF](https://www.wlf.louisiana.gov/), CPRA, LDEQ, and Louisiana Public Service Commission.
5. **Parish / local government** — Vermilion Parish and affected local bodies.
6. **Regulators / permitting bodies** — authoritative permit, environmental, wetlands, utility, and launch records.
7. **Credible local reporting** — useful for discovery and local context; promote claims only after primary confirmation when possible.
8. **Broader news / industry reporting** — useful for discovery and independent context, not a substitute for available primary records.

Source class in the news log is separate from hierarchy position: **A** official SpaceX/government/regulator; **B** major credible reporting; **C** local/secondary; **D** unverified/monitoring.

## Source register

| Source ID | Source | Publication date | Retrieved | Live check | Claims used |
|---|---|---:|---:|---|---|
| SRC-001 | [LED release](https://www.opportunitylouisiana.gov/news/spacex-launches-new-era-of-commercial-spaceflight-with-100-billion-louisiana-campus) | 2026-08-25 | 2026-09-13 | HTTP 200; visible dated release and body checked | FACT-001–FACT-014 |
| SRC-002 | [LED Starbase Louisiana landing page / FAQ](https://www.opportunitylouisiana.gov/spacex) | **Unknown — no visible publication date** | 2026-09-13 | HTTP 200; FAQ wording checked | FACT-001, FACT-002, FACT-003, FACT-005, FACT-009–FACT-013, FACT-015–FACT-017 |
| SRC-003 | [SpaceX Starbase Louisiana](https://www.spacex.com/sites/starbase-la) | **Unknown — no visible publication date in retrieved response** | 2026-09-13 | HTTP 200; official page shell live; configured content endpoint returned no usable page record | No claim promoted; contradiction/new-material check limited |
| SRC-004 | [SpaceX Careers](https://www.spacex.com/careers/) | **Unknown — no visible publication date in retrieved response** | 2026-09-13 | HTTP 200; official page shell live; no exact Louisiana posting captured | No open-role claim |
| SRC-005 | [SpaceX — Government Affairs Manager](https://job-boards.greenhouse.io/spacex/jobs/8787398002); [individual API](https://boards-api.greenhouse.io/v1/boards/spacex/jobs/8787398002) | `2026-09-14T12:57:12-04:00` (`first_published`) | 2026-09-16 UTC | HTTP 200 for exact posting and API; ID `8787398002`, exact title, and `Pecan Island, LA` also present in [official board listing](https://boards-api.greenhouse.io/v1/boards/spacex/jobs) | FACT-018; ROLE-001 |
| SRC-006 | [SpaceX — Sr. Counsel, Real Estate & Infrastructure](https://job-boards.greenhouse.io/spacex/jobs/8808149002); [individual API](https://boards-api.greenhouse.io/v1/boards/spacex/jobs/8808149002) | `2026-09-15T11:40:54-04:00` (`first_published`) | 2026-09-16 UTC | HTTP 200 for exact posting and API; ID `8808149002`, exact title, and `Pecan Island, LA` also present in [official board listing](https://boards-api.greenhouse.io/v1/boards/spacex/jobs) | FACT-019; ROLE-002 |

## Reproducible validation

For every meaningful item:

1. Open the canonical URL directly; do not use a search snippet as evidence.
2. Record HTTP availability, visible publisher, exact page title, publication date or explicit `unknown`, and UTC retrieval date.
3. Capture claim wording with its qualifier (`announced`, `expected`, `estimated`, `targeted`, `evaluating`, `required`, `approved`, `started`, or `completed`).
4. Assign stable source and fact IDs. Link every role signal to facts.
5. Compare against current facts and log rows. Ignore syndicated copies and unchanged claims.
6. Look for contradictions in higher-ranked or newer authoritative sources. If unresolved, retain both wordings and explain the difference; do not average or silently choose one.
7. For an open role, require an active official posting URL plus exact role, location, and check date. A careers landing page, stale posting, aggregator, or search result cannot prove a current vacancy.

## Freshness policy

- Review the 12 queries in the [weekly routine contract](README.md#weekly-routine-contract).
- Recheck official project, government, regulator, and careers sources before promoting a change.
- A live undated page gets a retrieval date, never an invented publication date.
- Treat targets, estimates, and evaluations as time-sensitive. Revalidate them when a newer authoritative source appears.
- If there is no meaningful change, make no repository edit, alert, or follow-up issue.
- Corrections append a new log row and preserve the superseded record.

## Current validation note

The two LED pages were live and supplied the seed evidence on 2026-09-13. The official SpaceX project link was followed and live. Its retrieved page was client-rendered, and the configured content lookup did not return usable claim text, so this review promotes no additional SpaceX-page claims and reports no verified contradiction. GitHub reported the public repository default branch as `phs-030-mission-readme`; its live README was 6,573 bytes and exactly matched the pinned baseline SHA-256 `49961b6d279c5aaa4b2a4728081fc1c60c227fa959a0333d04be4613a5a6dc15`. The raw `main/README.md` URL returned HTTP 404, consistent with `main` not yet being the public default branch.

On 2026-09-16 UTC, the exact official pages and individual API records for SRC-005 and SRC-006 returned HTTP 200, and both IDs were present with matching titles and locations in the official SpaceX Greenhouse board listing. API `first_published` timestamps are used as publication dates; retrieval time is not substituted. These records establish two time-bound official vacancies only. They do not establish first-ever Louisiana hiring, continuity with earlier reports, a third vacancy, engineering hiring, approved utilities, or construction start.
