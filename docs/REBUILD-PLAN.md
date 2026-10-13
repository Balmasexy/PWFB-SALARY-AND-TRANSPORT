# PWFB Salary and Transport Rebuild

This repository is separate from World Wallet AI.

## Transport acceptance checks
- DM 1: 66 expected records.
- DM 2: 70 expected records.
- Combined expected transport count: 136.

These are expected counts, not verified database counts. Never invent,
remove, alter, or mix records to force the totals to match.

## Keep datasets separate
Transport records and salary-payment records must remain separate.

DM 2 salary-payment reconciliation reference:
- 69 payments
- Control total: ₦11,948,980

Verify these figures against the original source records before marking
them reconciled. Check the complete first section and references 057–069.

## Release requirements
1. Inspect the existing source layout and database before moving code.
2. Preserve login, permissions, and existing records.
3. Make DM 1 and DM 2 independently selectable; default to DM 1.
4. Validate counts and financial totals against actual source data.
5. Test desktop and mobile layouts and run the existing build.
6. Deploy to a separate Render staging service before production changes.
7. Never commit credentials, API keys, tokens, or private keys.
