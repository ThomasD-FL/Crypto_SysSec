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

2. Understanding crypto currency

Nonce: In cryptography, the term nonce was taken up to designate a combination of numbers or letters that is only used once in the respective context. Typical ways of generating a nonce are the use of (cryptographically secure) random values that are sufficiently large so that the probability of double use is negligible (see birthday paradox),

Transaction: Each node in the peer-to-peer network acts as a register and trustee who carries out changes of ownership and automatically maps verifiable rules about these transactions. All transactions are always audited by all other nodes.

If a participant now wants to transfer an amount to an account, he creates a transfer order with the amount and the public key of the target account and signs this order with his secret key. This order is published via the P2P network. It now has to be checked and certified and archived as a transaction in the joint accounting.

The steps in the operation of a decentralized cryptocurrency are:
1. New transactions are signed and sent to all nodes.
2. Each node collects new transactions in a block.
3. Each node looks for the nonce that validates its block.
4. When a node finds a valid block, it sends the block to all other nodes.
5. The nodes only accept the block if it is valid according to the rules:

    a. The hash value of the block must correspond to the current level of difficulty.
    
    b. All transactions must be correctly signed.
    
   c. The transactions must be covered in accordance with the previous blocks (no double spending).
   
   d. New issue and transaction fees must conform to the accepted rules.
   
6. The nodes express their acceptance of the block by adopting its hash value in their new blocks.

