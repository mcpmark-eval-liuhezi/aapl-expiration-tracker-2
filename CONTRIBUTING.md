# Contributing to aapl-expiration-tracker

Thanks for your interest in contributing to this repository! This repo tracks Apple (AAPL) options expiration data for weekly risk meeting reviews. All market figures must come from live data sources (Yahoo Finance via the desk's data pipeline).

## Adding a new expiration tracker

1. Create a tracking issue titled `Expiry YYYY-MM-DD` (substitute the real date).
2. Include in the issue body:
   - The expiration's at-the-money strike (closest strike to current share price)
   - The highest-open-interest call strike and its OI
   - The highest-open-interest put strike and its OI
   - The share price you used
3. Add `expirations.md` on a new branch (e.g. `add-expirations-markdown`) at the repo root with the company snapshot, full expiration list, and a per-expiration stats table.
4. Open a pull request from that branch into `main`.

## Code & workflow contributions

- Keep changes minimal and focused (one file or one job per PR).
- Use `作出的` minimal CI workflow in `.github/workflows/` triggered manually (`workflow_dispatch`).
- When adding a workflow, echo a single line in the job so runs are trivially verifiable.

## Data integrity

- Report exactly what the source returns; do not "clean up" odd values silently.
- Note the share price used and the pull date in every stats table.
- Flag low-liquidity expirities (e.g. OI 0 / volume null) rather than omitting them.

## Discussion

Repo discussions are off-topic Friendly; file issues for data fixes and PRs for changes.
