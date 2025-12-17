## Features

This page provides an overview of the features available in SafeSend. It is intended as a reference for understanding what functionality the platform offers and how features relate to one another.

### Safe Send

The Safe Send feature is the primary interface for creating token transfers.

It allows users to:

- Select a blockchain network
- Choose a token
- Specify one or more recipients
- Configure transfer and test amounts
- Review transfer summaries before execution

Safe Send coordinates approvals, confirmations, and execution as part of a single transfer flow.

### Multiple Recipients

SafeSend supports sending tokens to multiple recipients within a single transfer configuration.

This feature:

- Allows adding multiple recipient entries
- Calculates the total transfer amount automatically
- Handles distribution to recipients during execution

Each recipient entry includes an address, transfer amount, and optional test amount.

### Transaction History

Transaction History displays past and pending transfers.

For each transfer, it provides:

- Transfer status
- Token and network information
- Recipient details
- Transaction hash and block explorer links

Transaction History reflects on-chain data and updates as confirmations are received.

### Address Book

The Address Book allows users to store and reuse wallet addresses.

This feature helps:

- Reduce manual address entry
- Minimize copy-and-paste errors
- Speed up repeat transfers

Stored addresses can be selected during transfer configuration.

### Custom Tokens

SafeSend supports adding tokens that are not included in the default token list.

Custom token functionality includes:

- Adding tokens by contract address
- Displaying token metadata when available
- Selecting custom tokens during transfers

SafeSend does not validate the legitimacy of custom token contracts.

### Token Management

Token Management provides tools for managing custom tokens.

Users can:

- View all added custom tokens
- Review token metadata and associated networks
- Remove custom tokens from the token list

Removing a token does not affect wallet balances or on-chain assets.

### Wallet Verification

SafeSend requires wallet verification before transfers can be initiated.

This feature:

- Confirms ownership of the connected wallet address
- Uses cryptographic signatures
- Does not move or lock funds

Verification must be completed before transfer configuration.

### Telegram Confirmation

Telegram confirmation is used as an external verification step.

This feature:

- Sends transfer details to Telegram
- Requires explicit user confirmation before execution
- Acts as an out-of-band safeguard against accidental transfers

Transfers cannot be executed without Telegram confirmation.

### Profile

The Profile section allows users to manage account-related settings.

Available options include:

- Connecting or disconnecting Telegram
- Viewing wallet-related information

Profile settings affect how confirmations and notifications are handled.


### Related Reference Pages


- [Limitations](./0-limitations.md)
- [Security Considerations](./2-security.md)
