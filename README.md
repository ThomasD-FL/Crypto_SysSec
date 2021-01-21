# Crypto_SysSec
Anonymizing crypto currency transactions

In this project we will analyze ways to anonymize crypto currency transactions using zero knowledge proofs.
1. Step: Understanding smart contracts

To enter the world of crypto-currencies, we have designed our own Smart Contract in Solidity as a first step. Our newly invented currency is called "FlensCoin". With the help of the Solidity-IDE "Remix" you can test our created contract (flenscoin.sol). For testing on a test network you will need to install the MetaMask Chrome extension which allows using several testing networks.
The next task we set up our own blockchain was created on a virtual machine under the operating system ubuntu 20.4. A private test Ethereum blockchain was set up and started.
the following programs were installed geth (Go Ethereum) and solc(Solidity Compiler). To start your own private test Ethereum blockchain, manual initialization of the first Genesis block is required.
With the command geth we generate Genesis-Block.json
 geth --datadir "Flens-arena" init src/genesis-block.json
 An account was also created and mining was started manually.Then a simple Solidity script for an Ethereum Smart Contract was created, compiled and deployed.
