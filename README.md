<div align="center">
  <h1 align="center">awesome zk verifier</h1>

A curated list of awesome things related to zero knowledge proof verifiers. 

Inculding: onchain zk proof verifier, recursive zk proof verifier etc.

  <p align="center">
    <a href="https://github.com/sindresorhus/awesome">
      <img alt="awesome list badge" src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg">
    </a>
    <a href="https://github.com/SuccinctPaul/awesome-zk-verifier/graphs/contributors">
      <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/SuccinctPaul/awesome-zk-verifier">
    </a>
    <a href="http://makeapullrequest.com">
      <img alt="pull requests welcome badge" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat">
    </a>
  </p>

</div>


## Contents

- [Awesome zk verifier](#awesome-zk-verifier)
  - [Circuit Verifier](#circuit-verifier)
    - [Groth16 Circuit Verifier](#Groth16-Circuit-Verifier)
    - [Halo2 Circuit Verifier](#Halo2-Circuit-Verifier)
    - [Plonky2 Circuit Verifier](#Plonky2-Circuit-Verifier)
    - [Plonky3 Circuit Verifier](#Plonky3-Circuit-Verifier)
    - [Boojum Circuit Verifier](#Boojum-Circuit-Verifier)
    - [Winterfell Circuit Verifier](#winterfell-circuit-verifier)
    - [zkVM Circuit Verifier](#zkVM-Circuit-Verifier)
  - [Contract Verifier](#Contract-Verifier)
    - [Bitcoin Script Verifier](#bitcoin-script-verifier)
    - [Solidity Verifier](#solidity-verifier)
    - [Cairo Verifier](#cairo-verifier)
    - [Solona Verifier](#solona-verifier)
    - [Move Verifier](#move-verifier)
    - [Cosmwasm Verifier](#cosmwasm-verifier)
  - [Other Verifiers](#other-verifiers)
    - [Gnark Arkworks Verifier](#gnark-arkworks-verifier)
    - [Groth16 Wasm Verifier](#groth16-wasm-verifier)
    - [Fflonk Verifier](#fflonk-verifier)
    - [Snarkjs Verifier](#snarkjs-verifier)
  - [Related Awesome Lists](#related-awesome-lists)

## Circuit Verifier

Verify zkp'sproof by (another) zk prover circuit. Aka. aggregation/recursive prove.

### Groth16 Circuit Verifier
* By snarkpack
  * https://github.com/filecoin-project/bellperson/tree/master/src/groth16/aggregate
  * https://github.com/nikkolasg/snarkpack


### Halo2 Circuit Verifier:
* https://github.com/privacy-scaling-explorations/snark-verifier

### Plonky2 Circuit Verifier
* https://github.com/arnaucube/plonky2-recursion-experiment
* By gnark
  * https://github.com/succinctlabs/gnark-plonky2-verifier
  * https://github.com/Lagrange-Labs/mapreduce-plonky2/tree/main/gnark-utils
  * https://github.com/zkMIPS/gnark-plonky2-verifier
  * https://github.com/cf/gnark-plonky2-verifier/blob/c59e33fd8f1b407b355d7b9a74e34792e7c78f37/prover/src/lib.rs#L24-L40
* By circom
  * https://github.com/polymerdao/plonky2-circom
* By halo2
  * https://github.com/maxgillett/halo2-fri-gadget
  * https://github.com/shuklaayush/halo2-plonky2-verifier
  * https://github.com/Omniverse-Web3-Labs/fri-kzg-verifier
  * https://github.com/DoHoonKim8/stark-verifier
  * https://github.com/qope/another-circuit
* by groth16
  * https://github.com/Electron-Labs/plonky2-groth16-verifier
  
### Plonky3 Circuit Verifier
* By gnark
  * https://github.com/succinctlabs/sp1/tree/main/recursion/gnark-ffi/go/sp1
* By plonky2
  * https://github.com/QEDProtocol/plonky2.5


### Boojum Circuit Verifier
* https://github.com/matter-labs/snark-wrapper

### Winterfell Circuit Verifier
* By circom
  * https://github.com/VictorColomb/stark-snark-recursive-proofs


### zkVM Circuit Verifier
As the raw verifier of a prover is a program(most of them writen in Rust), which can be proven by a zkvm. 
So that we can generate aggregationg proof by zkvm instead of writing a aggregation circuit.

#### KZG zkVM Circuit Verifier
* https://github.com/smtmfft/sp1-c-kzg

#### Fflonk zkVM Circuit Verifier
* https://github.com/RizeLabs/sp1-fflonk

#### Plonky2 zkVM Circuit Verifier
* https://github.com/wborgeaud/sp1-plonky2
    
#### Platinum zkVM Circuit Verifier
* https://github.com/raphaelDkhn/sp1_recursion

## Contract Verifier
> Verify proof by onchain contract.

### Bitcoin Script Verifier
Verify zkp proof in bitcoin Script

#### Groth16 Bitcoin Script Verifier
* https://github.com/chainwayxyz/bitvm-zk-verifier
* https://github.com/FairgateLabs/rust-bitvmx-zk-proof

#### Circle Stark Bitcoin Script Verifier
* https://github.com/Bitcoin-Wildlife-Sanctuary/bitcoin-circle-stark
* https://github.com/bitlayer-org/tap-stark

### Solidity Verifier
Verify zkp proof in Solidity Contract

#### Groth16 Solidity Verifier
* https://github.com/recmo/evm-groth16
* https://github.com/succinctlabs/sp1-contracts/blob/main/contracts/src/v3.0.0-rc1/Groth16Verifier.sol
* https://github.com/circuitscan/snarkjs-groth16-multi-verifier/blob/main/test/contracts/semaphorev4-1.sol

#### whir Solidity Verifier
* https://github.com/privacy-scaling-explorations/sol-whir

#### Fflonk Solidity Verifier
* https://github.com/recmo/evm-groth16
* https://github.com/0xPolygonHermez/zkevm-contracts/tree/main/contracts/verifiers

#### Plonk Solidity Verifier
* https://github.com/matter-labs/solidity_plonk_verifier
* https://github.com/DelphinusLab/delphinus-solidity
* https://github.com/fluidex/solidity_recursive_plonk_verifier
* https://github.com/matter-labs/era-contracts/blob/main/l1-contracts/contracts/state-transition/Verifier.sol
  Rust Version:
  * https://github.com/HorizenLabs/zksync-era-verifier
* https://github.com/succinctlabs/sp1-contracts/blob/main/contracts/src/v3.0.0-rc1/PlonkVerifier.sol
* https://github.com/zkVerify/ultraplonk_verifier

#### Halo2 Solidity Verifier
* https://github.com/privacy-scaling-explorations/halo2-solidity-verifier
* https://github.com/akinovak/instance-verifier

#### Plonky2 Solidity Verifier
* https://github.com/polymerdao/plonky2-solidity-verifier

#### Marlin Solidity Verifier
* https://github.com/Zokrates/ZoKrates/blob/develop/zokrates_proof_systems/src/scheme/marlin.rs

#### Nova Solidity Verifier
* https://github.com/argumentcomputer/solidity-verifier
* https://github.com/privacy-scaling-explorations/folding-schemes

#### gm17 Solidity Verifier
* https://github.com/Zokrates/ZoKrates/blob/develop/zokrates_proof_systems/src/scheme/gm17.rs
  * Rust 
    * https://github.com/arkworks-rs/gm17
    
#### Mina Solidity Verifier
* https://github.com/NilFoundation/mina-state-proof

#### Placeholder Solidity Verifier
* https://github.com/NilFoundation/cairo-placeholder-verification

#### Sp1 Solidity Verifier
* https://github.com/RizeLabs/sp1-verifier

### Cairo Verifier
Verify zkp proof in Cairo Contract

#### Stark Cairo Verifier
* https://github.com/HerodotusDev/cairo-verifier
* https://github.com/ZeroSync/ZeroSync/tree/main/src/stark_verifier

#### Snark Cairo Verifier
 * https://github.com/keep-starknet-strange/garaga Including Groth16 and protostar's test demos.

#### Circom Cairo Verifier
* https://github.com/lambdaclass/circom_export_to_cairo

#### Placeholder Cairo Verifier
* https://github.com/NilFoundation/cairo-placeholder-verification

### Solona Verifier
Verify zkp proof in Solona Contract

#### Groth16 Solona Verifier
* https://github.com/Lightprotocol/groth16-solana
* https://github.com/zkLinkProtocol/groth16-sol-verifier
* https://github.com/gnosed/solana_groth16_verifier

### Move Verifier
Verify zkp proof in Move Contract

#### Groth16 Move Verifier
* https://github.com/MystenLabs/sui/blob/main/sui_programmability/examples/crypto/sources/groth16.move

#### Halo2 Move Verifier
* https://github.com/zkmove/halo2-verifier.move


### Cosmwasm Verifier
#### Groth16 Cosmwasm Verifier
* https://github.com/DoraFactory/zk-cosmwasm/tree/main/cw-groth16

#### Plonk Cosmwasm Verifier
* https://github.com/DoraFactory/zk-cosmwasm/tree/main/cw-plonk


## Other Verifiers
Following contains verifier by other crypto-lib implement.
* eg: CryptoA's verified by cryptoB, aka `CryptoA CryptoB Verifier`

### Gnark Arkworks Verifier
* https://github.com/succinctlabs/snark-bn254-verifier
  which not using ark-groth16.
* https://github.com/Bisht13/gnark-bn254-verifier
* https://github.com/geometers/gnark-arkworks-verifier

### Groth16 Wasm Verifier
* https://github.com/xycloo/wasm-groth16-verifier

### Fflonk Verifier
* https://github.com/SuccinctPaul/ark-fflonk-verifier
* https://github.com/RizeLabs/sp1-fflonk
* https://github.com/HorizenLabs/fflonk_verifier

### Snarkjs Verifier
* https://github.com/DoraFactory/snarkjs-bellman-adapter


## Related Awesome Lists

https://github.com/seresistvanandras/awesome-evm-proof-verifiers