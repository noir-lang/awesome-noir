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

- [Educational Curriculum] [ZKCamp's Open Source Noir course](https://github.com/ZKCamp/aztec-noir-course)
  - 6 lectures to give participants the knowledge and skills necessary to build decentralized applications based on ZKPs using Noir
  - Lessons include ZKP Fundamentals; An Introduction to Aztec Ecosystem; Noir Basics; Building a Noir Application; and Advanced Noir  
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
- [45 mins] [Outlandish Noir Stuff; Workshop at ETHCC](https://www.youtube.com/watch?v=pdrZ7Y__obU)
  - How to use Noir to build a bunch of outlandish stuff
- [1 hr] [Circuit Safety and an Introduction to Noir](https://www.youtube.com/watch?v=rLvu61DA-hk)
  - Common circuit bugs
  - Proving system vulnerabilities
  - Unconstrained functions
- [1 hr] [Introduction to Noir in Spanish](https://www.youtube.com/watch?v=m4P-sAqa8_o) ([Written Tutorial and Code](https://dev.to/turupawn/circuitos-de-aztec-noir-en-tu-navegador-zk-es-semana-3-78a))
- [1.5 hrs] [ZK dApps - Why, What and How?](https://www.youtube.com/watch?v=DpCbeGcX0cI)
- [1.5 hrs] [Sudoku in Noir](https://drive.google.com/file/d/1D4XCdiIZVjUW1JHDoMW3pG-15mgjMm9E/) ([Source Code](https://github.com/guipublic/crypdoku))
- [2 hrs] [ZK HACK III - Introduction to Noir](https://www.youtube.com/watch?v=5CziMfChveY) ([Souce Code](https://github.com/joss-aztec/quadratic_voting_noir))
  - Code-together: Quadratic Voting

### Blog Posts & Articles

- [Understanding the Technical Aspects of Aztec and Noir](https://hackmd.io/XZX9_pZ8Q1aa_ySDPeQopg)
- Noir 101 for Solidity devs in ([English](https://mirror.xyz/crisgarner.eth/IRRxnP-HVP-7qLZ-bTI2HRpKTmSRPCDl-Q6gm2NTj4g)) and ([Spanish](https://mirror.xyz/crisgarner.eth/Iek7PhbhU4WpIJ6eixFq80_7R6czH7fbdCoN0Bd7NfI))

## Get Coding

### Dev Tools

- [Noir Editor](https://noir-lang.github.io/noir-cra/)   - Browser IDE ([Souce Code](https://github.com/noir-lang/noir-cra))
- [VSCode Extension](https://marketplace.visualstudio.com/items?itemName=noir-lang.noir-programming-language-syntax-highlighter) - Syntax highlight ([Source Code](https://github.com/noir-lang/vscode-noir))
- [Vim Plugin](https://github.com/Louis-Amas/noir-vim-support) - Syntax highlight
- [Emacs Plugin](https://melpa.org/#/noir-mode) - Syntax highlight ([Source Code](https://github.com/hhamud/noir-mode))
- [Tree-sitter-noir](https://github.com/hhamud/tree-sitter-noir) - Tree-sitter grammar for Noir language
- [Emacs Tree-sitter Plugin](https://melpa.org/#/noir-ts-mode) - Syntax highlight ([Source Code](https://github.com/hhamud/noir-ts-mode))
- [hardhat-noir](https://www.npmjs.com/package/hardhat-noir) - Hardhat plugin ([Source Code](https://github.com/spalladino/hardhat-noir))
- [Python2Noir](https://github.com/storswiftlabs/python2noir) - From Python to Noir language transpiler

### Boilerplates

- [nplate](https://github.com/whitenois3/nplate) - Minimalist template
- [noir-hardhat-template](https://github.com/hooperben/noir-hardhat-template) - Hardhat template
- [noir-starter](https://github.com/noir-lang/noir-starter) - Template repository containing example projects using Noir (Next.js + Hardhat, Foundry, etc.)
- [noir-starter-nuxt](https://github.com/iam-robi/noir-starter-nuxt) - Template repository containing example minimal project using Noir, Nuxt and Hardhat
- [noir-vite-starter](https://github.com/HaMMeRSI/noir-vite-starter) - Template repository contiaining example minimal project using Noir and Vite

### Libraries

- [Standard Library](https://github.com/noir-lang/noir/tree/master/noir_stdlib) - the Noir Standard Library

#### Types

- [BigInt](https://github.com/shuklaayush/noir-bigint) - a library that provides a custom BigUint56 data type, allowing for computations on large unsigned integers
- [Signed Int](https://github.com/resurgencelabs/signed_int) - a library for accessing a custom Signed Integer data type, allowing access to negative numbers on Noir
- [Fraction](https://github.com/resurgencelabs/fraction) - a library for accessing fractional number data type in Noir, allowing results that aren't whole numbers
- [U(int)2B(ytes)](https://github.com/colinnielsen/noir-u2b/tree/main) - a library for converting `u8`->`u120`s to `[u8]` array
- [ZKFloat](https://github.com/0x3327/ZKFloat) - a floating point library for Noir

#### Cryptograpy

- [Sparse Merkle Tree Verifier](https://github.com/vocdoni/smtverifier-noir/tree/main) - a library for verification of sparse Merkle trees
- [RSA](https://github.com/SetProtocol/noir-rsa) - this repository contains an implementation of a RSA signature verify for the Noir language
- [Merkle Root](https://github.com/tomoima525/noir-merkle-root) - a library for calculating Merkle root from given inputs. Using the Poseidon function for hashing
- [Quantized arithmetic](https://github.com/storswiftlabs/quantized_arithmetic) - a library for quantized value operations of zero-point quantization

#### Ethereum
- [Ethereum Storage Proof Verification](https://github.com/aragonzkresearch/noir-trie-proofs) - a library that contains the primitives necessary for RLP decoding (in the form of look-up table construction) and Ethereum state and storage proof verification (or verification of any trie proof involving 32-byte long keys)
- [ECrecover](https://github.com/colinnielsen/ecrecover-noir/tree/main) - a library to verify an ECDSA signature and return the source Ethereum address

#### Machine Learning

- [SKProof](https://github.com/0x3327/skproof) - a Scikit-learn compatible Python library for generating ZK proofs of execution
- [ML](https://github.com/metavind/noir-ml) - a library for implementing neural networks in Noir
- [zkML-Noir](https://github.com/storswiftlabs/zkml-noir) - a library for Python ML model transcoding Noir, including various algorithms such as Decision tree, K-Means, XGBoost, FNN, CNN
- [Matrix Operations](https://github.com/storswiftlabs/matrix_operations) - a library for matrix operations provides functionality for performing various matrix operations
- [Convolution](https://github.com/storswiftlabs/convolution) - a library for Convolutional Neural Network (CNN) library in Noir, including Convolutional layers, Pooling layers, and Linear (fully connected) layers.

#### Miscellaneous

- [Rate Limiting Nullifiers](https://github.com/Rate-Limiting-Nullifier/noir-rln) - a zero-knowledge gadget that enables spam prevention in anonymous environments


## Projects

A curated list of projects powered by Noir.

### Authentication

- Anonymous proof of token ownership on Aztec for token-gated access
  - [Sequi](https://github.com/sequi-xyz)
  - [Cyclone](https://github.com/TalDerei/cyclone)
- [SafeRecover](https://github.com/porco-rosso-j/safe-recovery-noir) - Recovery of ownership of Gnosis Safe accounts

### Gaming

- [Mastermind](https://github.com/vezenovm/mastermind-noir) - Mastermind in Noir
- [BattleZips](https://battlezips.com/) ([Source Code](https://github.com/BattleZips/BattleZips-Noir)) - On-chain Battleship
- [Sudoku, Wordle, and Trivia](https://github.com/ruizehung/Zero-Knowledge-Sudoku-Wordle-Trivia) - Sudoku, Wordle, and Trivia games
- [ZCaptcha](https://github.com/signorecello/zcaptcha) - A ZK version of Captcha
- [Hangman](https://github.com/resurgencelabs/hangman) - Simple implementation of the Hangman game

### Governance

- [MeloCafe](https://github.com/MeloCafe) - Anonymous on-chain voting
- [Nouns Research Sprint](https://github.com/aragonzkresearch/nouns-anonymous-voting) -  Anonymous voting research sprint solution with NounsDAO

### Social

- [FruityFriends](https://github.com/guelowrd/fruity-lib) - Various circuits (Proof of Intersection, Proof of Proximity, Proof of Proper Secret) to be used in social applications

## Contribute

Propose link additions by visiting [README.md](./README.md) and click the "pen" icon in the top right corner. Make changes to the file and follow the instructions to create a pull request.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
