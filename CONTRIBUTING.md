# Contributing to aapl-expiration-tracker

This repository tracks Apple (AAPL) options expiration data weekly for the risk desk review.

## Adding a New Week's Data

1. Create a new branch from `main` (e.g., `add-expirations-markdown-YYYY-MM-DD`).
2. Add or update `expirations.md` at the repo root with:
   - Company snapshot (headquarters, sector, industry, current share price)
   - Full list of available option expiration dates
   - Per-expiration stats table (ATM strike, highest-open-interest call strike, highest-open-interest put strike, share price used)
3. Open a pull request from your branch into `main`.
4. Once the PR is open, add a `CONTRIBUTING.md` to `main` if not already present, then update your PR branch with the latest `main` so it picks up that commit.

## Data Standards

- All market figures must come from live data (Yahoo Finance via the desk's MCP tools).
- Where a number looks odd, report exactly what the source returned rather than silently correcting it.
- Reference share price used should be stated explicitly in each tracking issue and in `expirations.md`.

## Workflow

A manual trigger workflow (`.github/workflows/manual-check.yml`) is available on `main`. It runs a single job that echoes a line and can be triggered via GitHub Actions -> Workflow spectrum -> Run workflow.

## Tracking Issues

Each expiration gets its own tracking issue titled `Expiry YYYY-MM-DD` with ATM strike, top-OI call strike, top-OI put strike, and the share price used.
