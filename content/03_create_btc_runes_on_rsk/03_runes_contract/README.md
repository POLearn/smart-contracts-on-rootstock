# Runes Mock Bridge Contract

The **RuneToken** contract is a versatile smart contract built on the Rootstock blockchain. It leverages the **ERC-1155 token standard**, making it capable of managing both fungible and non-fungible tokens within a single contract. These tokens, referred to as "Runes," play a vital role in decentralized applications (dApps) by allowing developers to create unique digital assets with custom functionality.

### Key Features of RuneToken

1. **ERC-1155 Standard Integration**  
   The RuneToken uses the powerful **ERC-1155** standard, which is designed to manage multiple token types—fungible, non-fungible, or even semi-fungible. This flexibility allows developers to build rich, multi-asset systems efficiently.

2. **Ownership Control 🔐**  
   By implementing the **Ownable** contract from OpenZeppelin, RuneToken restricts certain critical actions, such as minting and freezing tokens, to the contract owner. This ensures security and prevents unauthorized changes.

3. **Custom Metadata 🌐**  
   Each token in the RuneToken contract has a unique metadata URI. This URI typically points to off-chain resources (like images or descriptions) that provide additional context about the token.

### Why Runes Are Special on RSK and BTC

Runes on RSK are a groundbreaking evolution of NFTs, bridging the gap between ERC-1155 tokens on Ethereum and the Bitcoin ecosystem. While ERC-based NFTs have revolutionized digital ownership with their versatility and programmability, Runes take it a step further by combining the flexibility of Ethereum standards with the security and decentralization of Bitcoin, thanks to Rootstock (RSK)

### Quest: Deploying Rune Token on Rootstock 🎯

In this quest, you’ll deploy the **Rune Token** contract on **Rootstock** using the contract available on the **RSK Runes GitHub repository**. You can find it here: [RuneToken.sol on GitHub](https://github.com/rsksmart/rsk-runes/blob/main/contracts/RuneToken.sol).

![](https://raw.githubusercontent.com/POLearn/smart-contracts-on-rootstock/refs/heads/master/content/assets/images/load_contract.png)

![](https://raw.githubusercontent.com/POLearn/smart-contracts-on-rootstock/refs/heads/master/content/assets/images/rune_token.png)

To get started, you'll need to compile the contract using Solidity **v0.0.26**. Once the contract is compiled, you're ready to deploy it. When deploying, make sure to enter an `initialOwner` address, which should be the address you're using to deploy the contract.

![](https://raw.githubusercontent.com/POLearn/smart-contracts-on-rootstock/refs/heads/master/content/assets/images/deploy_rune.png)

Congrats 🎉! You've successfully deployed your Rune Token on Rootstock. You can now use it to mint both fungible and non-fungible tokens. Later, you'll learn how to **etch** Runes and bridge them using the RSK frontend. For more details on interacting with the Rune Token, check out the [RSK Runes GitHub Repository](https://github.com/rsksmart/rsk-runes).