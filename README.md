# Mayank0307-udacity-cryptostar-ethereum-dapp
This project is part of the Udacity Blockchain Nanodegree. In this project, a DAPP was created to create ERC 721 tokens associated with a Star name (CryptoStar). A user can mint a ERC 721 token with a given star name and tokenId. The DAPP smart contract inherits from the Openzeppelin ERC721.sol. The tokens are assigned a token name and a token symbol in the DAPP smart contract. The following functionality was added to the DAPP smart contract:
* Function createStar() - Creates a new Star using the provided star name and tokenID. This function calls the openZeppelin ERC721.sol _mint() function to create the token and assign the ownership to the msg.sender. 
* Function putStarUpForSale() - The owner of a token can use this function to put a star for sale by providing the tokenId and the sale price. 
* Function buyStar() - The function can be used to buy a star from an owner. The tokenId is transfered to the new owner.
* Function lookUptokenIdToStarInfo() - that looks up the stars using the Token ID, and then returns the name of the star.
* Function exchangeStars() - so 2 users can exchange their star tokens
* Function transferStar() - The function transfers a star from the address of the caller to a different address. The function    accepts 2 arguments, the address to transfer the star to, and the token ID of the star.

Truffle webpack was used to develop the code for this project. The functionality of the smart contract was tested using Mocha unit tests. The smart contract was then deployed to the Rinkeby test network using Metamask Wallet and Infura node. The front end of the DAPP was modified to create a new star and the corresponding ERC 721 tokenId. The front end was also modified so that a user can Lookup a star by ID using tokenIdToStarInfo() function.

## deployed smart contract address on rinkeby test network:

Starting migrations...
======================
> Network name:    'rinkeby'
> Network id:      4447
> Block gas limit: 6721975 (0x6691b7)


1_initial_migration.js
======================

   Replacing 'Migrations'
   ----------------------
   > transaction hash:    0xf2b0a726be118eb1a51dd25fc814affd93abadd223eb91a8e485f4971ebb2dba
   > Blocks: 0            Seconds: 0
   > contract address:    0x5F61204D91437181b9aB7E0A77b9d9072A8d7D44
   > block number:        5
   > block timestamp:     1591721958
   > account:             0x09E08B1888DD04C24814dE9881A31A2D0a799124
   > balance:             99.98701098
   > gas used:            188483 (0x2e043)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00376966 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00376966 ETH


Summary
=======
> Total deployments:   1
> Final cost:          0.00376966 ETH
## General Information
ERC-721 Token Name - Crypto Star

ERC-721 Token Symbol - CST

Version of the Truffle used - v5.0.18

Version of OpenZeppelin used - 2.1.2
