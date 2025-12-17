## Supported Tokens

This page describes the types of tokens supported by SafeSend. Token availability depends on the selected blockchain network and whether the token is included by default or added as a custom token.

SafeSend is currently optimized for stablecoin transfers but supports additional tokens through custom token configuration.

### Default Supported Tokens

SafeSend includes built-in support for commonly used stablecoins.

| Token | Symbol | Token Type |
|------|--------|------------|
| Tether USD | USDT | Stablecoin |
| USD Coin | USDC | Stablecoin |
| NodeOps Token | NODE | Utility Token |

Default tokens appear automatically in the token selector when the corresponding network is selected.

### Stablecoin Optimization

SafeSend is optimized for stablecoin transfers due to their frequent use in operational, treasury, and peer-to-peer transactions.

This optimization includes:

- Clear amount handling
- Predictable decimal behavior
- Improved transfer review and confirmation flows

Stablecoins are recommended for most SafeSend use cases.

### Custom Token Support

In addition to default tokens, SafeSend supports custom tokens.

Custom tokens:

- Can be added using a contract address
- Must be compatible with the selected network
- Appear in the token selector once added
- Behave the same as default tokens during transfers

Custom tokens allow SafeSend to support a wide range of ERC-20 or network-compatible tokens beyond the default list.

### Network Dependency

Token support is dependent on the selected blockchain network.

- Only tokens deployed on the selected network can be transferred
- Tokens cannot be transferred across networks
- Custom tokens must match the active network

For supported networks, see [Supported Networks](./3-supported-networks.md).

### Limitations

- SafeSend does not validate the legitimacy of token contracts
- Token metadata may be incomplete or unavailable for newly deployed tokens
- Unsupported token standards cannot be transferred

For additional constraints, see [Limitations](./0-limitations.md).

### Related Reference Pages

- [Supported Networks](./3-supported-networks.md)
- [Features](./1-features.md)
- [Security Considerations](./2-security.md)
