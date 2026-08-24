# Spaza Fund Atlas

A public, searchable transparency project for browsing South African Spaza Shop Support Fund approvals.

## What is in the Atlas

The site converts the published 34-page Annexure A approvals list into a searchable register. The current extraction contains **1,383 approval records** with a combined published package value of **R83,766,000**.

Visitors can search and filter by beneficiary, province, district and municipality; sort approvals; open beneficiary profiles; and download the currently filtered results as CSV.

Core fields are beneficiary/spaza-shop name, approval date, province, district, municipality, approved package amount, source page and research status.

## Evidence standard

The Annexure is the primary source for approval information. Independent company, director, address, contract and web research is stored separately and linked to supporting evidence.

Being listed in the Atlas is **not an allegation of wrongdoing**. “Unresearched” means no independent public-record review has yet been completed. A missing online footprint is not adverse evidence, and similar company names are not treated as identity matches without sufficient corroboration.

## Initial researched profiles

The first research layer includes MAHLASELA FRUIT AND VEG MARKET, NTOMBILELE LEGACY and PRELIM LOGISTIX. Each profile separates the source record from independent public evidence and states any identity limitation explicitly.

## Deployment

A GitHub Pages workflow is included at `.github/workflows/pages.yml`. Once GitHub Pages is configured to use **GitHub Actions** as its publishing source, pushes to `main` deploy automatically.

Expected project-site URL after Pages is enabled:

`https://mahlatse32.github.io/spaza-fund-atlas/`

## Repository structure

- `index.html` — public interface
- `styles.css` — responsive presentation
- `app.js` — search, filters, profiles, pagination and CSV export
- `packed-*.js` — compressed source dataset split into safe static chunks
- `research.js` — sourced independent research profiles
- `.github/workflows/pages.yml` — automatic GitHub Pages deployment

## Status

Public v1 code and the complete extracted dataset are committed. The research layer can now expand progressively across all beneficiaries.
