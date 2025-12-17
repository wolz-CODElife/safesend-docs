## How SafeSend Works

SafeSend is designed to reduce the risk of irreversible token transfer mistakes by adding verification and confirmation steps before a transaction is executed on-chain. Instead of relying solely on a single wallet approval, SafeSend introduces multiple checkpoints that help ensure the sender’s intent matches the final transaction.

This page explains the core concepts behind SafeSend and how each part of the transfer flow contributes to safer token transfers.


### The Problem SafeSend Addresses

On most blockchain networks, token transfers are final. If tokens are sent to the wrong address, there is no built-in mechanism to reverse the transaction or recover funds.

Common causes of transfer errors include:

- Copying or pasting an incorrect wallet address
- Sending tokens on the wrong network
- Approving a transaction without fully reviewing details
- Human error during manual transfers

SafeSend is designed to reduce these risks without taking custody of user funds.


### High-Level Flow

At a high level, SafeSend works by separating a token transfer into distinct phases:

1. Wallet connection and identity verification  
2. Transfer configuration and approval  
3. External confirmation  
4. On-chain execution  

Each phase acts as a checkpoint before the next phase can proceed.


### Wallet Connection and Verification

SafeSend requires users to connect a Web3 wallet to initiate any action. This establishes the sender’s identity and enables SafeSend to request signatures and approvals.

After connecting a wallet, SafeSend requires a verification signature. This signature does not move funds. It is used only to confirm that the user controls the connected wallet address.

SafeSend never stores private keys or seed phrases. All signatures are generated locally within the wallet provider.

### Transfer Configuration

Once the wallet is verified, the user configures the transfer by selecting:

- The blockchain network
- The token to send
- The final transfer amount
- A test amount (optional)
- The recipient address

This separation between configuration and execution allows users to review transfer details before any on-chain action occurs.

### Approval-Based Transfers

Instead of requesting unlimited token approval, SafeSend requests approval for the exact transfer amount.

This approach:

- Limits the scope of token permissions
- Reduces the impact of accidental approvals
- Gives users clearer visibility into what is being authorized

The transfer cannot proceed unless the approval matches the specified amount.

### External Confirmation via Telegram

Before executing a transfer, SafeSend requires confirmation through an external communication channel.

Telegram is used as an out-of-band confirmation mechanism. This means the final confirmation occurs outside the browser and wallet interface.

This step helps protect against:

- Accidental clicks
- Compromised browser sessions
- Automated or unintended submissions

A transfer will not execute unless it is explicitly confirmed through Telegram.

### On-Chain Execution and Tracking

After confirmation, SafeSend submits the transaction to the blockchain.

Once submitted:

- The transaction is processed by the network
- SafeSend monitors confirmation status
- A transaction hash and block explorer link are provided

All transfers are recorded on-chain and can be independently verified using standard blockchain explorers.

### What SafeSend Does Not Do

SafeSend is not a custody service and does not:

- Hold user funds
- Control private keys
- Reverse or cancel on-chain transactions
- Modify blockchain settlement rules

SafeSend acts as a verification and coordination layer on top of existing blockchain networks.

### When to Use SafeSend

SafeSend is particularly useful when:

- Sending tokens to new or unfamiliar addresses
- Transferring large amounts
- Managing operational or treasury transfers
- Reducing human error in repetitive transfers

For step-by-step instructions to use SafeSend, see the [Quickstart](docs/0-get-started/0-quickstart.md) or the [Tutorials](docs/2-tutorials/0-first-safesend-transfer.md).

