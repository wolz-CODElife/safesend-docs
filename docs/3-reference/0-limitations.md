## Limitations

This page describes functional and operational constraints of SafeSend. Understanding these limitations helps set correct expectations when using the platform for token transfers.

SafeSend is designed to reduce transfer errors, not to eliminate all risks associated with blockchain transactions.

### Irreversible Transactions

Blockchain transactions are final once confirmed on-chain.

SafeSend cannot:

- Reverse completed transactions
- Recover funds sent to incorrect addresses
- Cancel transactions after on-chain submission

Users are responsible for verifying all transfer details before confirmation.

### No Custody of Funds

SafeSend is a non-custodial application.

SafeSend does not:

- Hold user funds
- Control private keys
- Store seed phrases or wallet credentials

All transactions are authorized and signed directly through the user’s wallet.

### Network and Token Support

SafeSend is limited to supported blockchain networks and token standards.

Limitations include:

- Transfers are only supported on networks enabled in SafeSend
- Unsupported tokens cannot be transferred unless added as custom tokens
- Token metadata may be incomplete or unavailable for newly deployed tokens

Support for networks and tokens may change over time.

## External Dependencies

SafeSend relies on third-party services and protocols.

These include:

- Wallet providers for signing and approvals
- Blockchain networks for transaction execution
- Telegram for out-of-band confirmation

Availability or performance issues in these services may impact SafeSend functionality.

### Custom Token Risks

When using custom tokens:

- SafeSend does not verify contract legitimacy
- Incorrect contract addresses may result in failed transactions
- Malicious or non-standard tokens may behave unexpectedly

Users should verify token contracts through trusted sources before adding them.

### User Responsibility

SafeSend reduces common transfer mistakes but does not replace user diligence.

Users remain responsible for:

- Verifying recipient addresses
- Selecting the correct network and token
- Confirming transaction details before execution

### Feature Availability

Certain features may be unavailable due to:

- Network congestion
- Temporary maintenance
- Feature rollouts or deprecations

SafeSend does not guarantee uninterrupted availability of all features at all times.


### Related Reference Pages

- [Features](./1-features.md)
- [Security Considerations](./2-security.md)
