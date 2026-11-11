# AAPL Expiration Tracker

Weekly tracking of Apple (AAPL) option expirations for the risk meeting. All market figures below are from live data via Yahoo Finance as of the 2026-11-11 session.

## Company Snapshot

| Field | Value |
| --- | --- |
| Company | Apple Inc. |
| Ticker | AAPL (NASDAQGS) |
| Headquarters street address | One Apple Park Way, MS 927-4GC |
| City | Cupertino |
| State / Zip | CA 95014, United States |
| Sector | Technology |
| Industry | Consumer Electronics |
| Current share price | $355.63 (regular market price, latest session 2026-11-11) |
| Market cap | ~$5.168 T |
| Analyst rating | Buy (mean 2.22, 40 opinions) |
| 52-week range | $243.42 – $355.90 |

## Available Option Expiration Dates (AAPL)

| # | Expiration | Tenor |
| --- | --- | --- |
| 1 | 2026-11-11 | Weekly (upcoming) |
| 2 | 2026-11-13 | Weekly (upcoming) |
| 3 | 2026-11-16 | Weekly (upcoming) |
| 4 | 2026-11-18 | Weekly |
| 5 | 2026-11-20 | Weekly |
| 6 | 2026-11-27 | Monthly |
| 7 | 2026-12-04 | Quarterly |
| 8 | 2026-12-11 | Quarterly |
| 9 | 2026-12-18 | Quarterly |
| 10 | 2026-12-24 | Quarterly |
| 11 | 2027-01-15 | Quarterly |
| 12 | 2027-02-19 | Quarterly |
| 13 | 2027-03-19 | Quarterly |
| 14 | 2027-04-16 | Quarterly |
| 15 | 2027-06-17 | Quarterly |
| 16 | 2027-09-17 | Quarterly |
| 17 | 2027-12-17 | LEAP |
| 18 | 2028-01-21 | LEAP |
| 19 | 2028-03-17 | LEAP |
| 20 | 2028-06-16 | LEAP |
| 21 | 2028-12-15 | LEAP |
| 22 | 2029-01-19 | LEAP |

**Tracked expirations this week (3 soonest upcoming, skipping anything earlier than today):** 2026-11-11, 2026-11-13, 2026-11-16.

## Per-Expiration Stats

Share price used for all ATM calculations: **$355.63** (AAPL current price, Yahoo Finance, latest session 2026-11-11).

### Expiry 2026-11-11

| Metric | Value |
| --- | --- |
| At-the-money strike (closest to $355.63) | **355.0** |
| Highest-open-interest call strike | **355.0** (OI 33,155; contract AAPL261111C00355000) |
| Highest-open-interest put strike | **340.0** (OI 5,854; contract AAPL261111P00340000) |

### Expiry 2026-11-13

| Metric | Value |
| --- | --- |
| At-the-money strike (closest to $355.63) | **355.0** |
| Highest-open-interest call strike | **360.0** (OI 16,819; contract AAPL261113C00360000) |
| Highest-open-interest put strike | **330.0** (OI 10,223; contract AAPL261113P00330000) |

### Expiry 2026-11-16

| Metric | Value |
| --- | --- |
| At-the-money strike (closest to $355.63) | **355.0** |
| Highest-open-interest call strike | **355.0** (OI 5,737; contract AAPL261116C00355000) |
| Highest-open-interest put strike | **330.0** (OI 1,537; contract AAPL261116P00330000) |

## Notes for the Risk Meeting

- ATM strike is 355.0 for all three expirations since $355.63 sits between the 352.5 and 357.5 strikes and is closest to 355.0.
- Call OI leadership is concentrated at 355.0 for the two nearest expirations (11-11 and 11-16) and shifts to 360.0 for 11-13, indicating flow rotating into the front week.
- Put OI leadership is at 340.0 (11-11), 330.0 (11-13 and 11-16) — slightly out-of-the-money protection premia that narrow as we move out one expiry.
- All figures are as returned by Yahoo Finance on the 2026-11-11 session and should be re-pulled live before the meeting.

## Tracking Issues

| Issue | Expiry | Details |
| --- | --- | --- |
| #10 | 2026-11-11 | Company snapshot, ATM 355.0, call OI leader 355.0 (33,155), put OI leader 340.0 (5,854), share price $355.63 |
| #12 | 2026-11-13 | Company snapshot, ATM 355.0, call OI leader 360.0 (16,819), put OI leader 330.0 (10,223), share price $355.63 |
| #13 | 2026-11-16 | Company snapshot, ATM 355.0, call OI leader 355.0 (5,737), put OI leader 330.0 (1,537), share price $355.63 |

## Repository

- URL: https://github.com/mcpmark-eval-liuhezi/aapl-expiration-tracker-2
- Branch with this file: `add-expirations-markdown` (open PR into `main`)
- CONTRIBUTING.md: added to `main` after the PR was opened, and the PR branch was updated to include it.
- CI: manual (`workflow_dispatch`) demo workflow added to `main`; run triggered once and logs deleted to keep the repo tidy.
- Discussions: none configured on this repository yet.
