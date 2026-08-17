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
  - [Infrastructure](#infrastructure)
- [Libraries](#libraries)
  - [General](#general)
  - [Data Types](#data-types)
  - [Text & Encoding](#text--encoding)
  - [Collections](#collections)
  - [Cryptography](#cryptography)
    - [Elliptic Curves](#elliptic-curves)
    - [Hashes](#hashes)
    - [Encryption](#encryption)
    - [Signatures](#signatures)
    - [Merkle Trees](#merkle-trees)
  - [Ethereum](#ethereum)
  - [Media](#media)
- [Developer Tools](#developer-tools)
  - [AI Agentic Skills](#ai-agentic-skills)
  - [SDK](#sdk)
  - [Cross-platform](#cross-platform)
    - [Browser development](#browser-development)
    - [Mobile development](#mobile-development)
  - [IDE](#ide)
  - [Linting & debugging](#linting--debugging)
  - [Performance analysis](#performance-analysis)
  - [Security](#security)
  - [Library-related](#library-related)
  - [Private Shared States](#private-shared-states)
  - [Proving Backends](#proving-backends)
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

- [Payy](https://payy.network/) ([source code](https://github.com/polybase/payy)) - private stablecoin payments
- [Stellar Confidential Tokens](https://developers.stellar.org/docs/build/apps/privacy#confidential-tokens) ([source code](https://github.com/OpenZeppelin/stellar-contracts/tree/main/packages/tokens/src/confidential)) - Stellar token standard with private balances and transfer amounts
- Zerosats ([source code](https://github.com/zerosats/zerosats)) - private Bitcoin payments

### Social

- [anoncast](https://anoncast.org/) ([source code](https://github.com/Slokh/anoncast)) - anonymous X and Farcaster posting

### Infrastructure

- [Aztec](https://aztec.network/) ([source code](https://github.com/AztecProtocol/aztec-packages)) - privacy-first blockchain supporting smart contracts in Noir
- [Interfold](https://www.theinterfold.com/) ([source code](https://github.com/gnosisguild/interfold)) - private shared state protocol

## Libraries

### General

- [Standard Library](https://github.com/noir-lang/noir/tree/master/noir_stdlib) - standard library that ships with all Noir releases
- [ZK Kit Noir](https://github.com/privacy-scaling-explorations/zk-kit.noir) - collection of algorithm and utility libraries from Privacy & Scaling Explorations
- [nodash](https://github.com/olehmisar/nodash) - utility library for various data types, inspired by Lodash

### Data Types

- [BigNum](https://github.com/noir-lang/noir-bignum) - arithmetic computations of large unsigned integers of any length
- [IEEE754 Floating-point](https://github.com/sparq-org/noir_IEEE754) - IEEE 754-compliant floating-point arithmetic library supporting single and double precision
- [wad.nr Fixed-point](https://github.com/merkle-groot/wad.nr) - 18-decimal fixed-point arithmetics
- [Noir Dates](https://github.com/madztheo/noir-date) - A Noir library to parse and abstract away Dates

### Text & Encoding

- [Base64](https://github.com/noir-lang/noir_base64) - a library for base64 encoding
- [JSON parser](https://github.com/noir-lang/noir_json_parser) - JSON string parsing, adheres to [IETF RFC 8259](https://datatracker.ietf.org/doc/html/rfc8259)
- [String Search](https://github.com/noir-lang/noir_string_search) - proof of substring existence within a larger string
- [XPath 2.0 Functions](https://github.com/sparq-org/noir_XPath) - XPath 2.0 functions and operations (string, numeric, date/time, boolean); conformance-tested against W3C test-suite-derived cases

### Collections

- [Sort](https://github.com/noir-lang/noir_sort) - efficient sorting of fixed-sized arrays
- [Sparse Array](https://github.com/noir-lang/sparse_array) - efficient immutable and mutable sparse arrays

### Cryptography

#### Elliptic Curves

- [BigCurve](https://github.com/noir-lang/noir_bigcurve) - operations over elliptic curves instantiated with an arbitrary prime field

#### Hashes

- [Keccak256](https://github.com/noir-lang/keccak256) - Keccak256 hashes
- [MiMC](https://github.com/noir-lang/mimc) - MiMC hashes
- [Poseidon](https://github.com/noir-lang/poseidon) - Poseidon and Poseidon2 hashes
- [RIPEMD160](https://github.com/distributed-lab/noir-ripemd160) - RIPEMD160 hashes
- [SHA256](https://github.com/noir-lang/sha256) - SHA256 hashes
- [SHA512](https://github.com/noir-lang/sha512) - SHA512 and SHA384 hashes

#### Encryption

- [ECDH](https://github.com/privacy-scaling-explorations/zk-kit.noir/tree/main/packages/ecdh) - simple implementation of ECDH on the Baby Jubjub curve
- [RLWE Gadgets](https://github.com/aryaethn/noir-rlwe-gadgets) - verify Ring-LWE / BFV encryption via Schwartz-Zippel random-evaluation, useful for verifiable lattice-based cryptography and FHE


#### Signatures

- [EdDSA](https://github.com/noir-lang/eddsa) - EdDSA signature verification
- [ECDSA](https://github.com/zkpassport/noir-ecdsa) - ECDSA (NIST and Brainpool curves) signature verification
- [RSA](https://github.com/zkpassport/noir_rsa) - RSA signature verification
- [Schnorr](https://github.com/noir-lang/schnorr) - Schnorr signature verification
- [zkQES](https://github.com/d3mage/zk-QES/) - PDF and XML document signature verification

#### Merkle Trees

- [ZK-Kit: Merkle Trees](https://github.com/privacy-scaling-explorations/zk-kit.noir/tree/main/packages/merkle-trees) - verification of (non-)membership proofs and add/update/delete leaves

### Ethereum

- [ECrecover](https://github.com/colinnielsen/ecrecover-noir) - ECDSA signature verification and return of source Ethereum address
- [EIP-712](https://github.com/geovgy/eip712-noir) - EIP-712 typed data hashing
- [Ethereum MPT Proof](https://github.com/RadNi/mpt-noir) - proving Ethereum Merkle Patricia Trie with recursive proof aggregations
- [Ethereum Storage Proof](https://github.com/noir-lang/eth-proofs) - proving and verifying historical Ethereum / EVM accounts, storage, logs, receipts & transactions; forked from vlayer-monorepo, updated for compatibility with recent Noir releases, including modernizing outdated patterns

### Media

- [Apertrue](https://github.com/Apertrue/circuits) - proving authenticity of photos and videos through C2PA signatures from trusted devices

## Developer Tools

### AI Agentic Skills

- [Privacy Apps with Noir](https://ethskills.com/noir/SKILL.md) by ETHSKILLS
- [Writing Idiomatic Noir](https://github.com/noir-lang/noir/blob/master/.claude/skills/noir-idioms/SKILL.md) by the Noir team
- [ACIR Optimization Loop](https://github.com/noir-lang/noir/blob/master/.claude/skills/noir-optimize-acir/SKILL.md) by the Noir team
- [Noir Circuit Auditor](https://github.com/0xVikasRushi/noir-claude-auditor) by 0xVikasRushi

### SDK

- [ZKPassport](https://zkpassport.id/) - proving information in national passports
- [ZKProofport](https://zkproofport.app) - proving Coinbase attestations, Google Workspace and Microsoft 365 memberships
- [ZK Email](https://zk.email/) - proving email senders and/or contents

### Cross-platform

#### Browser development

- [NoirJS](https://noir-lang.org/docs/tutorials/noirjs_app) - compile and execute Noir programs in JavaScript / TypeScript
- [Noir Codegen for TypeScript](https://noir-lang.org/docs/reference/noir_codegen) - generate TypeScript bindings for computing Noir program outputs in TS

#### Mobile development

- [MoPro](https://github.com/zkmopro) by PSE - prove and verify Noir programs on mobile (Android and iOS)
- [Noir.rs](https://github.com/zkpassport/noir_rs) by ZKPassport - prove and verify Noir programs with Rust
- [Swoir](https://github.com/Swoir/swoir) by ZKPassport - prove and verify Noir programs with Swift on iOS and MacOS
- [Noir Android](https://github.com/madztheo/noir_android) by ZKPassport - prove and verify Noir programs with Kotlin on Android

### IDE

- [Noir Playground](https://www.noir-playground.app/) ([source code](https://github.com/0xandee/noir-playground)) - in-browser development environment
- [VS Code Extension](https://marketplace.visualstudio.com/items?itemName=noir-lang.vscode-noir) ([source code](https://github.com/noir-lang/vscode-noir))
- [Neovim Plugin](https://github.com/noir-lang/noir-nvim)
- [Zed Plugin](https://github.com/shuklaayush/zed-noir)
- [Emacs Tree-sitter Plugin](https://melpa.org/#/noir-ts-mode) ([source code](https://github.com/hhamud/noir-ts-mode))
- [tree_sitter_noir](https://github.com/tsujp/tree_sitter_noir) - tree-sitter grammar

### Linting & debugging

- [aztec-lint](https://github.com/NethermindEth/aztec-lint) by Nethermind - static analyzer for Aztec.nr contracts, also works with vanilla Noir programs
- [VS Code Debugger](https://noir-lang.org/docs/tooling/debugger)
- [CodeTracer](https://github.com/metacraft-labs/codetracer) - time-travelling debugger with Noir support

### Performance analysis

- [Noir + Barretenberg Profiler](https://github.com/noir-lang/noir/tree/master/tooling/profiler) - flamegraph opcode, execution and proving costs
- [noir-web](https://github.com/gnosisguild/noir-web) – benchmark proving and verification of Noir programs on the browser

### Security

- [Lampe](https://github.com/reilabs/lampe) by Reilabs - formal verification of Noir programs with Lean

### Library-related

- [Merkle Tree Generator](https://github.com/eyalron33/mpz/) - generate Noir-library-friendly Pedersen based Merkle trees
- [Poseidon2 in TypeScript](https://github.com/zkpassport/poseidon2) - a Poseidon2 library in pure TypeScript with support for the implementation used by Noir (over BN254)
- [Poseidon2 in Solidity](https://github.com/platus-xyz/poseidon2-solidity) - for the BN254 scalar field, implemented in Solidity with inline Yul for gas efficiency.

### Private Shared States

- [coSNARKs](https://github.com/TaceoLabs/co-snarks) - generate witness and prove Noir programs in a Multi-Party Computation network
- [Kalypso](https://docs.kalypso.org/tutorials/noir-circuits/) - generate witness and prove Noir programs in Trusted Execution Environments

### Proving Backends

- [Barretenberg (UltraHonk / MegaHonk)](https://github.com/AztecProtocol/barretenberg) by Aztec Foundation
  - [Solidity verifier](https://barretenberg.aztec.network/docs/how_to_guides/how-to-solidity-verifier) by Aztec Foundation
  - [Rust verifier](https://github.com/NethermindEth/rs-soroban-ultrahonk) by Nethermind and Stellar Development Foundation
- [coSNARKs](https://github.com/TaceoLabs/co-snarks) by Taceo Labs
- [ProveKit (Spartan + WHIR)](https://github.com/worldfnd/ProveKit) by World
- [Sonobe (Nova, HyperNova)](https://github.com/privacy-scaling-explorations/sonobe) by 0xPARC and PSE
- [Sunspot (Groth16)](https://github.com/reilabs/sunspot) by Reilabs

## Contribute

Propose link additions by [editing the README.md](https://github.com/noir-lang/awesome-noir/edit/main/README.md). We welcome and appreciate your contributions — thank you for helping improve this list!

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
