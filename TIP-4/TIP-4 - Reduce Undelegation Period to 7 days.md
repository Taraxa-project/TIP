# TIP-4 - Reduce Undelegation Period to 7 Days

Author(s): Előd Varga [@vargaelod23](https://github.com/vargaelod23)

Created: 2024-11-11

Discussion: [https://discord.com/channels/419749122556297216/1305645251918168094](https://discord.com/channels/419749122556297216/1305645251918168094)
<br><br><br>

## Table of Contents

- [Summary](#summary)
- [Motivation](#motivation)
- [Specifications](#specifications)
- [Rationale](#rationale)
- [Copyright](#copyright)
  <br><br><br>

## Summary

This proposal aims to reduce the staking undelegation periods from the current 700540 blocks(~32 days) to 163459 blocks(~7 days). This will help to increase the staking participation by increasing constant staking ratios and the overall security of the network.
<br><br><br>

## Motivation

The existing 32-day undelegation period limits flexibility for stakers, creating a barrier to entry for users who prioritize liquidity. By reducing this period to 7 days, we aim to align with industry standards, improve user experience, and boost staking participation. A higher staking ratio will also strengthen the network’s security as more assets are committed to supporting consensus.
<br><br><br>

## Specifications

### Proposed Undelegation Period

The new undelegation period will be set to 163459 blocks (~7 days), replacing the current 700540 blocks (~32 days).
<br><br>

### Technical Implementation

This change will involve:

- Updating the staking contract to implement the new undelegation period.
- Running thorough tests to confirm stability and security with the new period.
- Conducting a security audit post-update to ensure the change does not expose the network to additional risks.
  <br><br>

### Rationale

A 7-day undelegation period was chosen as it strikes a balance between security and usability. Here’s why this timeframe is effective:

1. **Security and Staking Ratio Stability**: Shortening the unstaking period to 7 days aligns with or is close to other leading PoS networks. It allows users to participate without locking assets for an extended period, encouraging more participants and a stable staking ratio.

2. **Competitive Advantage**: Currently, many other EVM chains have adopted undelegation periods ranging from 3 to 7 days, which are appealing to users. By following this industry trend, Taraxa will maintain its appeal to both current and prospective stakers.

3. **User Demand for Liquidity**: Reducing the unstaking period supports users’ need for more flexible asset management. Meeting this demand can attract more validators, leading to a stronger, more secure network overall.

<br><br>

### Undelegation Periods Across EVM Chains

| Blockchain          | Undelegation Period | Notes                                                                            |
| ------------------- | ------------------- | -------------------------------------------------------------------------------- |
| Ethereum            | ~5 days             | Since the Shanghai upgrade, staked ETH can be withdrawn in approximately 5 days. |
| Binance Smart Chain | 7 days              | Utilizes PoSA (Proof of Staked Authority) with a 7-day undelegation period.      |
| Fantom              | 7 days              | High-performance EVM-compatible chain with a 7-day period.                       |
| Moonbeam            | 7 days              | Operates on Polkadot with EVM compatibility and has a 7-day period.              |
| Avalanche           | 2-52 weeks          | Users select staking duration; unstaking period depends on chosen lock-in.       |
| Harmony             | 7 days              | Features a ~7-day unstaking period to maintain flexibility and security.         |
| Celo                | ~3 days             | A shorter period to ensure liquidity and retain user interest in staking.        |

### Summary

Reducing the undelegation period aligns Taraxa with other EVM PoS chains, meeting market standards for flexibility while maintaining security. EVM chains that use similar durations have managed to balance high staking ratios and liquidity, thereby enhancing network security through more extensive validator participation. Implementing a 7-day period would therefore make Taraxa more competitive by addressing user needs for both security and accessible liquidity, fostering higher staking rates and a more secure network overall.
<br><br>

## Copyright

All Taraxa Improvement Proposals follow the same [license](https://github.com/Taraxa-project/TIP/blob/main/LICENSE).
