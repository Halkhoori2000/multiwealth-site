# Content verification

Checked against the local MultiWealth checkout on September 10, 2026.
Only feature descriptions are included here; no account records, source documents,
credentials or application screenshots are copied into the showcase.

| Public description | Application source used for verification |
| --- | --- |
| Current navigation and workspaces | `src/App.tsx`, `src/components/layout/AppShell.tsx`, `src/pages/PersonalFinance.tsx` |
| Statement coverage and reconciliation | `src/pages/personal-finance/Statements.tsx`, `src/components/accounts/ImportStatementsDrawer.tsx` |
| AECB report history and estimates | `src/pages/personal-finance/Credit.tsx` |
| Categories, payees and planner buckets | `src/pages/personal-finance/Classify.tsx`, `src/pages/Planner.tsx` |
| Pots and linked balances | `src/pages/Pots.tsx` |
| Real Estate workspace | `src/components/layout/AppShell.tsx`, `src/pages/properties/` |
| PDF parser coverage | `server/src/parsers/index.ts` |
| Generic CSV formats | `src/lib/parseStatementCsv.ts` |
| Cheque states and account detail location | `server/src/routes/cheques.ts`, `src/components/accounts/AccountDetailPanel.tsx` |
| 29 bank/issuer integrations, seven campaign producers, optional scheduling | `services/intel/README.md`, `services/intel/data/banks.yaml` |
| Bank Agents development status | `src/pages/personal-finance/BankAgents.tsx` |
| Copilot preview and live Activity feed | `src/components/copilot/Copilot.tsx` |
| Optional MCP adapter | `services/mcp-adapter/README.md` |
| Ports, modes and client generation | `package.json`, `server/package.json`, `server/.env.example`, `server/prisma.config.ts` |
| Node compatibility | Installed Vite and Prisma package engine declarations |
| Backup defaults and included uploads | `scripts/backup-db.sh` |

## Editorial choices

- A registry entry is described as an integration, not verified complete coverage.
- No product total is advertised without a dated catalog count.
- No bank-specific CSV guarantee is inferred from the generic CSV parser.
- Emirates NBD account/catalog support is kept separate from PDF parser support.
- Illustrative market prices, rates and credit scores are not current data.
- Self-hosted storage is distinguished from connections used by optional services.
- Working ingestion/activity features are distinguished from the Copilot Chat preview.
