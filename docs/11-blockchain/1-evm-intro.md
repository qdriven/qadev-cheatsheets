# Ethereum Blockchain Intro

1. Introduction
    - Blockchain
    - World state
    - Account
    - Transaction
    - Message
    - Decentralised database
    - Atomicity and order
2. Virtual machine
    - Ethereum virtual machine (EVM)
    - Message call
    - Exception
    - Gas and fee
    - Input and output
    - Byte order
    - Instruction set
    - Miscellaneous
    - What is Ethereum blockchain?
    - BlockChain Conceptions
    - Ethereum EVM illustrated

exploring some mental models and implementations

## Ethereum Transaction/Block Conception

- Transaction:
  * Ethereum can be viewed as a transaction-based state machine. 
  * A transaction represents a valid arc between two states.

![img.png](1.png)

- Block And Transaction
  * Transactions are collated into blocks 
  * A block is a package of data.  
    
![img.png](2.png)

- Chain Of States: Blockchain
  * Ethereum can be seen as a state chain
  * Ethereum can also be seen as a chain of blocks, so it is `BLOCKCHAIN`  

![img.png](3.png)
![img.png](4.png)

- Ledger: Accounting
  * Ethereum can also be seen as a stack of transactions
    
![img.png](5.png)

## Blockchain World State

The world state is a mapping between address and account state

![img.png](6.png)

![img.png](7.png)

## Blockchain - Account

- General Account:

![img.png](8.png)

- Smart contract account:
An account state could contain EVM code and storage
![img.png](9.png)
  
![img.png](10.png)

- Address of Account: A 160-bit code used for identifying accounts

![img.png](11.png)

## Blockchain - Transaction

A transaction is a cryptographically-signed instruction
![img.png](12.png)

Two types of Transaction:
- Contract Creation
- Message Call

![img.png](13.png)
![img.png](14.png)
![img.png](15.png)
![img.png](16.png)

## Blockchain - Message

* Message:
    - Message is passed between two Accounts
    - Message is Data (as a set of bytes) and Value (specified as Ether)

![img.png](17.png)

Message Trigger:
    - Transaction trigger
    - EVM trigger

![img.png](18.png)
![img.png](19.png)

## Blockchain - Decentralised database
A blockchain is a globally shared, decentralised, transactional database.

- General Database:
 
![img.png](20.png)
  
- Decentralised database

![img.png](21.png)

## Blockchain - P2P network

Decentralised nodes constitute Ethereum P2P network

![img.png](22.png)

External actors access the Ethereum world through Ethereum nodes

![img.png](23.png)

## Blockchain - Atomicity and order

- A transaction is an atomic operation. Can't divide or interrupt.
That is, **All** (complete done) or **Nothing** (zero effect).

![img.png](24.png)

- Transactions cannot be overlapped. Transactions must be executed sequentially.

  
![img.png](25.png)
![img.png](26.png)
![img.png](27.png)

- Ordering inter block
The order between blocks is determined by a consensus algorithm such as PoW.
  
![img.png](28.png)

## Blockchain - virtual machine

The Ethereum Virtual Machine is the runtime environment for smart contracts in Ethreum
![img.png](img.png)


![img_1.png](img_1.png)
![img_2.png](img_2.png)

![img_3.png](img_3.png)

![img_4.png](img_4.png)
![img_5.png](img_5.png)
![img_6.png](img_6.png)

![img_7.png](img_7.png)
![img_8.png](img_8.png)
![img_9.png](img_9.png)
![img_10.png](img_10.png)

## Blockchain- Gas and Fee
![img_11.png](img_11.png)
![img_12.png](img_12.png
![img_13.png](img_13.png)

## Blockchain - Endian of Memory

![img_14.png](img_14.png)
![img_15.png](img_15.png)
![img_16.png](img_16.png)
![img_17.png](img_17.png)
![img_18.png](img_18.png)

![img_19.png](img_19.png)
![img_20.png](img_20.png)

## Blockchain - Code Generation

![img_21.png](img_21.png)
![img_22.png](img_22.png)

## Source Code

![img_23.png](img_23.png)
![img_24.png](img_24.png)
![img_25.png](img_25.png)
![img_26.png](img_26.png)
![img_27.png](img_27.png)

![img_28.png](img_28.png)
![img_29.png](img_29.png)
![img_30.png](img_30.png)
![img_31.png](img_31.png)
![img_32.png](img_32.png)
![img_33.png](img_33.png)
![img_34.png](img_34.png)
![img_39.png](img_39.png)
![img_35.png](img_35.png)

![img_36.png](img_36.png)
![img_37.png](img_37.png)
![img_38.png](img_38.png)

## Web3 and Geth Node

![img_40.png](img_40.png)
![img_41.png](img_41.png)
![img_42.png](img_42.png)
![img_43.png](img_43.png)
![img_44.png](img_44.png)

## Refereneces:
[E1] Ethereum Yellow Paper
ETHEREUM: A SECURE DECENTRALISED GENERALISED TRANSACTION LEDGER
https://ethereum.github.io/yellowpaper/paper.pdf
[E2] Glossary
https://github.com/ethereum/wiki/wiki/Glossary
[E3] White Paper
A Next-Generation Smart Contract and Decentralized Application Platform
https://github.com/ethereum/wiki/wiki/White-Paper
[E4] Design Rationale
https://github.com/ethereum/wiki/wiki/Design-Rationale
[E5] Ethereum Development Tutorial
https://github.com/ethereum/wiki/wiki/Ethereum-Development-Tutorial
[E6] Ethereum Introduction
https://github.com/ethereum/wiki/wiki/Ethereum-introduction
[E7] Solidity Documentation
https://media.readthedocs.org/pdf/solidity/develop/solidity.pdf
https://solidity.readthedocs.io/en/develop/
[E8] Web3 JavaScript app API for 0.2x.x
https://github.com/ethereum/wiki/wiki/JavaScript-API
[E9] ethereum/wiki Subtleties
https://github.com/ethereum/wiki/wiki/Subtleties#exceptional-conditions

[W1] Awesome Ethereum Virtual Machine
https://github.com/pirapira/awesome-ethereum-virtual-machine
[W2] Diving Into The Ethereum VM
https://blog.qtum.org/diving-into-the-ethereum-vm-6e8d5d2f3c30
[W3] Stack Exchange: Ethereum block architecture
https://ethereum.stackexchange.com/questions/268/ethereum-block-architecture/6413
[W4] Porosity 
https://www.comae.io/reports/dc25-msuiche-Porosity-Decompiling-Ethereum-Smart-Contracts.pdf

[C1] Go Ethereum
https://github.com/ethereum/go-ethereum
[C2] Solc (Solidity compiler)
https://github.com/ethereum/solidity
[C3] Mist (Ethereum Wallet)
https://github.com/ethereum/mist
[C4] MetaMask
https://github.com/MetaMask/metamask-extension
[C5] Remix
https://github.com/ethereum/browser-solidity
[C6] Truffle
https://github.com/trufflesuite/truffle