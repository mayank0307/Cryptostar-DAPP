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
> Network id:      4
> Block gas limit: 10000000 (0x989680)


1_initial_migration.js
======================

   Replacing 'Migrations'
   ----------------------
   > transaction hash:    0xf5d0b764211abb779e64d710b0528a228cc112967f5b76527223fa15569707b8
   > Blocks: 1            Seconds: 21
   > contract address:    0x967c421a8aC9A92cBFCa2dbb384b116968D85eaC
   > block number:        6641080
   > block timestamp:     1591771670
   > account:             0x0fc48086421D32A05F4101C4aB13cdD51112dDaE
   > balance:             9.94446043
   > gas used:            225441 (0x370a1)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00225441 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00225441 ETH


2_deploy_contracts.js
=====================

   Replacing 'StarNotary'
   ----------------------
   > transaction hash:    0x8794783a02b7cf7db36fd338aea45b78372bb29f649e37f7b2d4dd9390ded1cd
   > Blocks: 0            Seconds: 9
   > contract address:    0x3EFD279A901100e7c68AfC3035F2c94cEbef00D1
   > block number:        6641082
   > block timestamp:     1591771700
   > account:             0x0fc48086421D32A05F4101C4aB13cdD51112dDaE
   > balance:             9.91247331
   > gas used:            3156349 (0x30297d)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.03156349 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.03156349 ETH


Summary
=======
> Total deployments:   2
> Final cost:          0.0338179 ETH

## General Information
ERC-721 Token Name - Crypto Star Awsome

ERC-721 Token Symbol - CSTA

Version of the Truffle used - v5.1.27

Version of OpenZeppelin used - 2.1.2
