# What are Bitcoin Runes?

Bitcoin Runes are a new protocol designed to enable more advanced functionality on the Bitcoin blockchain. Built on the concept of **Bitcoin Script**, Runes offer a more flexible and expressive syntax, allowing developers to implement complex conditions within Bitcoin transactions. This enhanced programmability allows Bitcoin to support use cases beyond simple value transfers, making it more versatile and developer-friendly for various applications like fungible tokens, smart contracts, and decentralized finance (DeFi).

### How Bitcoin Runes Work

Bitcoin Runes enable developers to encode **smart contract logic** directly into Bitcoin transactions. They allow for conditions such as:

- **Multi-signature requirements**: Transactions that require multiple parties to authorize.
- **Time-locks**: Locks that prevent funds from being accessed until a specific time or block height.
- **Conditional payouts**: Payouts that are made only if certain conditions are met.

Unlike Bitcoin Script, which is low-level and challenging to work with, Runes provide a more **readable** and **user-friendly** way to create these complex conditions, making them a powerful tool for developers looking to build sophisticated systems directly on Bitcoin.

### The History of Bitcoin Runes

The breakthrough came in December 2022 with the launch of the Ordinals protocol by Casey Rodarmor. Ordinals tracked individual satoshis (the smallest unit of Bitcoin) to create NFTs on Bitcoin, offering a mechanism for inscribing data onto each satoshi. While Ordinals created true NFTs on Bitcoin, the protocol introduced scalability issues by generating large amounts of on-chain data, which burdened the Bitcoin network and led to slow transactions and high fees.

While Ordinals demonstrated how NFTs could be utilized on Bitcoin, the need for a scalable solution for fungible tokens remained unmet. Enter BRC-20, a standard proposed by a pseudonymous developer, Domo, in March 2023. BRC-20 built on the Ordinals framework to introduce a fungible token standard on Bitcoin. However, as it was based on a data-heavy protocol, it faced similar scalability issues, putting significant strain on the Bitcoin network.

Casey Rodarmor proposed a new solution: Runes, a UTXO-based (Unspent Transaction Output) protocol for creating fungible tokens directly on the Bitcoin blockchain. Runes were designed to address the network congestion and inefficiencies of previous token protocols by utilizing Bitcoin’s native UTXO model in a more efficient and lightweight way. This new protocol allowed for the creation of fungible tokens without the heavy on-chain data load that had plagued Ordinals and BRC-20.

The first Rune was created on Block 840,000 in April 2024, following Bitcoin’s highly anticipated halving event, marking the beginning of a new chapter for tokenization on Bitcoin. Unlike previous approaches, Runes are designed to be far more scalable and efficient, making them a promising tool for developers and users seeking to build and trade fungible tokens on the Bitcoin network without overwhelming its infrastructure.