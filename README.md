# Awesome Noir

A curated list of resources for programming with Noir.

⚠️ Projects listed are not endorsed as safe and secure by the Noir team. Users are advised to exercise caution before utilizing any content or code provided herein.

[![Awesome](https://img.shields.io/badge/Awesome-Repo-blue?logo=awesome-lists&style=flat)](https://awesome.re)
[![X (formerly Twitter) Follow](https://img.shields.io/twitter/follow/NoirLang)](https://x.com/NoirLang)
[![Discord](https://img.shields.io/badge/Discord-5865F2?logo=discord&logoColor=white&labelColor=5865F2&style=flat&labelWidth=100)](https://discord.com/invite/RJdCBN373S)

## Contents

<!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->

- [Resources](#resources)
  - [Benchmarks](#benchmarks)
- [Applications](#applications)
  - [Finance](#finance)
  - [Social](#social)
- [Libraries](#libraries)
  - [General](#general)
  - [Data Types](#data-types)
    - [Numerics](#numerics)
    - [Dates & Times](#dates--times)
  - [Data Type Manipulation](#data-type-manipulation)
    - [General](#general-1)
    - [Numerics](#numerics-1)
    - [Bytes](#bytes)
    - [Texts](#texts)
    - [Collections](#collections)
  - [Cryptography](#cryptography)
    - [Elliptic Curves](#elliptic-curves)
    - [Hashes](#hashes)
    - [Encryption](#encryption)
    - [Signatures](#signatures)
    - [Merkle Trees](#merkle-trees)
    - [Message Authentication Code](#message-authentication-code)
    - [Randomness](#randomness)
  - [Blockchain Specifics](#blockchain-specifics)
    - [Aztec](#aztec)
    - [Ethereum](#ethereum)
    - [Bitcoin](#bitcoin)
  - [Social](#social-1)
  - [Machine Learning](#machine-learning)
- [Developer Tools](#developer-tools)
  - [SDK](#sdk)
  - [Infrastructure](#infrastructure)
  - [AI Agentic Skills](#ai-agentic-skills)
  - [IDE](#ide)
  - [Linting](#linting)
  - [Debugging](#debugging)
  - [Performance](#performance)
  - [Cross-platform](#cross-platform)
    - [Browser development](#browser-development)
    - [Mobile development](#mobile-development)
  - [EVM](#evm)
  - [Private shared states](#private-shared-states)
  - [Library-related](#library-related)
  - [Security](#security)
  - [Proving Backends](#proving-backends)
    - [Needs updating](#needs-updating)
- [Contribute](#contribute)
- [License](#license)

<!-- TOC end -->

---

## Resources

- [Docs](https://noir-lang.org/docs)
- [GitHub](https://github.com/noir-lang)
- [Discord](https://discord.gg/RJdCBN373S)

### Benchmarks

- [Ethproofs' Benchmarks](https://ethproofs.org/csp-benchmarks) - benchmarks of hashes and signature verifications in Noir with Barretenberg amongst other ZK stacks
- [tsujp's Hash Benchmarks](https://observablehq.com/d/83efd5e7d136c471) - benchmarks of Poseidon2, Keccak256 and SHA256 at various input sizes and iterations

## Applications

### Finance

- [Payy](https://payy.network/) - private stablecoin payments

### Social

- [anoncast](https://anoncast.org/) - anonymous X and Farcaster posting
- [Openbands](https://openbands.xyz/) - pseudonymous posting by company, nationality or age

## Libraries

For library tooling (e.g. input generators, TypeScript implementations), refer to the [library-related tooling](#library-related) section.

### General

- [Standard Library](https://github.com/noir-lang/noir/tree/master/noir_stdlib) - standard library that ships with all Noir releases
- [ZK Kit Noir](https://github.com/privacy-scaling-explorations/zk-kit.noir) - collection of algorithm and utility libraries from Privacy & Scaling Explorations

### Data Types

#### Numerics

- [BigNum](https://github.com/noir-lang/noir-bignum) - a library for arithmetic computations of large unsigned integers of any length
- [Fraction](https://github.com/resurgencelabs/fraction) - a library for accessing fractional number data types in Noir, allowing results that aren't whole numbers
- [ZKFloat](https://github.com/0x3327/ZKFloat) - a floating point library for Noir
- [IEEE754](https://github.com/jeswr/noir_IEEE754) - an IEEE 754-compliant floating-point arithmetic library supporting single and double precision
- [Complex Numbers](https://github.com/doctoruber/complexnr) - This library offers a comprehensive suite of operations for complex numbers
- [Fixed Point Library](https://github.com/doctoruber/noir-fixed-point) - The FixedPoint library offers precise fixed-point arithmetic operations tailored for Noir
- [Fixed Point Library for scale 2^-16](https://github.com/hashcloak/noir-fixed-point) - an optimized fixed point arithmetic library designed for scale 2^-16.
- [wad.nr Fixed Point Library](https://github.com/merkle-groot/wad.nr) - An 18-decimals fixed-point arithmetic library for Noir that enables safe token calculations in DeFi contracts.

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
- [Merkle Tree](https://github.com/noir-lang/merkle) - Merkle Tree implementations forked from Aztec Packages

#### Message Authentication Code

- [Noir HMAC](https://github.com/zkpersona/noir-hmac) - hash-based message authentication code

#### Randomness

- [Cryptographically Secure Pseudo-Random Number Generator](https://github.com/doctoruber/CSPRNG) - pseudo-random number generation

### Blockchain Specifics

#### Aztec

- [Aztec Storage proofs](https://github.com/nemi-fi/aztec_storage_proofs) - proving Aztec note inclusion in plain Noir, with verification in JavaScript or Solidity

#### Ethereum

- [ECrecover](https://github.com/colinnielsen/ecrecover-noir) - ECDSA signature verification and return of source Ethereum address
- [EIP-712](https://github.com/geovgy/eip712-noir) - A Noir library for EIP-712 typed data hashing
- [Ethereum MPT Proof](https://github.com/RadNi/mpt-noir) - proving Ethereum Merkle Patricia Trie with recursive proof aggregations
- [Ethereum Storage Proof](https://github.com/noir-lang/eth-proofs) - proving and verifying historical Ethereum / EVM accounts, storage, logs, receipts & transactions; forked from vlayer-monorepo, updated for compatibility with recent Noir releases, including modernizing outdated patterns

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

### SDK

- [ZKPassport](https://zkpassport.id/) - proving information in national passports
- [ZKProofport](https://zkproofport.app) - proving Coinbase attestations, Google Workspace and Microsoft 365 memberships
- [ZK Email](https://zk.email/) - proving email senders and/or contents

### Infrastructure

- [Aztec](https://aztec.network/) - privacy-first blockchain supporting smart contracts in Noir

### AI Agentic Skills

- [Privacy Apps with Noir](https://ethskills.com/noir/SKILL.md) by ETHSKILLS
- [Writing Idiomatic Noir](https://github.com/noir-lang/noir/blob/master/.claude/skills/noir-idioms/SKILL.md) by the Noir team
- [ACIR Optimization Loop](https://github.com/noir-lang/noir/blob/master/.claude/skills/noir-optimize-acir/SKILL.md) by the Noir team
- [Noir Circuit Auditor](https://github.com/0xVikasRushi/noir-claude-auditor) by 0xVikasRushi

### IDE

- [Noir Playground](https://www.noir-playground.app/) - A browser-based Noir zero-knowledge proof development environment. ([Source Code](https://github.com/0xandee/noir-playground))
- [VS Code Extension](https://marketplace.visualstudio.com/items?itemName=noir-lang.vscode-noir) - Syntax highlight, error highlight, codelens, etc. ([Source Code](https://github.com/noir-lang/vscode-noir))
- [Neovim Plugin](https://github.com/noir-lang/noir-nvim) - Syntax highlight, error highlight, etc.
- [Emacs Plugin](https://melpa.org/#/noir-mode) - Syntax highlight ([Source Code](https://github.com/hhamud/noir-mode))
- [Zed Plugin](https://github.com/shuklaayush/zed-noir) - Syntax highlight, LSP support
- [tree_sitter_noir](https://github.com/tsujp/tree_sitter_noir) - Tree-sitter grammar for Noir
- [Emacs Tree-sitter Plugin](https://melpa.org/#/noir-ts-mode) - Syntax highlight ([Source Code](https://github.com/hhamud/noir-ts-mode))
- [JetBrains Noir Language Support](https://plugins.jetbrains.com/plugin/29753-noir-language-support) - Syntax highlight and extended context features ([Source Code](https://github.com/ZKLSOL/JetBrains-Noir-Syntax-Highlight-Plugin))

### Linting

- [aztec-lint](https://github.com/NethermindEth/aztec-lint) by Nethermind - static analyzer for Aztec.nr contracts, also works with vanilla Noir programs

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

- [Lampe](https://github.com/reilabs/lampe) by Reilabs - formal verification of Noir programs with Lean
- [zk-mutant](https://github.com/mutorium/zk-mutant) - mutation testing for Noir programs
- [noir-metrics](https://github.com/mutorium/noir-metrics) - source code metrics for Noir programs with machine-friendly JSON outputs

### Proving Backends

- [Barretenberg (UltraHonk / MegaHonk)](https://github.com/AztecProtocol/barretenberg) by Aztec Labs
- [coSNARKs](https://github.com/TaceoLabs/co-snarks) by Taceo Labs
- [ProveKit (Spartan + WHIR)](https://github.com/worldfnd/ProveKit) by World
- [Sonobe (Nova, HyperNova)](https://github.com/privacy-scaling-explorations/sonobe) by 0xPARC and PSE
- [Sunspot (Gnark Groth16)](https://github.com/reilabs/sunspot) by Reilabs

#### Needs updating

- [Plonky2](https://github.com/blocksense-network/noir) by Blocksense
- [Edge (Supernova)](https://github.com/pluto/edge) by Pluto
- [Gnark](https://github.com/lambdaclass/noir_backend_using_gnark) by Lambdaclass
- [Groth16](https://github.com/TomAFrench/acvm-backend-groth16) by Tom
- [Halo2](https://github.com/Ethan-000/halo2_backend) by Ethan
- [Marlin](https://github.com/noir-lang/marlin_arkworks_backend) by Noir team
- [Plonky2](https://github.com/eryxcoop/acvm-backend-plonky2) by Eryx
- [Plonky3](https://github.com/vacekj/air-fried-gyatt) by Josef

## Contribute

Propose link additions by [editing the README.md](https://github.com/noir-lang/awesome-noir/edit/main/README.md). We welcome and appreciate your contributions — thank you for helping improve this list!

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
