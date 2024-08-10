# awesome zk verifier
> [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
> A curated list of awesome things related to zero knowledge proof verifiers.

## Contents

- [Awesome zk verifier](#awesome-zk-verifier)
  -  [Circuit Verifier](#Circuit-Verifier)
     - [Groth16 Circuit Verifier](#Groth16-Circuit-Verifier)
     - [Halo2 Circuit Verifier](#Halo2-Circuit-Verifier)
     - [Plonky2 Circuit Verifier](#Plonky2-Circuit-Verifier)
     - [Boojum Circuit Verifier](#Boojum-Circuit-Verifier)
     - [Plonky3 Circuit Verifier](#Plonky3-Circuit-Verifier)
  -  [Contract Verifier](#Contract-Verifier)


## Circuit Verifier

Verify proof by zk prover circuit. Aka. aggregation prove.

### Groth16 Circuit Verifier
  * https://github.com/xycloo/wasm-groth16-verifier
### Halo2 Circuit Verifier:
  * https://github.com/privacy-scaling-explorations/snark-verifier

### Plonky2 Circuit Verifier
  * https://github.com/succinctlabs/gnark-plonky2-verifier
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


### Circuit Verifier by zkvm
> As the raw verifier of a prover is a program(most of them writen in Rust), which can be proven by a zkvm. So that we can generate aggregationg proof by zkvm instead of writing a aggregation circuit.

* Verify c-kzg proof:
  * https://github.com/smtmfft/sp1-c-kzg
    
* Verify fflonk proof:
  * https://github.com/RizeLabs/sp1-fflonk
    
* Verify plonky2 proof:
  * https://github.com/wborgeaud/sp1-plonky2
    
* Verify platinum proof:
  * https://github.com/raphaelDkhn/sp1_recursion


## Contract Verifier
> Verify proof by onchain contract.

### bitcoin Script: Verify zkp proof in bitcoin Script

* Groth16
  * https://github.com/zulu-network/bitvm-groth16-verifier
  * https://github.com/chainwayxyz/bitvm-zk-verifier
    
* ffloink
  * https://github.com/BitVM/BitVM/pull/69
* circle stark(aka.stwo)
  * https://github.com/Bitcoin-Wildlife-Sanctuary/bitcoin-circle-stark

 
### Solidity: Verify zkp proof in Solidity Contract
* Groth16
  * https://github.com/recmo/evm-groth16

* plonk
  * https://github.com/matter-labs/solidity_plonk_verifier
  * https://github.com/DelphinusLab/delphinus-solidity
  * https://github.com/fluidex/solidity_recursive_plonk_verifier

* halo2
  * https://github.com/privacy-scaling-explorations/halo2-solidity-verifier
  * https://github.com/akinovak/instance-verifier
  
* plonky2
  * https://github.com/polymerdao/plonky2-solidity-verifier

* Nova
  * https://github.com/lurk-lab/solidity-verifier
  * https://github.com/privacy-scaling-explorations/folding-schemes
    
* Mina
  * https://github.com/NilFoundation/mina-state-proof
    
* Placeholder
  * https://github.com/NilFoundation/cairo-placeholder-verification
* Sp1
  * https://github.com/RizeLabs/sp1-verifier

### Cairo: Verify zkp proof in Cairo Contract
* stark
    * https://github.com/HerodotusDev/cairo-verifier
    * https://github.com/ZeroSync/ZeroSync/tree/main/src/stark_verifier
* snark(Pairing)
   * https://github.com/keep-starknet-strange/garaga Including Groth16 and protostar's test demos.
* circom
  * https://github.com/lambdaclass/circom_export_to_cairo
* Placeholder
    * https://github.com/NilFoundation/cairo-placeholder-verification

### Solona: Verify zkp proof in Solona Contract
* Groth16
  * https://github.com/zkLinkProtocol/groth16-sol-verifier
  * https://github.com/gnosed/solana_groth16_verifier

### Move: Verify zkp proof in Move Contract
* Groth16
  * https://github.com/MystenLabs/sui/blob/main/sui_programmability/examples/crypto/sources/groth16.move
* halo2
  * https://github.com/zkmove/halo2-verifier.move


