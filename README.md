# Awesome Noir

A curated list of resources for learning and programming in Noir.

⚠️ This repository or the contained links are not endorsed as safe and secure by Aztec Labs or the Noir team. Users are advised to exercise caution before utilizing any content or code provided herein.

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![X (formerly Twitter) Follow](https://img.shields.io/twitter/follow/NoirLang)](https://x.com/NoirLang)

---

## Official Resources

- [Docs](https://noir-lang.org/)
- [GitHub](https://github.com/noir-lang/noir)
- [Discord](https://discord.gg/RJdCBN373S)
- [Noir Forum](https://forum.aztec.network/c/noir/7)

## Boilerplates

- [noir-starter](https://github.com/noir-lang/noir-starter) - project template containing examples using Noir with Vite + Hardhat and Foundry
- [hardhat-noir-starter](https://github.com/olehmisar/hardhat-noir-starter) - project template with seamless Hardhat integration
- [noir-library-starter](https://github.com/noir-lang/noir-library-starter) - library template
- [noir-react-native-starter](https://github.com/madztheo/noir-react-native-starter) - mobile development template using React Native
- [nargo binary examples](https://github.com/noir-lang/noir/tree/master/examples) - barebones use of nargo binary (and a proving backend) from: simple prove/verify, codegen, to recursion

## Libraries

For package management (e.g. library registry, CLI manager), refer to the [package management tooling](#package-management) section.

For library tooling (e.g. input generators, TypeScript implementations), refer to the [library-related tooling](#library-related) section.

### General

- [Standard Library](https://github.com/noir-lang/noir/tree/master/noir_stdlib) - standard library that ships with all Noir releases
- [ZK Kit Noir](https://github.com/privacy-scaling-explorations/zk-kit.noir) - collection of algorithm and utility libraries from Privacy & Scaling Explorations

### Data Types

#### Numerics

- [BigNum](https://github.com/noir-lang/noir-bignum) - a library for arithmetic computations of large unsigned integers of any length
- [Fraction](https://github.com/resurgencelabs/fraction) - a library for accessing fractional number data type in Noir, allowing results that aren't whole numbers
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

#### Arrays

- [Sort](https://github.com/noir-lang/noir_sort) - efficient sorting of fixed-sized arrays
- [Sparse Array](https://github.com/noir-lang/sparse_array) - efficient immutable and mutable sparse arrays

### Cryptography

#### Elliptic Curves

- [BigCurve](https://github.com/noir-lang/noir_bigcurve) - operations over elliptic curves instantiated with an arbitrary prime field
- [Pairing over BLS12-381](https://github.com/ewynx/noir_bls12_381_pairing) - Pairing over BLS12-381

#### Hashes

- [Griffin for BN254](https://github.com/TaceoLabs/noir-griffin) - zk-friendly Griffin hashes
- [Hash to curve](https://github.com/skaunov/hash_to_curve) - hashing to bigger curves
- [Keccak256](https://github.com/noir-lang/keccak256) - Keccak256 hashes
- [MiMC](https://github.com/noir-lang/mimc) - MiMC hashes
- [SHA1](https://github.com/michaelelliot/noir-sha1) - SHA1 hashes
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
- [JWT](https://github.com/saleel/noir-jwt) - Verification of JSON Web Tokens (JWTs) and prove claims
- [PLUME](https://github.com/signorecello/zk-nullifier-sig/) - ECDSA-based nullifiers
- [RSA](https://github.com/noir-lang/noir_rsa) - RSA signature verification
- [Schnorr](https://github.com/noir-lang/schnorr) - Schnorr signature verification
- [WebAuthn/Passkeys](https://github.com/olehmisar/noir_webauthn) - Verification of WebAuthn/Passkeys signatures; verifies signatures produced by `credentials.get`

#### Merkle Trees

- [Merkle Root](https://github.com/tomoima525/noir-merkle-root) - calculating Merkle root from given inputs of a Poseidon based Merkle tree
- [Sparse Merkle Tree Implementation](https://github.com/jordan-public/zk-optimized-sparse-merkle-tree) - TypesSript library to generate optimized sparse merkle trees
- [Sparse Merkle Tree Verifier](https://github.com/vocdoni/smtverifier-noir) - verification of sparse Merkle trees
- [Sparse Merkle Tree Verify/Add/Update/Delete](https://github.com/privacy-scaling-explorations/zk-kit.noir/tree/main/packages/merkle-trees) - verification of (non-)membership proofs and add/update/delete leaves

#### Message Authentication Code

- [Noir HMAC](https://github.com/Envoy-VC/noir_hmac) - hash-based message authentication code

#### Randomness

- [Cryptographically Secure Pseudo-Random Number Generator](https://github.com/doctoruber/CSPRNG) - pseudo-random number generation

### Ethereum

- [ECrecover](https://github.com/colinnielsen/ecrecover-noir) - ECDSA signature verification and return of source Ethereum address
- [Ethereum Storage Proof](https://github.com/olehmisar/vlayer-monorepo) - proving and verifying historical Ethereum / EVM accounts, storage, logs, receipts & transactions

### Social

- [Noir Social Verify](https://github.com/Envoy-VC/noir_social_verify) - zkEmail based proof of GitHub, Google, LinkedIn and X accounts and account details

### Machine Learning

- [Convolution](https://github.com/storswiftlabs/convolution) - Convolutional Neural Network (CNN) library, including Convolutional layers, Pooling layers, and Linear (fully connected) layers
- [ML](https://github.com/metavind/noir-ml) - neural networks
- [SKProof](https://github.com/0x3327/skproof) - Scikit-learn compatible Python library for generating ZK proofs of execution
- [zkML-Noir](https://github.com/storswiftlabs/zkml-noir) - Python ML model Noir transcoding, including various algorithms such as Decision tree, K-Means, XGBoost, FNN, CNN

## Dev Tools

### Package Management

#### Library Registry

- [Noir Directory](https://noir.directory) by Oleh
- [Noir Libs](https://noir-libs.org/) by Walnut

#### CLI Manager

- [noir-libs](https://github.com/walnuthq/noir-libs) by Walnut

### IDE

- [VS Code Extension](https://marketplace.visualstudio.com/items?itemName=noir-lang.vscode-noir) - Syntax highlight, error highlight, codelens, etc. ([Source Code](https://github.com/noir-lang/vscode-noir))
- [Neovim Plugin](https://github.com/noir-lang/noir-nvim) - Syntax highlight, error highlight, etc.
- [Emacs Plugin](https://melpa.org/#/noir-mode) - Syntax highlight ([Source Code](https://github.com/hhamud/noir-mode))
- [Zed Plugin](https://github.com/shuklaayush/zed-noir) - Syntax highlight, LSP support
- [Tree-sitter-noir](https://github.com/hhamud/tree-sitter-noir) - Tree-sitter grammar for Noir language
- [Emacs Tree-sitter Plugin](https://melpa.org/#/noir-ts-mode) - Syntax highlight ([Source Code](https://github.com/hhamud/noir-ts-mode))

### Performance

- [Noir + Barretenberg Profiler](https://github.com/noir-lang/noir/tree/master/tooling/profiler) - Opcode, execution and proving costs flamegraphing tool

### Cross-language

- [noir_js](https://github.com/noir-lang/noir/tree/master/tooling/noir_js) - compiling and executing Noir programs in JavaScript / TypeScript
- [Noir.rs](https://github.com/zkpassport/noir_rs) - Proving and verifying Noir programs in Rust (compatible with mobile architectures such as iOS and Android)
- [Python2Noir](https://github.com/storswiftlabs/python2noir) - Python to Noir transpiler
- [Swoir](https://github.com/Swoir/swoir) - Proving and verifying Noir programs in Swift on iOS and MacOS
- [Noirandroid](https://github.com/madztheo/noir_android) - Proving and verifying Noir programs in Kotlin on Android

### EVM

- [hardhat-noir](https://www.npmjs.com/package/hardhat-plugin-noir) - Hardhat plugin ([Source Code](https://github.com/olehmisar/hardhat-noir))
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

### Proving Backends

- [Barretenberg (UltraHonk / MegaHonk)](https://github.com/AztecProtocol/barretenberg) by Aztec Labs
- [Plonky2](https://github.com/blocksense-network/noir) by Blocksense
- [Plonky2](https://github.com/eryxcoop/acvm-backend-plonky2) by Eryx
- [Sonobe (Nova, HyperNova)](https://github.com/privacy-scaling-explorations/sonobe) by 0xPARC and PSE
- [coSNARKs](https://github.com/TaceoLabs/co-snarks) by Taceo Labs
- [Plonky3](https://github.com/vacekj/air-fried-gyatt) by Josef (needs updating)
- [Halo2](https://github.com/Ethan-000/halo2_backend) by Ethan (needs updating)
- [Groth16](https://github.com/TomAFrench/acvm-backend-groth16) (needs updating)
- [Marlin](https://github.com/noir-lang/marlin_arkworks_backend) (needs updating)

## Projects

### General

- [ZKEmail](https://github.com/zkemail/zkemail.nr) - privacy-preserving proof of emails

### Benchmarks

- [Noir Development Bench](https://noir-lang.github.io/noir/dev/bench/) - Compilation and execution memory and time benchmarks of latest Noir GitHub commits
- [ZK-Bench](https://zkbench.dev) - Compare Noir to other ZK frameworks (Risc Zero, Leo, Miden, etc)

### Authentication

- Safe modules for privacy-preserving multi-sig
  - [Dark Safe](https://github.com/colinnielsen/dark-safe)
  - [zkSafe](https://github.com/1kx-network/zksafe/)
  - [SAMM](https://github.com/oxor-io/samm-circuits) - zkEmail based
- [zkLogin](https://github.com/olehmisar/zklogin) - Apple/Google account based authentication for EVM smart accounts

### Commercial
- [GitClaim](https://github.com/saleel/gitclaim) - privacy-preserving airdrop claims through proof of GitHub contributions
- [z-imburse](https://github.com/Mach-34/z-imburse) - automated and privacy-preserving expense reimbursements

### Gaming

- [BattleZips](https://battlezips.com/) ([Source Code](https://github.com/BattleZips/BattleZips-Noir)) - on-chain Battleship
- [Dappicom](https://github.com/tonk-labs/dappicom) - Nintendo Entertainment System (NES) emulator in Noir for proofs of gameplays / speedruns

### Governance

- [Nouns Anonymous Voting](https://github.com/aragonzkresearch/nouns-anonymous-voting) - privacy-preserving voting research project for NounsDAO

### Identity
 
- [Anon-Aadhaar](https://github.com/anon-aadhaar/anon-aadhaar-noir) - privacy-preserving verification of Aadhaar (Indian residence ID) through proofs revealing only selected identity information
- [OpenPassport](https://github.com/openpassport-org/openpassport) - identity wallet supporting privacy-preserving proofs of goverment-issued IDs
- [zkPassport](https://github.com/zkpassport/circuits) - privacy-preserving proofs of national passports

### Social

- [anon.world](https://github.com/Slokh/anonworld) - social media with optional anonymity
- [Rate Limiting Nullifiers](https://github.com/Rate-Limiting-Nullifier/noir-rln) - spam regulation in anonymous environments
- [StealthNote](https://github.com/saleel/stealthnote) - message board for people in an organization to anonymously broadcast messages

### Miscellaneous

- [Winning projects from Aztec-sponsored hackathons](https://github.com/AztecProtocol/dev-rel/tree/main/hackathons#previous-winners)

## Learning

### Interactive Tutorials

- [NoirGuardians](https://www.noirguardians.io/)
  - 3 quests that use storytelling and lore to teach basic programming in Noir, along with some advanced features that Noir offers
  - Get a first introduction to the Noir language, and learn how to integrate Noir programs into Solidity contracts
- [Zeronaut](https://github.com/eternauta1337/zeronaut) 

### Educational Curriculums

- [ZKCamp's Open Source Noir course](https://github.com/ZKCamp/aztec-noir-course)
  - 6 lectures to give participants the knowledge and skills necessary to build decentralized applications based on ZKPs using Noir
  - Lessons include ZKP Fundamentals; An Introduction to Aztec Ecosystem; Noir Basics; Building a Noir Application; and Advanced Noir
- [Video Series] [BattleZips-Noir](https://www.youtube.com/playlist?list=PLWACGbvIsEgnR2aUCr9i-PpmTVhF5Zuik) ([Source Code](https://github.com/BattleZips/BattleZips-Noir))
  - Walkthrough of building an on-chain Battleships game using zero-knowledge
  - Follow along and build your own game using Noir
 
### Examples

- [Noir Examples](https://github.com/noir-lang/noir-examples) - reference examples of zero-knowledge applications in Noir
- [Circuit Examples](https://github.com/thor314/circuit-examples) - demonstration implementation of dot products & Merkle proofs in Noir, Circom and RISC0

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
- [1.5 hrs] [ZK dApps - Why, What and How?](https://www.youtube.com/watch?v=DpCbeGcX0cI)
- [1.5 hrs] [Sudoku in Noir](https://drive.google.com/file/d/1D4XCdiIZVjUW1JHDoMW3pG-15mgjMm9E/) ([Source Code](https://github.com/guipublic/crypdoku))
- [2 hrs] [ZK HACK III - Introduction to Noir](https://www.youtube.com/watch?v=5CziMfChveY) ([Source Code](https://github.com/joss-aztec/quadratic_voting_noir))
  - Code-together: Quadratic Voting
- [1.1 hrs] [Noir on Scroll Workshop](https://www.youtube.com/watch?v=xLQfMu-shYA) ([Part of Source Code](https://github.com/Turupawn/NoirScrollDemo))

### Blog Posts & Articles

- [Understanding the Technical Aspects of Aztec and Noir](https://hackmd.io/XZX9_pZ8Q1aa_ySDPeQopg)
- Noir 101 for Solidity devs in ([English](https://mirror.xyz/crisgarner.eth/IRRxnP-HVP-7qLZ-bTI2HRpKTmSRPCDl-Q6gm2NTj4g)) and ([Spanish](https://mirror.xyz/crisgarner.eth/Iek7PhbhU4WpIJ6eixFq80_7R6czH7fbdCoN0Bd7NfI))
- [Privacy-preserving KYC with Noir](https://medium.com/@tisura/privacy-preserving-kyc-57002ab8d3f2)
- [An incomplete guide to zk-KYC apps](https://medium.com/@tisura/an-incomplete-guide-to-zk-kyc-apps-d7b4c684795c)

### International Resources

- [Introduction to Noir in Spanish](https://www.youtube.com/watch?v=m4P-sAqa8_o)
  - ([Written Tutorial and Code](https://dev.to/turupawn/circuitos-de-aztec-noir-en-tu-navegador-zk-es-semana-3-78a))
- [Building a ZK dApp in Cantonese](https://www.youtube.com/watch?v=IAQrO1j20pg)
  - [Slides](https://docs.google.com/presentation/d/1Zh8McXfdjREg0Y6iG9Q1_d-8Sgi7QT_7gJdOSmLqEEI/)

## Contribute

Propose link additions by visiting [README.md](./README.md) and click the "pen" icon in the top right corner. Make changes to the file and follow the instructions to create a pull request.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
