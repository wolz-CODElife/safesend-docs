## Add a Custom Token

This guide explains how to add a custom token to SafeSend when the token you want to transfer does not appear in the default token list.

Use this guide when you need to send an ERC-20 or compatible token that is not automatically detected by SafeSend.

Before you begin, make sure that:

- Your wallet is connected and verified
- You are connected to the correct blockchain network
- You have the token contract address available

To find a token contract address, use a blockchain explorer (like Etherscan for Ethereum, BscScan for BNB Chain, or Solscan for Solana) by searching the token's name or symbol. You can also find it on the project's official website, CoinGecko/CoinMarketCap, or their social media (Twitter, Discord), but always verify the network. The address is a unique identifier for the token's smart contract on the blockchain, which is needed to add it to your wallet or to send/receive the token.

If you are new to SafeSend, start with the [Quickstart](../0-get-started/0-quickstart.md).


### Add a Custom Token

1. Open the **Safe Send** page in the SafeSend dashboard.
2. Click **Add Custom Token** below the token selection area.
3. Select a chain
4. Enter the token contract address.
5. Review the token details displayed by SafeSend, including:
   - Symbol
   - Decimals
   - Token name
6. Confirm the token to add it to your available token list.

Once added, the token becomes available for selection during transfers.


### Selecting a Custom Token for Transfers

After adding a custom token:

1. Select chain you added the custom token to.
2. Open the token selection dropdown.
2. Select the custom token from the list.
3. Continue configuring your transfer as usual.

Custom tokens behave the same as default tokens during the transfer flow.
> [!NOTE]
> - Custom tokens only show under the chain you add them to. 
> - Only add token contract addresses from trusted sources.
> - SafeSend does not validate the legitimacy of custom token contracts.
> - Incorrect or malicious contract addresses may result in failed transactions or loss of funds.

### When to Use Custom Tokens

Adding a custom token is useful when:

- The token is newly deployed
- The token is not widely indexed
- You are transferring project-specific or internal tokens


### Related Guides

- [Send Tokens Using SafeSend](./1-send-tokens.md)
- [How SafeSend Works](../0-get-started/1-how-safesend-works.md)
