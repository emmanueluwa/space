---
layout: "../../layouts/BlogPost.astro"
title: Third Blog Post
date: 2022-11-23
draft: true
---

Solidity

- Here are the docs for solidity, the high level language used to implement and interact with smart contracts, https://docs.soliditylang.org/en/v0.8.13/
- Solidity is influenced by mainly C++, Python and Javascript.
- Each contract written can be seen as a class in object-orientated programming, for this reason inheritance can be used for a contract to inherit all functions of another contract.
- Calling a function in a contract or making a state(current data) change to the EVM, counts as a transaction which costs gas fees.
- A view function, allows for the state from the blockchain to be read, this is not a transaction and therefore has no fee.
- A require function, if a condition is not met, execution is reverted and the users money will be returned.
- Transfer function, allows us to send eth from one address to another.
- In solidity there are two main ways to store information:

In memory, which occurs during execution and is deleted after.

In storage, which is stored before and after execution.

Smart contracts

- Two things needed when interacting with smart contracts,

1. Address of the contract

2. ABI, Application Binary Interface of the contract
   For further reading: https://docs.soliditylang.org/en/v0.8.13/abi-spec.html#:~:text=The%20Contract%20Application%20Binary%20Interface,as%20described%20in%20this%20specification.

- Smart contracts are immutable by default in Ethereum. It is the logic of the contract that is stored on the blockchain forever. For a developer it is not common that changes will need to be made after deployment, this is possible with smart contracts but has decentralisation implications.
- There is more than one way to make changes to a smart contract, each of which have pros and cons:

1. Parameterize method
2. Migration method (for example, version 1 to version 2) for more: https://blog.trailofbits.com/2018/10/29/how-contract-migration-works/
3. The proxies method (using low level functionality) for more: https://blog.trailofbits.com/?s=proxies&submit=Search
   Development/Test suites

- Infura.io, a development suite for testing. For more: https://infura.io/
- Brownie, a python-based contract development and testing platform. The platform relies on web3.py, for more: https://eth-brownie.readthedocs.io/en/stable/
- Brownie offers mainnet-forking, which allows us to fork smart contracts that have been deployed to the Ethereum mainnet, as a result of this we can test these smart contracts locally. For more on mainnet: https://ethereum.org/en/enterprise/
- Alchemy.io, development platform for building scalable and reliable decentralised applications, for more on alchemy: https://www.alchemy.com/
- Openzepplin, amongst other things they offer templates to help get started with smart contracts. For more: https://www.openzeppelin.com/
