# FUNGO — Transparency & Reporting Framework

This document defines how project information should be published and updated. It is a reporting standard, not a claim that every item below has already been completed.

## 1. Public status

| Item | Current status |
|---|---|
| Project name / ticker | FUNGO / FUNGO |
| Intended network | Solana |
| Intended launch venue | Pump.fun |
| Mint address | Supplied by maintainer; independent verification pending |
| Graduation | Not yet graduated, per maintainer |
| PumpSwap pool | Not confirmed |
| Official website / social links | Not supplied in this repository |
| Audit report | None documented |
| Formal DAO governance | Not documented |

## 2. Publication rules

- Use the exact mint address as the canonical token identifier.
- Label maintainer-supplied information separately from independently verified facts.
- Attach an explorer link and transaction signature to material on-chain claims.
- Include the date and, where possible, the Solana slot for snapshots.
- Correct errors openly with a dated repository commit.
- Never fabricate holder counts, market cap, volume, liquidity, allocation, or partnership claims.
- Do not call a planned feature launched until users can access it and evidence is linked.

## 3. Recommended monthly disclosure

When reliable data is available, publish:
- Mint address and token metadata.
- Total supply, decimals, mint authority, freeze authority, token program.
- Holder distribution and top-holder concentration with methodology.
- Known project-controlled wallets and their disclosed purposes.
- Bonding-curve state and progress, if available.
- Graduation and migration transaction signatures, if completed.
- Pool address, quote asset, and reserve snapshot, if migrated.
- Material security incidents and remediation status.
- Roadmap progress, delays, and completed deliverables.

## 4. Wallet disclosure template

| Wallet | Public address | Declared role | Evidence / notes |
|---|---|---|---|
| Creator / deployer | Pending | Pending | Do not label without confirmation |
| Treasury | Not disclosed | Not disclosed | No treasury claim |
| Operations | Not disclosed | Not disclosed | No operations-wallet claim |

Do not publish personal identity information or imply ownership from wallet activity alone.

## 5. Change log expectations

Every material update should record:
- Date of observation.
- What changed.
- Source of evidence.
- Relevant mint, account, pool, or transaction address.
- Whether the update is verified or maintainer-reported.

## 6. Status vocabulary

- **Planned:** Intention only; not implemented.
- **In progress:** Work has started; not complete.
- **Maintainer-reported:** Supplied by project maintainer but not independently verified.
- **Verified on-chain:** Supported by a direct chain account or transaction.
- **Completed:** Deliverable exists and its evidence is linked.
- **Not confirmed:** Evidence is not currently available.
- **Not applicable:** The item does not apply.

## 7. Public communication checklist

Before publishing an announcement:
- Confirm the mint address character by character.
- Verify the current lifecycle state.
- Check links and domains.
- Remove unsupported claims and guaranteed-return language.
- State whether figures are live, historical, or estimates.
- Include a concise risk reminder for trading-related posts.
- Ensure the repository and official channels do not contradict one another.

## Creator fees

The creator reports that FUNGO creator fees are enabled. The fee configuration, recipient wallet, rate, accrued amount, and withdrawal history have not yet been independently verified. This is a maintainer-reported disclosure, not a guarantee of fee generation or income.
