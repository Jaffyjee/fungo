# FUNGO — Project Overview & Whitepaper

**Version:** 1.0  
**Project:** FUNGO ($FUNGO)  
**Network:** Solana (intended; verify mint on mainnet)  
**Launch venue:** Pump.fun  
**Lifecycle status:** Pre-graduation; on-chain state must be checked before each public update  
**Mint supplied by maintainer:** `3RWCQUsHN6gJR8saXHMhHa2pKTpJzy889CwUNBsEpump`

## 1. Executive summary

FUNGO is a community-oriented meme-token project intended for the Solana ecosystem. Its initial distribution venue is Pump.fun. This document describes the project's identity, launch model, transparency commitments, and current verification boundaries.

FUNGO is a speculative digital asset. It does not represent equity, debt, a claim on revenue, ownership of a business, or a promise of profit. No price target, return, exchange listing, airdrop, reward, or future utility is guaranteed.

## 2. Project purpose

FUNGO aims to provide a recognizable community token identity and a transparent public information source. The project will prioritize:
- Clear and consistent token identification.
- Publicly documented launch and lifecycle milestones.
- Verifiable links to on-chain activity.
- Explicit disclosure of unknown or unverified information.
- Community safety and resistance to impersonation.

Any future utility or product proposal must be separately documented with its scope, delivery status, dependencies, and risks. Roadmap items are intentions, not guarantees.

## 3. Network and launch architecture

The intended network is Solana and the intended launch venue is Pump.fun. Pump.fun's documented lifecycle includes token creation, trading on a bonding curve, completion of the curve, and migration into a PumpSwap pool after graduation conditions are met. See the platform documentation in [References](#11-references).

**FUNGO has not graduated yet, according to the project maintainer.** This repository does not claim a completed migration, an active PumpSwap pool, or a confirmed DEX listing. The exact current curve state should be checked against the mint and the platform's on-chain accounts.

## 4. Token parameters

| Parameter | Project record | Verification |
|---|---|---|
| Name | FUNGO | Metadata check pending |
| Symbol | FUNGO | Metadata check pending |
| Network | Solana mainnet intended | Mint/account check pending |
| Mint | `3RWCQUsHN6gJR8saXHMhHa2pKTpJzy889CwUNBsEpump` | Supplied by maintainer; not independently confirmed |
| Target supply | 1,000,000,000 | Actual mint supply pending |
| Decimals | Not published | Read from mint |
| Mint authority | Not published | Read from mint |
| Freeze authority | Not published | Read from mint |
| Token program | Not published | Read from account owner |
| Graduation | Not yet graduated | Verify live state |
| PumpSwap pool | Not confirmed | Add only after migration is verified |

Do not treat a project target as an on-chain fact. The actual mint account and transaction history are authoritative for token supply, decimals, authorities, and lifecycle state.

## 5. Tokenomics and distribution

No wallet allocation percentages are asserted in this version. The project will publish distribution information only after reviewing reliable on-chain evidence. A distribution report should distinguish:
- Total minted supply.
- Tokens held in bonding-curve or protocol-controlled accounts.
- Creator/deployer-controlled balances.
- Known treasury or operational wallets, if any.
- Largest holder balances and concentration.
- Burned tokens, if any, with transaction evidence.

Wallet labels should be evidence-based and should not imply beneficial ownership unless that relationship is known. A holder concentration snapshot is time-sensitive and must include its observation slot or timestamp.

## 6. Fees and liquidity

Trading fees, creator fees, platform fees, and migration mechanics are determined by the relevant platform and current protocol implementation. FUNGO will not describe trading as fee-free or liquidity as locked unless the specific claim is supported by current documentation and on-chain evidence.

Graduation is not guaranteed. Even after migration, pool liquidity can be depleted by trading, and token prices can fall sharply.

## 7. Governance and administration

This repository does not currently define a formal DAO, voting system, treasury mandate, or binding governance process. Community discussion does not itself create enforceable governance rights. Any future governance mechanism must publish:
- Decision scope and limits.
- Eligible participants and voting method.
- Proposal and execution process.
- Treasury controls and signer policy, if applicable.
- Conflict-of-interest and emergency procedures.

## 8. Security and operational commitments

The project will:
- Publish the exact verified mint through controlled channels.
- Never ask users for seed phrases or private keys.
- Avoid unofficial claim pages and wallet-connect prompts.
- Disclose known admin authorities and material wallet control where verifiable.
- Correct inaccurate repository claims through dated commits.
- Treat third-party audits as completed only when a public report and scope are available.

A repository, website, or social account is not a substitute for a smart-contract audit.

## 9. Roadmap principles

Roadmap milestones are subject to resources, platform rules, technical feasibility, and community decisions. The project will distinguish **planned**, **in progress**, **completed**, and **blocked** work. A milestone is completed only when evidence or a public deliverable is linked.

## 10. Risk factors

FUNGO may be illiquid, volatile, manipulated, or lose all market value. Risks include smart-contract and protocol changes, wallet compromise, phishing, concentrated holdings, market manipulation, failed launch objectives, platform downtime, regulatory uncertainty, and third-party infrastructure failure. See [RISK_DISCLOSURE.md](RISK_DISCLOSURE.md).

## 11. References

- [Pump protocol documentation](https://www.pumpdocs.fun/docs)
- [Pump.fun bonding curve documentation](https://x.preview.pump.fun/docs/bonding-curve)
- [Solscan mint lookup](https://solscan.io/account/3RWCQUsHN6gJR8saXHMhHa2pKTpJzy889CwUNBsEpump)
- [Solana Explorer mint lookup](https://explorer.solana.com/address/3RWCQUsHN6gJR8saXHMhHa2pKTpJzy889CwUNBsEpump)

Explorer links are lookup tools, not independent confirmation that the supplied address belongs to FUNGO.

## Disclaimer

This document is informational only and is not investment, legal, tax, or financial advice. Digital assets involve substantial risk. Do your own research and never risk funds you cannot afford to lose.