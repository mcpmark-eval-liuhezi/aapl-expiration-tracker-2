# AAPL Options Expiration Tracker

Weekly tracking repository for Apple (AAPL) options expiration review ahead of the risk meeting.

All market figures below were pulled **live from Yahoo Finance** at the time of week's review.
Any number that looks odd is reported exactly as the source returned it.

---

## 1. Company Snapshot (Apple Inc.)

| Field | Value |
|-------|-------|
| **Ticker** | AAPL |
| **Headquarters street address** | One Apple Park Way, MS 927-4GC |
| **City** | Cupertino |
| **State / ZIP** | CA 95014, United States |
| **Sector** | Technology |
| **Industry** | Consumer Electronics |
| **Current share price** | $355.63 (US, NasdaqGS, last trade $355.63; post-market $355.47) |
| **Exchange** | NMS (Nasdaq Global Select Market) |
| **Market cap** | ~$5.168T |
| **Analyst consensus** | Buy (mean 2.22, 40 analysts) |

---

## 2. Expiration Map (available expirations returned by Yahoo Finance)

Full list of currently available AAPL option expiration dates:

| # | Expiration | Tenor |
|---|-----------|-------|
| 1 | **2026-11-11** | Soonest upcoming |
| 2 | **2026-11-13** | 2nd soonest |
| 3 | **2026-11-16** | 3rd soonest |
| 4 | 2026-11-18 | Weekly |
| 5 | 2026-11-20 | Weekly |
| 6 | 2026-11-27 | Monthly |
| 7 | 2026-12-04 | Monthly |
| 8 | 2026-12-11 | Monthly |
| 9 | 2026-12-18 | Monthly |
| 10 | 2026-12-24 | Monthly |
| 11 | 2027-01-15 | Quarterly |
| 12 | 2027-02-19 | Quarterly |
| 13 | 2027-03-19 | Quarterly |
| 14 | 2027-04-16 | Quarterly |
| 15 | 2027-06-17 | Quarterly |
| 16 | 2027-09-17 | Annual |
| 17 | 2027-12-17 | Annual |
| 18 | 2028-01-21 | Annual |
| 19 | 2028-03-17 | Annual |
| 20 | 2028-06-16 | Annual |
| 21 | 2028-12-15 | Annual |
| 22 | 2029-01-19 | Annual |

> The three soonest upcoming expirations (skipping anything earlier than today) are **2026-11-11**, **2026-11-13**, and **2026-11-16**. These are the focus of this week's per-expiration stats below.

---

## 3. Per-Expiration Chain Stats

**Reference share price used throughout:** **$355.63**

### Expiration 2026-11-11 (weekly, ~2 days to expiry)

| Metric | Value |
|--------|-------|
| **At-the-money strike** | **355** (closest strike to $355.63; $0.63 away) |
| **Highest-OI call strike** | **355** (Open Interest **33,155**; last $0.65; volume 183,207) |
| **Highest-OI put strike** | **340** (Open Interest **5,854**; last $0.01; volume 6,326) |

### Expiration 2026-11-13 (weekly, ~4 days to expiry)

| Metric | Value |
|--------|-------|
| **At-the-money strike** | **355** (closest strike to $355.63; $0.63 away) |
| **Highest-OI call strike** | **360** (Open Interest **16,819**; last $0.84; volume 22,135) |
| **Highest-OI put strike** | **330** (Open Interest **10,223**; last $0.04; volume 6,984) |

### Expiration 2026-11-16 (weekly, ~5 days to expiry)

| Metric | Value |
|--------|-------|
| **At-the-money strike** | **355** (closest strike to $355.63; $0.63 away) |
| **Highest-OI call strike** | **355** (Open Interest **5,737**; last $3.68; volume 2,541) |
| **Highest-OI put strike** | **320** (Open Interest **951**; last $0.04; volume 137) |

---

## 4. Summary Table

| Expiration | ATM Strike | Top-Call OI Strike (OOI) | Top-Put OI Strike (OOI) | Share Price Used |
|-----------|-----------|--------------------------|-------------------------|------------------|
| 2026-11-11 | 355 | 355 (33,155) | 340 (5,854) | $355.63 |
| 2026-11-13 | 355 | 360 (16,819) | 330 (10,223) | $355.63 |
| 2026-11-16 | 355 | 355 (5,737) | 320 (951) | $355.63 |

---

## 5. Notes & Observations

- **ATM strike is 355 for all three expirations** — spot ($355.63) sits between the 352.5 and 355 strikes, and 355 is the closest listed strike in every chain returned by the source.
- **Call OI concentration:** The 2026-11-11 expiry shows the heaviest call open interest at strike 355 (33,155 contracts), which is typical for the nearest weekly where dealer positioning clusters around spot. For 2026-11-13 the top call OI moves to 360 (16,819), and for 2026-11-16 it回到 355 (5,737) as liquidity thins out two weeks out.
- **Put OI drifts lower strike-wise across expirations:** 340 (11-11) → 330 (11-13) → 320 (11-16). This is a normal pattern as} Long-dated put protection demand concentrates further out, and near-term put OI follows the money lower.
- **Low-liquidity flag (reported exactly as returned):** The 2026-11-16 put chain shows very thin activity — top put OI is only 951 at strike 320 with volume of 137, and many strikes report `openInterest: 0` or `volume: null`. Treat that expiry's put stats as approximate.
- **Puts at-the-money (357.5) are in-the-money** per the source (`inTheMoney: true`) for the 2026-11-11 chain, whereas calls at 355 are also marked inTheMoney: true in that same chain — reported verbatim from the source.
- Tracking issues for each expiration are #7 (2026-11-11), #9 (2026-11-13), and #11 (2026-11-16) in this repo.

---

## 6. Repository Structure

- `README.md` — this repo's overview
- `CONTRIBUTING.md` — contribution guidelines on `main`
- `expirations.md` — this file (added via PR from `add-expirations-markdown`)
- `.github/workflows/` — minimal manual trigger workflow for CI checks
- Issues #7, #9, #11 — per-expiration tracking issues

*Data source: Yahoo Finance (live pull).Figures are reported exactly as returned by the source at pull time.*
