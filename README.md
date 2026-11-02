# Savings DAI

A tokenized wrapper around the DSR. Supports ERC4626. Share to asset conversions are real-time even if the pot hasn't been dripped in a while.

## Deployments

Commit `665879762f8b5df5d234463f45d1d6a49bd4fbeb` (no referral):

- [Mainnet](https://etherscan.io/address/0x83f20f44975d03b1b09e64809b757c47f942beea)
- [Goerli](https://goerli.etherscan.io/address/0xd8134205b0328f5676aaefb3b2a0dc15f4029d8c)

## Referral Code

The `deposit` and `mint` functions accept an optional `uint16 referral` parameter that frontends can use to mark deposits as originating from them. Such deposits emit a `Referral(uint16 indexed referral, address indexed owner, uint256 assets, uint256 shares)` event. This could be used to implement a revshare campaign, in which case the off-chain calculation scheme will likely need to keep track of any `Transfer` and `Withdraw` events following a `Referral` for a given token owner.

## Copyright

This code was created by hexonaut.
Since it should belong to the MakerDAO community the Copyright for the code has been transferred to Dai Foundation

## Audits

Audit reports are hosted on the auditors' public portfolio pages:

| Auditor | Report | Date |
| --- | --- | --- |
| Cantina | [Sky: Plasma SkyLink Bridge Deployment Validation](https://cantina.xyz/portfolio/10c453c8-321e-4f11-9466-7906ef39475c) | 2026-04-16 |
| Cantina | [Sky: Avalanche SkyLink Bridge Deployment Validation](https://cantina.xyz/portfolio/8deb51bb-909d-4419-a289-10c105e0269e) | 2026-04-02 |
| ChainSecurity | [MakerDAO Savings USDS](https://www.chainsecurity.com/security-audit/makerdao-savings-nst/) | 2024-09-30 |
| Cantina | [susds](https://cantina.xyz/portfolio/97f6afde-9776-4fd1-b8a2-57478d18e295) | 2024-09-17 |
| Cantina | [snst (updates)](https://cantina.xyz/portfolio/3c9937ad-8874-4509-a9c1-cf8997de803b) | 2024-08-24 |
| Cantina | [sdai snst](https://cantina.xyz/portfolio/9cff4d7b-b94c-4708-860e-f63f38e21148) | 2024-06-21 |
| ChainSecurity | [Oasis Savings DAI](https://www.chainsecurity.com/security-audit/oasis-savings-dai/) | 2023-05-08 |

ChainSecurity reports are cumulative: each portfolio page hosts the latest version of the report, which covers all previously reviewed versions.
