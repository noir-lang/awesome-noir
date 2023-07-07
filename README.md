# Awesome Noir

A curated list of resources for learning and programming in Noir.

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Noir.svg?style=social&label=Follow%20%40Noir)](https://twitter.com/NoirLang)
[![Discord](https://img.shields.io/discord/563037431604183070?logo=discord)](https://discord.gg/aztec)

## Contents

- [Official Resources](#official-resources)
- [Learning](#learning)
  - [Learning by Doing](#learning-by-doing)
  - [Talks & Workshops](#talks--workshops)
  - [Blog Posts & Articles](#blog-posts--articles)
- [Get Coding](#get-coding)
  - [Dev Tools](#dev-tools)
  - [Boilerplates](#boilerplates)
  - [Libraries](#libraries)
- [Projects](#projects)
  - [Authentication](#authentication)
  - [Gaming](#gaming)
  - [Governance](#governance)
  - [Social](#social)
- [Contribute](#contribute)

---

## Official Resources

- [Docs](https://noir-lang.org/)
- [GitHub](https://github.com/noir-lang/noir)
- [Forum](https://discourse.aztec.network/c/noir/7)
- [noir-starter repo](https://github.com/noir-lang/noir-starter)

## Learning

### Learning By Doing

- [Practice Exercises] [Noir-by-example](https://noir-by-example.org/)
  - An introduction to Noir with a bunch of simple examples 
  - Learn how to organize your Noir logic, write For Loops, and create complex package structures  
- [Video Series] [BattleZips-Noir](https://www.youtube.com/playlist?list=PLWACGbvIsEgnR2aUCr9i-PpmTVhF5Zuik) ([Source Code](https://github.com/BattleZips/BattleZips-Noir))
  - Walkthrough of building an on-chain Battleships game using zero-knowledge
  - Follow along and build your own game using Noir
- [Practice Exercises] [Circuit Examples](https://github.com/thor314/circuit-examples)
  - Demonstration of dot products & Merkle proofs in Noir, in comparison to Circom and RISC0
  

### Talks & Workshops

- [10 mins] [Writing Circuits with Noir](https://www.youtube.com/watch?v=I5M8LhOECpM&t=2879s) ([Source Code](https://github.com/vezenovm/basic_mul_noir_example))
  - Nargo setup
  - Basic Noir syntax
  - Noir interactions in TypeScript
- [20 mins] [Painless Zero-Knowledge Circuitry with Noir at ETHDam](https://www.youtube.com/watch?v=5KLTroMcldg&list=PLc5OGwyCUIhXny_mY4NPE5JfYNcTh8jUs&index=28)
  - Introduction to Noir
  - Simple demo and test
- [20 mins] [Private Value Transfer in 10 Lines](https://www.youtube.com/watch?v=wYqqXas8_O4) ([Source Code](https://github.com/vezenovm/simple_shield))
  - Tornado-like private asset transfer using Merkle proofs
- [25 mins] [Noir as a Smart Contract Language](https://www.youtube.com/watch?v=tYdUaCbACtk)
  - Noir as the smart contract language for the Aztec rollup
  - Noir smart contracts
- [1 hr] [Circuit Safety and an Introduction to Noir](https://www.youtube.com/watch?v=rLvu61DA-hk)
  - Common circuit bugs
  - Proving system vulnerabilities
  - Unconstrained functions
- [1 hr] [Introduction to Noir in Spanish](https://www.youtube.com/watch?v=m4P-sAqa8_o) ([Written Tutorial and Code](https://dev.to/turupawn/circuitos-de-aztec-noir-en-tu-navegador-zk-es-semana-3-78a))
- [1.5 hrs] [Sudoku in Noir](https://drive.google.com/file/d/1D4XCdiIZVjUW1JHDoMW3pG-15mgjMm9E/) ([Source Code](https://github.com/guipublic/crypdoku))
- [2 hrs] [ZK HACK III - Introduction to Noir](https://www.youtube.com/watch?v=5CziMfChveY) ([Souce Code](https://github.com/joss-aztec/quadratic_voting_noir))
  - Code-together: Quadratic Voting

### Blog Posts & Articles
- [Understanding the Technical Aspects of Aztec and Noir](https://hackmd.io/XZX9_pZ8Q1aa_ySDPeQopg)

## Get Coding

### Dev Tools

- [Noir Editor](https://noir-lang.github.io/noir-cra/)   - Browser IDE ([Souce Code](https://github.com/noir-lang/noir-cra))
- [VSCode Extension](https://marketplace.visualstudio.com/items?itemName=noir-lang.noir-programming-language-syntax-highlighter) - Syntax highlight ([Source Code](https://github.com/noir-lang/vscode-noir))
- [Vim Plugin](https://github.com/Louis-Amas/noir-vim-support) - Syntax highlight
- [Emacs Plugin](https://melpa.org/#/noir-mode) - Syntax highlight ([Source Code](https://github.com/hhamud/noir-mode))
- [hardhat-noir](https://www.npmjs.com/package/hardhat-noir) - Hardhat plugin ([Source Code](https://github.com/spalladino/hardhat-noir))

### Boilerplates

- [nplate](https://github.com/whitenois3/nplate) - Minimalist template
- [noir-hardhat-template](https://github.com/hooperben/noir-hardhat-template) - Hardhat template
- [noir-starter](https://github.com/noir-lang/noir-starter) - Template repository containing example projects using Noir (Next.js + Hardhat, Foundry, etc.)

### Libraries

- [Standard Library](https://github.com/noir-lang/noir/tree/master/noir_stdlib) - the Noir Standard Library 
- [Ethereum Storage Proof Verification](https://github.com/aragonzkresearch/noir-trie-proofs) - a library that contains the primitives necessary for RLP decoding (in the form of look-up table construction) and Ethereum state and storage proof verification (or verification of any trie proof involving 32-byte long keys)
- [BigInt](https://github.com/shuklaayush/noir-bigint) - a library that provides a custom BigUint56 data type, allowing for computations on large unsigned integers 
- [ECrecover](https://github.com/colinnielsen/ecrecover-noir/tree/main) - a library to verify an ECDSA signature and return the source Ethereum address 
- [Sparse Merkle Tree Verifier](https://github.com/vocdoni/smtverifier-noir/tree/main) - a library for verification of sparse Merkle trees
- [Signed Int](https://github.com/resurgencelabs/signed_int) - a library for accessing a custom Signed Integer data type, allowing access to negative numbers on Noir
- [Fraction](https://github.com/resurgencelabs/fraction) - a library for accessing fractional number data type in Noir, allowing results that aren't whole numbers 


## Projects

A curated list of projects powered by Noir.

### Authentication

- Anonymous proof of token ownership on Aztec (for token-gated access)
  - [Sequi](https://github.com/sequi-xyz)
  - [Cyclone](https://github.com/TalDerei/cyclone)

### Gaming

- [Mastermind](https://github.com/vezenovm/mastermind-noir) - Mastermind in Noir
- [BattleZips](https://battlezips.com/) ([Source Code](https://github.com/BattleZips/BattleZips-Noir)) - On-chain Battleship
- [Sudoku, Wordle, and Trivia](https://github.com/ruizehung/Zero-Knowledge-Sudoku-Wordle-Trivia) - Sudoku, Wordle, and Trivia games
- [ZCaptcha](https://github.com/signorecello/zcaptcha) - A ZK version of Captcha

### Governance

- [MeloCafe](https://github.com/MeloCafe) - Anonymous on-chain voting

### Social

- [FruityFriends](https://github.com/guelowrd/fruity-lib) - Various circuits (Proof of Intersection, Proof of Proximity, Proof of Proper Secret) to be used in social applications

## Contribute

Propose link additions by visiting [README.md](./README.md) and click the "pen" icon in the top right corner. Make changes to the file and follow the instructions to create a pull request.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
