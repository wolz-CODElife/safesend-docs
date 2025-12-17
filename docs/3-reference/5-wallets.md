## Supported Wallets

This page describes the wallet providers supported by SafeSend. Wallet connectivity is required to verify ownership, approve transfers, and execute transactions.

SafeSend supports both direct wallet integrations and a broad range of wallets through WalletConnect.


### WalletConnect Support

In addition to direct integrations, SafeSend supports wallets through WalletConnect.

- WalletConnect enables access to **510+ compatible wallets**
- Wallets can be connected using QR code or mobile deep links
- Availability depends on the wallet provider and device

Wallets connected via WalletConnect follow the same verification and approval flow as directly supported wallets.

### Wallet Selection Behavior

When connecting a wallet:

- Only one wallet can be connected at a time
- Wallet availability depends on the selected network
- Some wallets may prompt additional permissions or confirmations

SafeSend relies on the connected wallet for all cryptographic signing and approvals.

### Security Considerations

- SafeSend does not store private keys or seed phrases
- All signatures and approvals occur within the wallet provider
- Wallet security depends on the wallet application and device

For more details, see [Security Considerations](./2-security.md).

### Limitations

- Wallet availability may vary by browser or device
- Unsupported wallets cannot be connected manually
- WalletConnect availability depends on third-party infrastructure

For additional constraints, see [Limitations](./0-limitations.md).

### Related Reference Pages

- [Supported Networks](./3-supported-networks.md)
- [Supported Tokens](./4-supported-tokens.md)
- [Features](./1-features.md)
- [Security Considerations](./2-security.md)
