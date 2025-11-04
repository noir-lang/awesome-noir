# Awesome Noir

A curated list of resources for learning and programming in Noir.

⚠️ This repository or the contained links are not endorsed as safe and secure by Aztec Labs or the Noir team. Users are advised to exercise caution before utilizing any content or code provided herein.

[![Awesome](https://img.shields.io/badge/Awesome-Repo-blue?logo=awesome-lists&style=flat)](https://awesome.re)
[![X (formerly Twitter) Follow](https://img.shields.io/twitter/follow/NoirLang)](https://x.com/NoirLang)
[![Discord](https://img.shields.io/badge/Discord-5865F2?logo=discord&logoColor=white&labelColor=5865F2&style=flat&labelWidth=100)](https://discord.com/invite/RJdCBN373S)

## Contents

<!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->

- [Useful Resources](#useful-resources)
- [Projects](#projects)
   * [General](#general)
   * [Authentication](#authentication)
   * [Commercial](#commercial)
   * [DeFi](#defi)
   * [Gaming](#gaming)
   * [Governance](#governance)
   * [Identity](#identity)
   * [Social](#social)
- [Benchmarks](#benchmarks)
- [Learning](#learning)
   * [Interactive Tutorials](#interactive-tutorials)
   * [Educational Curriculums](#educational-curriculums)
   * [Examples](#examples)
   * [Talks & Workshops](#talks-workshops)
      + [Coding in Noir](#coding-in-noir)
      + [Coding with Noir Projects](#coding-with-noir-projects)
      + [Project walkthroughs](#project-walkthroughs)
      + [Security](#security)
   * [Blog Posts & Articles](#blog-posts-articles)
   * [International Resources](#international-resources)
- [Boilerplates](#boilerplates)
- [Libraries](#libraries)
   * [General](#general-1)
   * [Data Types](#data-types)
      + [Numerics](#numerics)
      + [Dates & Times](#dates-times)
   * [Data Type Manipulation](#data-type-manipulation)
      + [General](#general-2)
      + [Numerics](#numerics-1)
      + [Bytes](#bytes)
      + [Texts](#texts)
      + [Collections](#collections)
   * [Cryptography](#cryptography)
      + [Elliptic Curves](#elliptic-curves)
      + [Hashes](#hashes)
      + [Encryption](#encryption)
      + [Signatures](#signatures)
      + [Merkle Trees](#merkle-trees)
      + [Message Authentication Code](#message-authentication-code)
      + [Randomness](#randomness)
   * [Blockchain Specifics](#blockchain-specifics)
      + [Aztec](#aztec)
      + [Ethereum](#ethereum)
      + [Bitcoin](#bitcoin)
   * [Social](#social-1)
   * [Machine Learning](#machine-learning)
- [Developer Tools](#developer-tools)
   * [Package Management](#package-management)
      + [Library Registry](#library-registry)
      + [CLI Manager](#cli-manager)
   * [IDE](#ide)
   * [Linting](#linting)
   * [Debugging](#debugging)
   * [Performance](#performance)
   * [Cross-platform](#cross-platform)
      + [Browser development](#browser-development)
      + [Mobile development](#mobile-development)
   * [EVM](#evm)
   * [Private shared states](#private-shared-states)
   * [Library-related](#library-related)
   * [Security](#security-1)
   * [Proving Backends](#proving-backends)
- [Contribute](#contribute)
- [License](#license)

<!-- TOC end -->

---

## Useful Resources

- [Docs](https://noir-lang.org/docs)
- [GitHub](https://github.com/noir-lang)
- [Discord](https://discord.gg/RJdCBN373S)
- [Community Job Board](https://www.notion.so/aztecnetwork/Noir-Community-Job-Board-1a1a1f6b0e3580a58515ecae879c8cf2)

## Projects

### General

- [AnonRadar](https://www.anonradar.xyz/) - registry of Noir projects
- [ZK Email](https://github.com/zkemail/zkemail.nr) - privacy-preserving proof of emails

### Authentication

- Safe modules for privacy-preserving multi-sig
  - [Dark Safe](https://github.com/colinnielsen/dark-safe)
  - [zkSafe](https://github.com/1kx-network/zksafe/)
  - [SAMM](https://github.com/oxor-io/samm-circuits) - zkEmail based
- [zkLogin](https://github.com/olehmisar/zklogin) - Apple/Google account based authentication for EVM smart accounts

### Commercial

- [GitClaim](https://github.com/saleel/gitclaim) - privacy-preserving airdrop claims through proof of GitHub contributions
- [z-imburse](https://github.com/Mach-34/z-imburse) - automated and privacy-preserving expense reimbursements
- [ZK-Flexor](https://github.com/RadNi/zk-flexor) - privacy-preserving proofs of EVM asset balances

### DeFi

- [Mezcal](https://github.com/olehmisar/mezcal) - a cutting edge on-chain limit order book dark pool.

### Gaming

- [ZK-AntiCheat](https://github.com/pop-eax/ZK-AntiCheat) - Privacy-Preserving anticheat engine 
- [Terry Escape](https://github.com/fatlabsxyz/terry-escape) - Multiplayer faction warfare in fog of war
- [zk-hangman-noir](https://github.com/Turupawn/zk-hangman-noir) - end-to-end zkDApp demo showcasing the Hangman circuit, EVM contract, and WASM frontend

### Governance

- [Nouns Anonymous Voting](https://github.com/aragonzkresearch/nouns-anonymous-voting) - privacy-preserving voting research project for NounsDAO

### Identity

- [Anon-Aadhaar](https://github.com/anon-aadhaar/anon-aadhaar-noir) - privacy-preserving verification of Aadhaar (Indian residence ID) through proofs revealing only selected identity information
- [Self](https://github.com/selfxyz/self) - identity wallet supporting privacy-preserving proofs of government-issued IDs
- [ZKPassport](https://github.com/zkpassport/) - privacy-preserving proofs of national passports
- [Rarimo](https://github.com/rarimo/passport-zk-circuits-noir) - passport signature verification circuits


### Social

- [anon.world](https://github.com/Slokh/anonworld) - social media with optional anonymity
- [Rate Limiting Nullifiers](https://github.com/curryrasul/rln.nr) - spam regulation/rate-limiting in anonymous environments
- [StealthNote](https://github.com/saleel/stealthnote) - message board for people in an organization to anonymously broadcast messages

## Benchmarks

- [MoPro's Benchmarks](https://zkmopro.org/docs/performance/#noir) - benchmarks of Noir programs on mobile and browser
- [Semaphore Benchmarks](https://hashcloak.github.io/semaphore-noir-final-report/benchmarks.html) - benchmarks of Semaphore implementations in Noir and Circom
- [RSA Benchmarks](https://github.com/zkpassport/noir_rsa?tab=readme-ov-file#benchmarks) - benchmarks of the Noir RSA signature verification library
- ECDSA secp256r1 Benchmarks - benchmarks of ECDSA signature verifications across different ZK tech stacks
  - [From the Base team](https://github.com/lukasrosario/zk-snark-ecdsa-benchmarks)
  - [From the Hyli team](https://github.com/vladfdp/p256-proving-benchmark)
- [Noir Development Bench](https://noir-lang.github.io/noir/dev/bench/) - development benchmarks of compilation and execution on latest Noir GitHub commits
- [Noir Benchmark CLI](https://github.com/francoperez03/noir-benchmark-cli) - CLI tool for benchmarking NoirJS + Barretenberg proof generation with visual pipeline profiling and performance insights

## Learning

### Interactive Tutorials

- [Noirlings](https://github.com/satyambnsal/noirlings) - A hands-on, interactive way to learn Noir programming language through practical exercises.
- [Noirlings.app](https://www.noirlings.app/) - Learn Noirlings on your browser, no setup needed.
- [Glass Bridge With Noir](https://zkdev.net/docs/tutorial/glass-bridge) – A browser-based game that demonstrates Zero-Knowledge Proofs using Noir. Learn by proving a secret path without revealing it.

### Educational Curriculums

- [Noir Programming And ZK Circuits by Cyfrin](https://updraft.cyfrin.io/courses/noir-programming-and-zk-circuits)
  - Step into the world of Noir, a domain-specific programming language for writing circuits, and learn to build zero-knowledge (ZK) apps. The Noir Programming and ZK Circuits course will teach you how to write circuits, how to build a full ZK protocol from scratch (using Noir, Barretenberg, and Solidity), and how to build the backend of a full-stack, privacy-preserving ZK application.
- [ZKCamp's Open Source Noir course](https://github.com/ZKCamp/aztec-noir-course)
  - 6 lectures to give participants the knowledge and skills necessary to build decentralized applications based on ZKPs using Noir
  - Lessons include ZKP Fundamentals; An Introduction to Aztec Ecosystem; Noir Basics; Building a Noir Application; and Advanced Noir
- [Video Series] [BattleZips-Noir](https://www.youtube.com/playlist?list=PLWACGbvIsEgnR2aUCr9i-PpmTVhF5Zuik) ([Source Code](https://github.com/BattleZips/BattleZips-Noir))
  - Walkthrough of building an on-chain Battleships game using zero-knowledge
  - Follow along and build your own game using Noir

### Examples

- [Noir Examples](https://github.com/noir-lang/noir-examples) - reference examples of zero-knowledge applications in Noir
- [Circuit Examples](https://github.com/thor314/circuit-examples) - demonstration implementation of dot products & Merkle proofs in Noir, Circom and RISC0
- [Write an app-specific plasma that preserves privacy](https://ethereum.org/developers/tutorials/app-plasma/) - complete tutorial for an application that relies on Ethereum and Noir for integrity while preserving privacy (except for one centralized component).

### Talks & Workshops

#### Coding in Noir

- [Workshop] [Build Your First ZK App with Noir](https://www.youtube.com/watch?v=06INZUM5Ca8)
- [Workshop] [ProtocolBerg v2: Learn Noir in an Afternoon](https://watch.protocol.berlin/65a90bf47932ebe436ba9351/watch?session=684ff138caecf08629c002f2)
- [Workshop] [Noir Xmas Camp: Building Applications with Noir](https://youtu.be/KxWNFIMyFiQ?si=cJmZSgpAbfeTOWxj) - E2E app building with NoirJS and the Noir Debugger
- [Workshop] [NoirHack: Advanced Noir](https://www.youtube.com/watch?v=OLhm6pKogbY) - using unconstrained functions for performance
- [Workshop] [NoirCon 2: Vibe Coding Noir](https://www.youtube.com/watch?v=KOFUwzqd4oo) - AI-assisted Noir coding with Cursor and Claude

#### Coding with Noir Projects

- [Talk] [d/Infra Summit: coNoir](https://www.youtube.com/watch?v=VvuKWx6afOA)
- [Talk] [NoirCon 2: Semaphore](https://www.youtube.com/watch?v=vfL7z74jGyU)
- [Workshop] [NoirHack: MoPro](https://www.youtube.com/watch?v=UrT2x3JSKFg)
- [Workshop] [NoirHack: ZK Email](https://www.youtube.com/watch?v=jpJdxlIZd5w)
- [Workshop] [NoirHack: ZK Kit](https://www.youtube.com/watch?v=jKI60vZkCPY)
- [Workshop] [NoirHack: ZKPassport](https://www.youtube.com/watch?v=Na60y_WOWUY)

#### Project walkthroughs

- [Workshop] [NoirHack: Stealthnote and GitClaim](https://www.youtube.com/watch?v=aX5ExM4sL6A)

#### Security

- [Workshop] [Circuit Safety and an Introduction to Noir](https://www.youtube.com/watch?v=rLvu61DA-hk) - common ZK vulnerabilities and an introduction to Noir
- [Workshop] [Noir Xmas Camp: Circuit Security & Production Readiness with Noir](https://youtu.be/pNI_56b7Bdo?si=LU1wQ-2Igd4Z7oNA)
- [Workshop] [NoirCon 2: Lampe](https://www.youtube.com/watch?v=CPel4WyBNuk) - formal verification of Noir programs in Lean

### Blog Posts & Articles

- [Understanding the Technical Aspects of Aztec and Noir](https://hackmd.io/XZX9_pZ8Q1aa_ySDPeQopg)
- Noir 101 for Solidity devs in ([English](https://mirror.xyz/crisgarner.eth/IRRxnP-HVP-7qLZ-bTI2HRpKTmSRPCDl-Q6gm2NTj4g)) and ([Spanish](https://mirror.xyz/crisgarner.eth/Iek7PhbhU4WpIJ6eixFq80_7R6czH7fbdCoN0Bd7NfI))
- [Privacy-preserving KYC with Noir](https://medium.com/@tisura/privacy-preserving-kyc-57002ab8d3f2)
- [An incomplete guide to zk-KYC apps](https://medium.com/@tisura/an-incomplete-guide-to-zk-kyc-apps-d7b4c684795c)
- [Build a Decentralized Voting Application w/ Noir](https://threesigma.xyz/blog/build-noir-decentralized-voting-application)

### International Resources

- [Introduction to Noir in Spanish](https://www.youtube.com/watch?v=m4P-sAqa8_o)
  - ([Written Tutorial and Code](https://dev.to/turupawn/circuitos-de-aztec-noir-en-tu-navegador-zk-es-semana-3-78a))
- [Building a ZK dApp in Cantonese](https://www.youtube.com/watch?v=IAQrO1j20pg)
  - [Slides](https://docs.google.com/presentation/d/1Zh8McXfdjREg0Y6iG9Q1_d-8Sgi7QT_7gJdOSmLqEEI/)

## Boilerplates

- [hardhat-noir-starter](https://github.com/olehmisar/hardhat-noir-starter) - project template with seamless Hardhat integration
- [noir-library-starter](https://github.com/noir-lang/noir-library-starter) - library template
- [noir-react-native-starter](https://github.com/madztheo/noir-react-native-starter) - mobile development template using React Native
- [nargo binary examples](https://github.com/noir-lang/noir/tree/master/examples) - barebones use of nargo binary (and a proving backend) from: simple prove/verify, codegen, to recursion
- [noir-recursive](https://github.com/teddav/noir-recursive) - recursion circuit template with UltraHonk in javascript

## Libraries

For package management (e.g. library registry, CLI manager), refer to the [package management tooling](#package-management) section.

For library tooling (e.g. input generators, TypeScript implementations), refer to the [library-related tooling](#library-related) section.

### General

- [Standard Library](https://github.com/noir-lang/noir/tree/master/noir_stdlib) - standard library that ships with all Noir releases
- [ZK Kit Noir](https://github.com/privacy-scaling-explorations/zk-kit.noir) - collection of algorithm and utility libraries from Privacy & Scaling Explorations

### Data Types

#### Numerics

- [BigNum](https://github.com/noir-lang/noir-bignum) - a library for arithmetic computations of large unsigned integers of any length
- [Fraction](https://github.com/resurgencelabs/fraction) - a library for accessing fractional number data types in Noir, allowing results that aren't whole numbers
- [ZKFloat](https://github.com/0x3327/ZKFloat) - a floating point library for Noir
- [Complex Numbers](https://github.com/doctoruber/complexnr) - This library offers a comprehensive suite of operations for complex numbers
- [Fixed Point Library](https://github.com/doctoruber/noir-fixed-point) - The FixedPoint library offers precise fixed-point arithmetic operations tailored for Noir
- [Fixed Point Library for scale 2^-16](https://github.com/hashcloak/noir-fixed-point) - an optimized fixed point arithmetic library designed for scale 2^-16.

#### Dates & Times

- [Noir Dates](https://github.com/madztheo/noir-date) - A Noir library to parse and abstract away Dates
- [DateTimeNr](https://github.com/doctoruber/DateTimeNr) - A Noir library to parse and abstract away DateTime objects

### Data Type Manipulation

#### General

- [nodash](https://github.com/olehmisar/nodash) - utility library for working with various data types, inspired by Lodash

#### Numerics

- [Matrix Operations](https://github.com/storswiftlabs/matrix_operations) - a library for matrix operations provides functionality for performing various matrix operations
- [Statistical Library](https://github.com/doctoruber/statnr) - Noir Statistical Library is a comprehensive library for statistical computations in the Noir language
- [Quantized arithmetic](https://github.com/storswiftlabs/quantized_arithmetic) - a library for quantized value operations of zero-point quantization

#### Bytes

- [U(int)2B(ytes)](https://github.com/colinnielsen/noir-u2b) - a library for converting `u8`->`u120`s to `[u8]` array

#### Texts

- [Base64](https://github.com/vlayer-xyz/noir-base64) - a library for base64 encoding
- [Noir Base64 Library](https://github.com/Envoy-VC/noir_base64_lib) - extension of `noir_base64` with support for Vectors and Base64 URL encoding and decoding
- [JSON parser](https://github.com/noir-lang/noir_json_parser) - JSON string parsing, adheres to [IETF RFC 8259](https://datatracker.ietf.org/doc/html/rfc8259)
- [String Utils](https://github.com/madztheo/noir-string-utils) - wrapper for String in Noir adding methods for common string operations
- [String Search](https://github.com/noir-lang/noir_string_search) - proof of substring existence within a larger string
- [zkRegEx](https://github.com/zkemail/zk-regex) - proof of Regular Expression (RegEx) verification

#### Collections

- [Sort](https://github.com/noir-lang/noir_sort) - efficient sorting of fixed-sized arrays
- [Sparse Array](https://github.com/noir-lang/sparse_array) - efficient immutable and mutable sparse arrays
- [Lib_LinkList](https://github.com/0xKarl98/Lib_LinkList) - A memory-efficient doubly-linked list implementation for Noir that supports constant time operations at both ends

### Cryptography

#### Elliptic Curves

- [BigCurve](https://github.com/noir-lang/noir_bigcurve) - operations over elliptic curves instantiated with an arbitrary prime field
- [Pairing over BLS12-381](https://github.com/ewynx/noir_bls12_381_pairing) - Pairing over BLS12-381

#### Hashes

- [Keccak256](https://github.com/noir-lang/keccak256) - Keccak256 hashes
- [MiMC](https://github.com/noir-lang/mimc) - MiMC hashes
- [Poseidon](https://github.com/noir-lang/poseidon) - Poseidon and Poseidon2 hashes
- [RIPEMD160](https://github.com/distributed-lab/noir-ripemd160) - RIPEMD160 hashes
- [SHA256](https://github.com/noir-lang/sha256) - SHA256 hashes
- [SHA512](https://github.com/noir-lang/sha512) - SHA512 and SHA384 hashes

#### Encryption

- [AES](https://github.com/TaceoLabs/noir-aes) - a (naive) implementation of AES encryption and decryption
- [ChaCha20 Implementation](https://github.com/SleepingShell/noir-chacha20) - a Noir implementation of ChaCha20 as defined by [RFC7539](https://www.rfc-editor.org/rfc/rfc7539)
- [ElGamal Encryption](https://github.com/jat9292/noir-elgamal/) - Exponential ElGamal Encryption on the Baby Jubjub curve
- [Hydra for BN254](https://github.com/TaceoLabs/noir-hydra) - symmetric encryption and decryption
- [ECIES](https://github.com/informalsystems/noir-ecies) - simple implementation of ECIES on the Baby Jubjub curve
- [ECDH](https://github.com/privacy-scaling-explorations/zk-kit.noir/tree/main/packages/ecdh) - simple implementation of ECDH on the Baby Jubjub curve

#### Signatures

- [BLS12_381 Elliptic Curve Pairing and Signature Verification Library](https://github.com/onurinanc/noir-bls-signature)
- [EdDSA](https://github.com/noir-lang/eddsa) - EdDSA signature verification
- [ECDSA](https://github.com/zkpassport/noir-ecdsa) - ECDSA (NIST and Brainpool curves) signature verification
- [JWT](https://github.com/saleel/noir-jwt) - Verification of JSON Web Tokens (JWTs) and prove claims
- [PLUME](https://github.com/signorecello/zk-nullifier-sig/) - ECDSA-based nullifiers
- [RSA](https://github.com/zkpassport/noir_rsa) - RSA signature verification
- [Schnorr](https://github.com/noir-lang/schnorr) - Schnorr signature verification
- [WebAuthn/Passkeys](https://github.com/olehmisar/noir_webauthn) - Verification of WebAuthn/Passkeys signatures; verifies signatures produced by `credentials.get`

#### Merkle Trees

- [ZK-Kit: Merkle Trees](https://github.com/privacy-scaling-explorations/zk-kit.noir/tree/main/packages/merkle-trees) - verification of (non-)membership proofs and add/update/delete leaves
- [Indexed Merkle Tree](https://github.com/numtel/indexed-merkle-noir) - Generate and verify proofs of inclusion, exclusion, or insert transition, includes complementary NPM package

#### Message Authentication Code

- [Noir HMAC](https://github.com/zkpersona/noir-hmac) - hash-based message authentication code

#### Randomness

- [Cryptographically Secure Pseudo-Random Number Generator](https://github.com/doctoruber/CSPRNG) - pseudo-random number generation

### Blockchain Specifics

#### Aztec

- [Aztec Storage proofs](https://github.com/nemi-fi/aztec_storage_proofs) - proving Aztec note inclusion in plain Noir, with verification in JavaScript or Solidity

#### Ethereum

- [ECrecover](https://github.com/colinnielsen/ecrecover-noir) - ECDSA signature verification and return of source Ethereum address
- [Ethereum Storage Proof](https://github.com/olehmisar/vlayer-monorepo) - proving and verifying historical Ethereum / EVM accounts, storage, logs, receipts & transactions
- [Ethereum MPT Proof](https://github.com/RadNi/mpt-noir) - proving Ethereum Merkle Patricia Trie with recursive proof aggregations

#### Bitcoin

- [op_rand](https://github.com/distributed-lab/op_rand) - VRF on Bitcoin. Proves the correctness of all the actions using Noir circuits with Barretenberg backend
- [bitcoin-prover](https://github.com/distributed-lab/bitcoin-prover) - proving the validity of the Bitcoin block header chain and the possibility of using the corresponding output as the input of a transaction.

### Social

- [Noir Social Verify](https://github.com/Envoy-VC/noir_social_verify) - zkEmail based proof of GitHub, Google, LinkedIn and X accounts and account details
- [Noir Semaphore](https://github.com/distributed-lab/noir-semaphore) - Semaphore Protocol adapted to use Noir.

### Machine Learning

- [Convolution](https://github.com/storswiftlabs/convolution) - Convolutional Neural Network (CNN) library, including Convolutional layers, Pooling layers, and Linear (fully connected) layers
- [ML](https://github.com/metavind/noir-ml) - neural networks
- [SKProof](https://github.com/0x3327/skproof) - Scikit-learn compatible Python library for generating ZK proofs of execution
- [zkML-Noir](https://github.com/storswiftlabs/zkml-noir) - Python ML model Noir transcoding, including various algorithms such as Decision tree, K-Means, XGBoost, FNN, CNN

## Developer Tools

### Package Management

#### Library Registry

- [Noir Libs](https://noir-libs.org/) by Walnut

#### CLI Manager

- [noir-libs](https://github.com/walnuthq/noir-libs) by Walnut
- [noirupi](https://github.com/michaelelliot/noirupi) - Interactive noirup and bbup. Update noir and bb interactively using `noirupi` and `bbupi`

### IDE

- [Noir Playground](https://www.noir-playground.app/) - A browser-based Noir zero-knowledge proof development environment. ([Source Code](https://github.com/0xandee/noir-playground))
- [VS Code Extension](https://marketplace.visualstudio.com/items?itemName=noir-lang.vscode-noir) - Syntax highlight, error highlight, codelens, etc. ([Source Code](https://github.com/noir-lang/vscode-noir))
- [Neovim Plugin](https://github.com/noir-lang/noir-nvim) - Syntax highlight, error highlight, etc.
- [Emacs Plugin](https://melpa.org/#/noir-mode) - Syntax highlight ([Source Code](https://github.com/hhamud/noir-mode))
- [Zed Plugin](https://github.com/shuklaayush/zed-noir) - Syntax highlight, LSP support
- [tree_sitter_noir](https://github.com/tsujp/tree_sitter_noir) - Tree-sitter grammar for Noir
- [Emacs Tree-sitter Plugin](https://melpa.org/#/noir-ts-mode) - Syntax highlight ([Source Code](https://github.com/hhamud/noir-ts-mode))

### Linting

- [Noir Static Analyzer](https://github.com/walnuthq/noir-static-analyzer) by Walnut

### Debugging

- [CodeTracer](https://github.com/metacraft-labs/codetracer) - A visual time-travelling debugger for Linux and MacOS with support for Noir

### Performance

- [Noir + Barretenberg Profiler](https://github.com/noir-lang/noir/tree/master/tooling/profiler) - Opcode, execution and proving costs flamegraphing tool
- [noir-web](https://github.com/gnosisguild/noir-web) – benchmark proving and verification of Noir programs on the browser

### Cross-platform

#### Browser development

- [NoirJS](https://noir-lang.org/docs/tutorials/noirjs_app) - compile and execute Noir programs in JavaScript / TypeScript
- [Noir Codegen for TypeScript](https://noir-lang.org/docs/reference/noir_codegen) - generate TypeScript bindings for computing Noir program outputs in TS

#### Mobile development

- [MoPro](https://github.com/zkmopro) by PSE - prove and verify Noir programs on mobile (Android and iOS)
- [Noir.rs](https://github.com/zkpassport/noir_rs) by ZKPassport - prove and verify Noir programs with Rust
- [Swoir](https://github.com/Swoir/swoir) by ZKPassport - prove and verify Noir programs with Swift on iOS and MacOS
- [Noir Android](https://github.com/madztheo/noir_android) by ZKPassport - prove and verify Noir programs with Kotlin on Android

### EVM

- [hardhat-noir](https://www.npmjs.com/package/hardhat-noir) - Hardhat plugin ([Source Code](https://github.com/olehmisar/hardhat-noir))
- [foundry-noir-helper](https://github.com/0xnonso/foundry-noir-helper) - helper library for working with Noir circuits within Foundry.

### Private shared states

- [coSNARKs](https://github.com/TaceoLabs/co-snarks) - generate witness and prove Noir programs in a Multi-Party Computation network
- [Kalypso](https://docs.marlin.org/user-guides/kalypso/tutorials/noir-circuits/) - generate witness and prove Noir programs in Trusted Execution Environments

### Library-related

- [Merkle Tree Generator](https://github.com/eyalron33/mpz/) - generate Noir-library-friendly Pedersen based Merkle trees
- [Safecat](https://neimanslab.org/2024-02-19/safecat.html) - generate Noir-library-friendly EdDSA Baby Jubjub Elliptic Curve signatures
- [Poseidon2 in TypeScript](https://github.com/zkpassport/poseidon2) - a Poseidon2 library in pure TypeScript with support for the implementation used by Noir (over BN254)

### Security

- [rocq-of-noir](https://github.com/formal-land/rocq-of-noir) - formal verification of Noir programs with Rocq
- [lampe](https://github.com/reilabs/lampe) - formal verification of Noir programs with Lean
- [hunter](https://github.com/nfurfaro/hunter) - mutation-testing of Noir programs
- [Circuzz fuzzer](https://github.com/Rigorous-Software-Engineering/circuzz) - fuzzer for finding soundness and completeness issues in the Noir infrastructure (by Consensys Diligence and TU Vienna)

### Proving Backends

- [Barretenberg (UltraHonk / MegaHonk)](https://github.com/AztecProtocol/barretenberg) by Aztec Labs
- [coSNARKs](https://github.com/TaceoLabs/co-snarks) by Taceo Labs
- [Edge (Supernova)](https://github.com/pluto/edge) by Pluto
- [Plonky2](https://github.com/blocksense-network/noir) by Blocksense
- [ProveKit (Recursive Groth16)](https://github.com/worldfnd/ProveKit) by World
- [Sonobe (Nova, HyperNova)](https://github.com/privacy-scaling-explorations/sonobe) by 0xPARC and PSE
- [Gnark](https://github.com/lambdaclass/noir_backend_using_gnark) by Lambdaclass (needs updating)
- [Groth16](https://github.com/TomAFrench/acvm-backend-groth16) (needs updating)
- [Halo2](https://github.com/Ethan-000/halo2_backend) by Ethan (needs updating)
- [Marlin](https://github.com/noir-lang/marlin_arkworks_backend) (needs updating)
- [Plonky2](https://github.com/eryxcoop/acvm-backend-plonky2) by Eryx (needs updating)
- [Plonky3](https://github.com/vacekj/air-fried-gyatt) by Josef (needs updating)

## Contribute

Propose link additions by [editing the README.md](https://github.com/noir-lang/awesome-noir/edit/main/README.md). We welcome and appreciate your contributions — thank you for helping improve this list!

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
