# awesome zk verifier
> [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
> A curated list of awesome things related to zero knowledge proof verifiers.

## Contents

- [Awesome zk verifier](#awesome-zk-verifier)
  - [Verifier Layer](#verifier-layer)
  - [Circuit Verifier](#circuit-verifier)
    - [Groth16 Circuit Verifier](#Groth16-Circuit-Verifier)
    - [Halo2 Circuit Verifier](#Halo2-Circuit-Verifier)
    - [Plonky2 Circuit Verifier](#Plonky2-Circuit-Verifier)
    - [Boojum Circuit Verifier](#Boojum-Circuit-Verifier)
    - [Plonky3 Circuit Verifier](#Plonky3-Circuit-Verifier)
    - [zkVM Circuit Verifier](#zkVM-Circuit-Verifier)
      - [KZG zkVM Circuit Verifier](#KZG-zkVM-Circuit-Verifier)
      - [Fflonk zkVM Circuit Verifier](#Fflonk-zkVM-Circuit-Verifier)
      - [Plnoky2 zkVM Circuit Verifier](#Plnoky2-zkVM-Circuit-Verifier)
      - [Platinum zkVM Circuit Verifier](#platinum-zkvm-circuit-verifier)
  - [Contract Verifier](#Contract-Verifier)
    - [Bitcoin Script Verifier](#bitcoin-script-verifier)
      - [Groth16 Bitcoin Script Verifier](#groth16-bitcoin-script-verifier)
      - [Fflonk Bitcoin Script Verifier](#Fflonk-bitcoin-script-verifier)
      - [Circle Stark Bitcoin Script Verifier](#circle-stark-bitcoin-script-verifier)
    - [Solidity Verifier](#solidity-verifier)
      - [Groth16 Solidity Verifier](#groth16-solidity-verifier)
      - [Fflonk Solidity Verifier](#fflonk-solidity-verifier)
      - [Plonk Solidity Verifier](#Plonk-solidity-verifier)
      - [Halo2 Solidity Verifier](#Halo2-solidity-verifier)
      - [Plonky2 Solidity Verifier](#Plonky2-solidity-verifier)
      - [Marlin Solidity Verifier](#marlin-solidity-verifier)
      - [Nova Solidity Verifier](#Nova-solidity-verifier)
      - [gm17 Solidity Verifier](#gm17-solidity-verifier)
      - [Mina Solidity Verifier](#Mina-solidity-verifier)
      - [Placeholder Solidity Verifier](#Placeholder-solidity-verifier)
      - [Sp1 Solidity Verifier](#Sp1-solidity-verifier)
    - [Cairo Verifier](#cairo-verifier)
      - [Stark Cairo Verifier](#Stark-Cairo-verifier)
      - [Snark Cairo Verifier](#Snark-Cairo-verifier)
      - [Circom Cairo Verifier](#Circom-Cairo-verifier)
      - [Placeholder Cairo Verifier](#Placeholder-Cairo-verifier)
    - [Solona Verifier](#solona-verifier)
      - [Groth16 Solona Verifier](#groth16-Solona-verifier)
    - [Move Verifier](#move-verifier)
      - [Groth16 Move Verifier](#groth16-Move-verifier)
      - [Halo2 Move Verifier](#groth16-Halo2-verifier)
    - [Cosmwasm Verifier](#cosmwasm-verifier)
      - [Groth16 Cosmwasm Verifier](#groth16-cosmwasm-verifier)
      - [Plonk Cosmwasm Verifier](#plonk-cosmwasm-verifier)
  - [Other Verifiers](#other-verifiers)
    - [Gnark Arkworks Verifier](#gnark-arkworks-verifier)
    - [Groth16 Wasm Verifier](#groth16-wasm-verifier)
    - [Fflonk Verifier](#fflonk-verifier)
    - [Snarkjs Verifier](#snarkjs-verifier)

## Verifier Layer
### Aligened Layer
* https://github.com/yetanotherco/aligned_layer
### zkVerify
* https://github.com/HorizenLabs/zkVerify
### hyle
* https://github.com/Hyle-org/hyle

## Circuit Verifier

Verify zkp'sproof by (another) zk prover circuit. Aka. aggregation prove.

### Groth16 Circuit Verifier
* https://github.com/filecoin-project/bellperson/tree/master/src/groth16/aggregate
* https://github.com/nikkolasg/snarkpack


### Halo2 Circuit Verifier:
* https://github.com/privacy-scaling-explorations/snark-verifier

### Plonky2 Circuit Verifier
* https://github.com/arnaucube/plonky2-recursion-experiment
* https://github.com/succinctlabs/gnark-plonky2-verifier
* https://github.com/Lagrange-Labs/mapreduce-plonky2/tree/main/gnark-utils
* https://github.com/zkMIPS/gnark-plonky2-verifier
* https://github.com/polymerdao/plonky2-circom
* https://github.com/maxgillett/halo2-fri-gadget
* https://github.com/shuklaayush/halo2-plonky2-verifier
* https://github.com/Omniverse-Web3-Labs/fri-kzg-verifier
* https://github.com/DoHoonKim8/stark-verifier
  * https://github.com/qope/another-circuit
* https://github.com/cf/gnark-plonky2-verifier/blob/c59e33fd8f1b407b355d7b9a74e34792e7c78f37/prover/src/lib.rs#L24-L40

### Boojum Circuit Verifier
* https://github.com/matter-labs/snark-wrapper

### Plonky3 Circuit Verifier
* https://github.com/succinctlabs/sp1/tree/main/recursion/gnark-ffi/go/sp1
* https://github.com/QEDProtocol/plonky2.5
* https://github.com/taikoxyz/gnark-plonky3-verifier
  

* Verify zkvm by another one?
* https://github.com/jimzk/sp1-recursive
* https://github.com/Bisht13/sp1-recursive-plonk


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
* https://github.com/zulu-network/bitvm-groth16-verifier
* https://github.com/chainwayxyz/bitvm-zk-verifier
    
#### Fflonk Bitcoin Script Verifier
* https://github.com/BitVM/BitVM/pull/69

#### Circle Stark Bitcoin Script Verifier
* https://github.com/Bitcoin-Wildlife-Sanctuary/bitcoin-circle-stark

### Solidity Verifier
Verify zkp proof in Solidity Contract

#### Groth16 Solidity Verifier
* https://github.com/recmo/evm-groth16
* https://github.com/succinctlabs/sp1-contracts/blob/main/contracts/src/v3.0.0-rc1/Groth16Verifier.sol
* https://github.com/circuitscan/snarkjs-groth16-multi-verifier/blob/main/test/contracts/semaphorev4-1.sol


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
Following contains verifier by other crypto implement.
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