# Understanding the `mintFungible` Function

The `mintFungible` function is a crucial part of the Runes Mock Bridge Contract, allowing the contract owner to create and distribute fungible tokens. This function ensures that tokens are minted in a structured and secure manner, adhering to predefined limits and rules. Let’s break down how it works and why each step is important.

![](https://raw.githubusercontent.com/POLearn/smart-contracts-on-rootstock/refs/heads/master/content/assets/images/mint_fungible_implementation.png)

- **Ensuring Supply Limits** - 
Before creating tokens, the function performs a critical check to confirm that the **initial supply** does not exceed the maximum supply limit (`maxSupply`). This step is essential to prevent over-minting, which could lead to inflation or disrupt the intended tokenomics of the system.
- **Generating a Unique Token ID** - 
Each fungible token is identified by a **unique token ID**, which the function generates by hashing the `runeName` using the `keccak256` algorithm. This ensures that every token type is distinct. To maintain this uniqueness, the function verifies that no other token with the same ID exists before proceeding.
- **Storing Token Information** - 
Once a unique token ID is established, the function saves all the relevant token details—such as its URI, name, symbol, maximum supply, and other properties—in a dedicated mapping called `_tokenInfos`. This stored information serves as the official record for the token, ensuring that its details are easily retrievable for various contract interactions.
- **Minting the Tokens** - 
The function then mints the tokens, allocating the specified **initial supply** to the receiver’s wallet address. This process creates the token on the blockchain, making it part of the Runes ecosystem and available for use.
- **Tracking Ownership** - 
Finally, the function updates the system’s ownership records by adding the minted token to the receiver’s list of owned tokens. This is done using the `_addUserToken` method, which ensures accurate tracking of token ownership for both individual users and broader dApp functionality.

The `mintFungible` function enables the secure and efficient creation of fungible tokens. It ensures that token generation adheres to the rules set by the contract, providing both transparency and reliability in the Runes ecosystem. 

### Quest: Minting a Fungible Rune Token 🎯

Using your RuneToken deployed in RSK, you can mint a fungible token. Let's provide these are the arguments for the method  

- `0x` represents an empty URI.  
- `POLNFTRune` is the name of your token (runeName).  
- `POR` is the token symbol.  
- `100` specifies the initial supply of the token.  
- `0` indicates the token type (use `0` for fungible).  
- `1` is the maximum supply for the token.  
- `0xA327f039b95703fa84D507e7338FB680D2BEf447` is the wallet address to receive the minted tokens.  

Enter these values into the respective fields of the `mintFungible` function in your dApp interface.  

![](https://raw.githubusercontent.com/POLearn/smart-contracts-on-rootstock/refs/heads/master/content/assets/images/mint_fungible_params.png)

Once done, submit the transaction and confirm it in your wallet. Wait for the transaction to complete, and your fungible token will be minted successfully on-chain. This completes your quest!  

> Note, the above minter address is one of (POL) addresses and is used as a placeholder for this quest. In a real application, this should be replaced with the designated address for receiving the Rune.