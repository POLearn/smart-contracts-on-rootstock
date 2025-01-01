## Rootstock Virtual Machines (RVM)

At the heart of Rootstock's architecture is the Rootstock Virtual Machine (RVM), which serves as the core of its smart contract platform. The RVM is designed to execute smart contracts across all full nodes in the Rootstock network. This execution process involves handling inter-contract communications, creating monetary transactions, and modifying the state of persistent contract memory, ensuring that the decentralized applications (dApps) running on Rootstock function smoothly and efficiently.

One of the standout features of the RVM is its compatibility with the Ethereum Virtual Machine (EVM) at the opcode level. This compatibility allows developers to seamlessly port Ethereum smart contracts to Rootstock without needing to rewrite code. As a result, the skills and tools used for Ethereum development can be directly applied to Rootstock, making it an attractive option for developers familiar with the Ethereum ecosystem. This interoperability not only simplifies the development process but also enhances the potential for cross-platform applications and integrations. RVM allows developers to use the same code, tools, and libraries as builders on Ethereum. 

## Two-way Peg
The two-way peg is a mechanism that allows the transfer of funds from one blockchain to a second blockchain/protocol (and vice versa) without demanding trust from third parties.

This mechanism locks the required amount of BTC on a multi-sig wallet, releases the equivalent amount of RBTC to the virtual machine, and sends it to your wallet.

To redeem the RBTC for BTC, the peg mechanism releases an amount to your Bitcoin wallet and locks an equivalent amount of RBTC from your wallet into the protocol reserve.

The locking and unlocking take no human intervention, which minimizes the risk of malicious interference. Instead, it’s done by a federation that must constantly audit the proper behavior of the protocol to ensure a secure flow of funds between Bitcoin and Rootstock chains. In exchange, members of the Federation are incentivized with fees generated from transactions happening via the RVM.