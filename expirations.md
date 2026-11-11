# AAPL Expiration Tracker

Weekly tracking of Apple (AAPL) option expiration data for the risk desk. All market figures below were pulled from live data (Yahoo Finance) on 2026-11-11.

## Company Snapshot

| Field | Value |
| --- | --- |
| Company | Apple Inc. (AAPL) |
| Headquarters street address | One Apple Park Way (MS 927-4GC) |
| City | Cupertino, CA 95014, United States |
| Sector | Technology |
| Industry | Consumer Electronics |
| Current share price | $355.63 (USD; regularMarketPrice / currentPrice from Yahoo Finance) |
| Exchange | NasdaqGS (NMS) |
| Market cap | ~$5.168T |
| Analyst consensus | Buy (2.2 mean, 40 opinions) |

## Expiration Map (available expirations, most recent first)

| # | Expiration Date |
| --- | --- |
| 1 | 2026-11-11 |
| 2 | 2026-11-13 |
| 3 | 2026-11-16 |
| 4 | 2026-11-18 |
| 5 | 2026-11-20 |
| 6 | 2026-11-27 |
| 7 | 2026-12-04 |
| 8 | 2026-12-11 |
| 9 | 2026-12-18 |
| 10 | 2026-12-24 |
| 11 | 2027-01-15 |
| 12 | 2027-02-19 |
| 13 | 2027-03-19 |
| 14 | 2027-04-16 |
| 15 | 2027-06-17 |
| 16 | 2027-09-17 |
| 17 | 2027-12-17 |
| 18 | 2028-01-21 |
| 19 | 2028-03-17 |
| 20 | 2028-06-16 |
| 21 | 2028-12-15 |
| 22 | 2029-01-19 |

This week we track the three soonest upcoming expirations: **2026-11-11**, **2026-11-13**, and **2026-11-16**.

## Per-Expiration Stats

Share price used for ATM calculations: **$355.63**

| Expiration | ATM Strike | Highest-OI Call Strike (OI) | Highest-OI Put Strike (OI) |
| --- | --- | --- | --- |
| 2026-11-11 | 355 | 355 (33,155) | 347.5 (6,358) |
| 2026-11-13 | 355 | 360 (16,819) | 330 (10,223) |
| 2026-11-16 | 355 | 355 (5,737) | 330 (1,537) |

### Notes

- **ATM strike** = strike closest to the current share price ($355.63). For all three expirations this is **355** (distance 0.63; the next nearest is 357.5 at distance 1.87).
- **Highest-open-interest call strike** = strike with the largest `openInterest` value on the calls side of the chain for that expiration.
- **Highest-open-interest put strike** = strike with the largest `openInterest` value on the puts side of the chain for that expiration.
- Open interest and volume figures are as returned by the source at pull time and can shift intraday.

## Related Issues

- #5 — Expiry 2026-11-11
- #6 — Expiry 2026-11-13
- #8 — Expiry 2026-11-16
