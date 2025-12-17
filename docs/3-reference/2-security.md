## Security Considerations

This page describes the security model used by SafeSend and outlines how security-related responsibilities are shared between SafeSend, external services, and the user.

SafeSend is designed to reduce the likelihood of accidental or unintended token transfers while maintaining a non-custodial architecture.


### Non-Custodial Design

SafeSend does not take custody of user funds.

- Private keys and seed phrases are never collected or stored
- All signing and approvals occur within the user’s wallet
- SafeSend cannot initiate transactions without explicit user authorization

Users retain full control over their assets at all times.

### Wallet Signatures and Approvals

SafeSend relies on cryptographic signatures provided by the connected wallet.

- Verification signatures are used to confirm wallet ownership
- Token approvals are scoped to the exact transfer amount
- Approvals do not grant unlimited access to tokens

Users should always review wallet prompts carefully before approving any action.

### Scoped Token Approvals

Instead of requesting unlimited token allowances, SafeSend requests approval only for the specified transfer amount.

This approach:

- Reduces exposure in case of user error
- Limits the impact of accidental approvals
- Provides clearer visibility into what is being authorized

Approvals apply only to the configured transfer.

### External Confirmation via Telegram

SafeSend uses Telegram as an out-of-band confirmation channel.

This confirmation step:

- Requires explicit user approval outside the browser
- Helps protect against accidental clicks or automated submissions
- Adds a second verification layer before execution

Transfers will not execute unless confirmed through Telegram.

### Transaction Execution

After confirmation:

- Transactions are submitted directly to the blockchain
- Execution follows standard blockchain settlement rules
- SafeSend monitors transaction status but does not control settlement

Once submitted on-chain, transactions cannot be reversed or modified.

### Custom Token Security

When adding and using custom tokens:

- SafeSend does not validate token contract legitimacy
- Token metadata is retrieved from on-chain data when available
- Non-standard or malicious contracts may behave unexpectedly

Users should verify contract addresses using trusted block explorers before adding custom tokens.

### External Dependencies

SafeSend depends on third-party systems, including:

- Wallet providers for signing and approvals
- Blockchain networks for transaction execution
- Telegram for confirmation messaging

Issues with these services may affect SafeSend’s availability or behavior.

### User Responsibilities

While SafeSend adds verification layers, users remain responsible for:

- Verifying recipient addresses
- Selecting the correct network and token
- Reviewing transaction details before confirmation
- Securing access to their wallet and Telegram account

SafeSend does not protect against compromised wallets or accounts.

### Summary

SafeSend enhances transfer safety through scoped approvals, external confirmation, and explicit verification steps. These measures reduce common transfer errors but do not eliminate all risks associated with blockchain transactions. Users should understand and follow best practices when using SafeSend.
