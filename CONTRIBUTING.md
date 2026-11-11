# Contributing to aapl-expiration-tracker

Thank you for contributing to the AAPL options expiration tracker. This repository holds weekly option expiration data for the risk desk, sourced from live market data (Yahoo Finance).

## Adding this week's tracking issues

1. Create one issue per upcoming expiration, in date order, titled `Expiry YYYY-MM-DD`.
2. Include in the issue body: the expiration date, the at-the-money strike, the highest-open-interest call strike, the highest-open-interest put strike, and the share price used.

## Adding the expirations.md summary

1. Create a working branch (e.g. `add-expirations-markdown`).
2. Add `expirations.md` at the repo root with:
   - Company snapshot (HQ address, city, sector, industry, share price)
   - Full list of currently available option expiration dates
   - Per-expiration stats table (ATM strike, highest-OI call strike, highest-OI put strike) for the three soonest upcoming expirations
3. Open a pull request from the branch into `main`.
4. After the PR is open, add a short `CONTRIBUTING.md` to `main`, then update the PR branch so it picks up that commit.

## Notes

- All market figures must come from live data. Where a number looks odd, report exactly what the source returned rather than altering it.
- Share price used for ATM calculations is documented in each issue and in `expirations.md`.
- Open interest and volume figures can shift intraday; note the pull timestamp in PR descriptions.
