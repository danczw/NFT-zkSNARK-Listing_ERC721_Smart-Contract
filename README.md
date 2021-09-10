# Property Title Smart Contract

This is a Ethereum based Smart Contract for decentralized property title listing. Users are able to mint their own token to represent their tutke ti the property. Therefore, proof of ownership is needed. zk-SNARKs are used to create a verification system which can proof the user has title to the property without revealing specific information on the property. Once the token is verified the user is able to place it on a bkockchain market place (OpenSea) for others to purchase.

---

## Setup

Setup for project development and related activities. The following resources have been used:

* [Remix - Solidity IDE](https://remix.ethereum.org/)
* [Truffle Framework](https://truffleframework.com/)
* [Ganache - One Click Blockchain](https://truffleframework.com/ganache)
* [Open Zeppelin ](https://openzeppelin.org/)
* [Interactive zero knowledge 3-colorability demonstration](http://web.mit.edu/~ezyang/Public/graph/svg.html)
* [Docker](https://docs.docker.com/install/)
* [ZoKrates](https://github.com/Zokrates/ZoKrates)

**Project Setup**

`npm install`

**ZoKrates Setup**

run ZoKrates via docker container to implement zkSnarks:

`docker run -v <path to project folder>/zokrates/code:/home/zokrates/code -ti zokrates/zokrates //bin/bash`

`zokrates compile -i code/square/square.code`

`zokrates setup`

`zokrates compute-witness -a 3 9`

`zokrates generate-proof`

`zokrates export-verifier`

a verifier.sol contract should be created to be used as zkSnark proof



---
###### *[part of my Blockchain Developer Nanodegree](https://www.udacity.com/course/blockchain-developer-nanodegree--nd1309)*
