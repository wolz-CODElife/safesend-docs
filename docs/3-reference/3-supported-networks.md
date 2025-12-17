## Supported Networks

This page lists the blockchain networks currently supported by SafeSend. Transfers can only be executed on the networks listed below.

Network support may change over time as SafeSend adds or updates integrations.

### Supported Networks

| Network Name           | Native Token | Network Type | Description |
|------------------------|--------------|--------------|-------------|
| Ethereum               | ETH          | Mainnet      | Ethereum mainnet supports ERC-20 token transfers and is commonly used for widely adopted and high-value tokens. |
| Arbitrum One           | ARB          | Mainnet (L2) | Arbitrum One is an Ethereum Layer 2 network that offers lower fees and faster confirmations while maintaining Ethereum compatibility. |
| Binance Smart Chain    | BNB          | Mainnet      | Binance Smart Chain supports BEP-20 tokens and provides lower transaction fees and faster block times compared to Ethereum. |
| Base                   | ETH          | Mainnet (L2) | Base is an Ethereum Layer 2 network designed for scalable, low-cost transactions using ERC-20 compatible tokens. |
| Arbitrum Sepolia       | ETH          | Testnet      | Arbitrum Sepolia is a test network used for development and validation. Tokens on this network have no real-world value. |


### Network Selection Behavior

- Only tokens compatible with the selected network are available
- Network selection determines transaction fees and confirmation times
- Transfers cannot be executed across networks

Users must ensure that the selected network matches both the token and recipient address.

### Limitations

- Transfers are restricted to the networks listed above
- Unsupported networks cannot be added manually
- Network availability depends on external blockchain infrastructure

For additional constraints, see [Limitations](./0-limitations.md).

### Related Reference Pages

- [Features](./1-features.md)
- [Security Considerations](./2-security.md)
