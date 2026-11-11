# FUNGO — Technical & On-Chain Verification

**Document status:** Operational specification  
**Last reviewed:** 2026-11-11  
**Network intent:** Solana mainnet  
**Launch venue:** Pump.fun  
**Graduation:** Not yet graduated, per project maintainer

## 1. Identity record

| Field | Value | Evidence status |
|---|---|---|
| Project | FUNGO | Project-maintained |
| Symbol | FUNGO | Project-maintained; metadata pending |
| Mint | `3RWCQUsHN6gJR8saXHMhHa2pKTpJzy889CwUNBsEpump` | User-supplied; verify account |
| Target supply | 1,000,000,000 | Target only |
| Decimals | — | Pending chain read |
| Token program | — | Pending chain read |
| Mint authority | — | Pending chain read |
| Freeze authority | — | Pending chain read |
| Metadata URI / update authority | — | Pending chain read |
| Bonding curve account | — | Pending |
| Curve completion state | Incomplete / not graduated | Maintainer-reported; verify live |
| PumpSwap pool | Not confirmed | Pending |

## 2. Required verification procedure

Before changing any status from pending:
1. Query Solana mainnet for the supplied address.
2. Confirm the account exists and is owned by the expected token program.
3. Decode the mint account and record decimals, raw supply, mint authority, and freeze authority.
4. Resolve token metadata and compare name, symbol, image URI, and update authority.
5. Locate the Pump.fun coin/bonding-curve state associated with this exact mint.
6. Read the curve completion / migration state from chain, not from screenshots or an unverified social post.
7. If graduated, identify the canonical PumpSwap pool and record its creation/migration transaction signature.
8. Record the observation timestamp and slot, plus links to the explorer account and transaction.

A ticker or token name is not a unique identifier. The mint address is the primary token identifier.

## 3. Lifecycle state machine

| State | Meaning | Evidence required |
|---|---|---|
| Address submitted | Mint string supplied by project maintainer | Maintainer record only |
| Mint verified | Valid mint account and metadata checked | Mainnet account + decoded mint |
| Bonding-curve trading | Associated Pump.fun curve is active | Curve account state + platform page |
| Curve complete | Graduation condition reached | On-chain curve state / completion transaction |
| Migrated | Liquidity migration transaction confirmed | Migration signature + pool account |
| Post-graduation trading | Canonical pool exists and is active | Pool state + swap transactions |

Current project reporting: **not graduated**. Do not infer curve progress or trading activity from this status alone.

## 4. Data dictionary for future public dashboard

| Metric | Definition | Publication rule |
|---|---|---|
| Total supply | Mint supply adjusted for decimals | Read directly from mint |
| Holder count | Distinct token accounts / owners, clearly defined | State methodology and snapshot slot |
| Top 10 concentration | Share of supply held by top 10 owners | Exclude or separately label protocol/LP/curve accounts |
| Largest holder | Largest owner balance share | Never identify a person from an address |
| Curve progress | Progress against current Pump.fun curve parameters | Use live program state; disclose calculation |
| SOL raised / reserves | Distinguish real reserves from virtual reserves | Never present virtual reserves as withdrawable liquidity |
| Market capitalization | Price multiplied by a stated supply basis | Label circulating vs fully diluted basis |
| Liquidity | Pool reserves and quote asset | Record pool address and timestamp |
| Volume | Trades over a stated interval | Name data provider and interval |
| Price | Quote from a named market and timestamp | Include pair and source |

## 5. Data quality and evidence standards

- Every live metric must include source, timestamp, and preferably Solana slot.
- Distinguish raw on-chain values from indexer-derived estimates.
- Do not mix virtual bonding-curve reserves with real token or SOL balances.
- Avoid reporting a market cap without explaining the supply basis and price source.
- Mark unavailable data as **N/A** rather than estimating.
- Preserve historical snapshots if publishing changes over time.
- Re-check status after material protocol changes.

## 6. Security notes

Never place private keys, seed phrases, API secrets, wallet JSON files, or signing credentials in this repository. Public wallet addresses may be published only when their role is clear and the project has authority to disclose that role. Use read-only RPC access for monitoring. Any transaction signing should occur in a trusted wallet with explicit human review.

## 7. Official technical references

- [Pump protocol docs](https://www.pumpdocs.fun/docs)
- [Pump.fun bonding curve overview](https://x.preview.pump.fun/docs/bonding-curve)
- [Solana Explorer](https://explorer.solana.com/)
- [Solscan](https://solscan.io/)