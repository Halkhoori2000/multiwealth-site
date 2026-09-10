# MultiWealth showcase

A static showcase and user guide for the private, self-hosted MultiWealth application.
Content reflects the application as of September 10, 2026.

## Current application

- **Overview:** net worth across accounts, investments, real estate and tangibles.
- **Personal Finance:** Accounts, Statements, Classify, Planner, Credit, Investments,
  Tangibles, Pots and Catalog.
- **Credit:** AECB report history, facility matching and labelled model estimates.
- **Real Estate:** Estate, Tenants, Mortgages, Rental Income, Expenses and Documents.
- **Catalog:** Products, Compare, Offers, Alerts and Key Facts Statement history.
  The optional Intel service has 29 bank and issuer integrations; actual coverage
  and freshness depend on each source and the latest successful refresh.
- **Integrations:** Bank Agents are under development. Agent ingestion and the MCP
  adapter require separate configuration. The in-app Copilot Chat is a UI preview;
  the Activity feed is connected.

Financial records and documents are stored on the user's host. Market data,
catalog refreshes and optional integrations use external services when enabled.
All website previews use fictional balances, scores, transactions and rates.

## Preview

No build or installation is required:

```sh
python3 -m http.server 5180 --bind 127.0.0.1
```

Open `http://127.0.0.1:5180` for the landing page and `/docs.html` for the guide.

## Files

- `index.html`: landing page, illustrative UI previews and responsive styles.
- `docs.html`: setup guide, module documentation and integration status.
- `favicon.svg`: existing project identity.
- `assets/`: legacy promotional images, retained but not used by the updated pages.
- `CONTENT_SOURCES.md`: source locations used to check product claims.

## Publishing

GitHub Pages currently serves the `main` branch from `/` at
`https://halkhoori2000.github.io/multiwealth-site/`.

After reviewing a change, push its commit to `main`. GitHub Pages builds and
publishes automatically. The legacy `gh-pages` branch is no longer the configured
source. No build step, visibility change or force push is required.

The application remains in its separate private repository. This repository
contains only the showcase and guide, not application source or user records.
