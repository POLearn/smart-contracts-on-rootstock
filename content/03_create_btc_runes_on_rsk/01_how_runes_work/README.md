# How Runes Function on Rootstock

Bitcoin Runes build upon two powerful elements of the Bitcoin network: its UTXO (Unspent Transaction Output) model and the OP_RETURN opcode. Let's break down how these concepts work and how they play a crucial role in the Runes ecosystem.

### The UTXO Model: Tracking and Managing Assets

Bitcoin's UTXO model serves as the foundation for tracking assets on the network. Every time a Bitcoin transaction occurs, it is broken down into individual outputs, called UTXOs. Think of a UTXO like a digital coin in your wallet — it holds a specific amount of Bitcoin, and when you spend it, any leftover amount becomes a new UTXO. 

For example, if you had 2 Bitcoin Runes in your wallet and wanted to send 1 Rune to a friend, the UTXO would be divided into two parts: one part sends 1 Rune to your friend, and the other keeps the remaining Rune for you. This system allows the network to easily track how many Runes each address holds, making it possible to transfer and manage them across the Bitcoin blockchain.

### OP_RETURN: Embedding Data into Transactions

In the Bitcoin network, transactions typically consist of transferring Bitcoin from one address to another. But with the `OP_RETURN` opcode, you can attach additional information to a transaction — up to 80 bytes of data. This data can include essential details about Runes, such as their name, symbol, and unique identifier. 

This extra information is stored in what’s known as a "Runestone," embedded in the `OP_RETURN` field of the transaction. The Runestone essentially describes the Rune and its properties, allowing the network to understand the specifics of each token. For example, a Runestone might tell the network that a Rune of Power is being transferred from one user to another.

This use of OP_RETURN allows Runes to store important information such as:
- The **name** of the Rune (e.g., "Sample Rune")
- The **token ID**, which is a unique identifier
- **Commands** that dictate what should happen to the Rune (e.g., minting or transferring)

### Why Choose Bitcoin Runes?

The combination of Bitcoin’s robust security and the OP_RETURN opcode allows Runes to be created and managed without relying on a separate blockchain. This makes Runes both secure and simple to use, as they leverage the Bitcoin network’s already established transaction system.

Runes are created, or "etched," and then minted into users’ wallets, allowing them to be transferred or traded directly on the Bitcoin network. By using Bitcoin’s existing infrastructure, Runes benefit from Bitcoin’s strong security and widespread adoption, making them a reliable and efficient way to manage tokens on the blockchain.