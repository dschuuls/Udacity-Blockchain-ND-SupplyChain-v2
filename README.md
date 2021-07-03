# Udacity-Blockchain-ND-SupplyChain-v2

I had to deploy on the Ropsten testnet because I can't receive enough ETH from faucets to deploy on Rinkeby!

Contract address: 0x7161e63F43810DFB8a315a33EB456A74a756eCD8

Transaction hash: 0xbf0ddb7bd1a51d10b98d4b87fe34669d05d82a922ecc3fd6daede9abe7de508e

https://ropsten.etherscan.io/address/0x7161e63F43810DFB8a315a33EB456A74a756eCD8

truffle 5.3.11,
compiler 0.4.24,
node 10.21.0,
web3 1.4.0

I replaced the truffle-contract.js file in /src/js with the latest version (4.0.31) from here: https://www.jsdelivr.com/package/npm/truffle-contract?path=dist.

I also put the latest web3.min.js file from the node_modules folder to /src/js.

Find my diagrams in /diagrams.

## About

### Motivation

Buying things like food or coffee, many people want to make sure it's produced ethically. How can consumers trust the product they buy? How can they be sure everything from harvesting, processing, packing and shipping is undergoing fair conditions for everybody involved?  
By having a blockchain solution, the consumer can now check every single step along the lifecycle of what's sitting in the shelves of the store where they buy their stuff. 

### Diving deeper

This project is a simple supply chain solution backed by the Ethereum blockchain. It uses smart contracts that let users track and verify the authenticity of the coffee as it changes its states along the supply chain. Specific user permission controls have been implemented to allow different roles to interact with the smart contract.

### Role overview

Farmer role: Can harvest coffee, process and pack it and put it up for sale.

Distributor role: Can buy coffee from a farmer and ship it to a retailer.

Retailer role: A retailer can receive coffee which was sent out by a distributor.

Consumer role: A consumer can purchase some coffee, after it reached the retailer.

All the described roles have been implemented as separate smart contracts. The base contract inherits from them.

### Architecture

To get more information about the architecture of this small project be sure to take a look at the UML diagrams in /diagrams.

### Simple Web UI

The provided Web UI is nothing fancy. It provides enough functionality to showcase the potential that this technology has though.
