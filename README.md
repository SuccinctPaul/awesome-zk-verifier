# awesome-zk-verifer


## Circuit Verifier
> Verify proof by zk prover circuit. Aka. aggregation prove.

* Verifier groth16 proof:
  * https://github.com/xycloo/wasm-groth16-verifier
* Verify halo2(kzg) proof:
  * https://github.com/privacy-scaling-explorations/snark-verifier
      
* Verify plonky2 proof:
  * https://github.com/succinctlabs/gnark-plonky2-verifier
  * https://github.com/polymerdao/plonky2-circom
  * https://github.com/maxgillett/halo2-fri-gadget
  * https://github.com/shuklaayush/halo2-plonky2-verifier
  * https://github.com/Omniverse-Web3-Labs/fri-kzg-verifier
  * https://github.com/DoHoonKim8/stark-verifier
    * https://github.com/qope/another-circuit
  * https://github.com/cf/gnark-plonky2-verifier/blob/c59e33fd8f1b407b355d7b9a74e34792e7c78f37/prover/src/lib.rs#L24-L40
    
* Verify Boojum proof:
  * https://github.com/matter-labs/snark-wrapper

* Verify plonky3 proof:
  * https://github.com/succinctlabs/sp1/tree/main/recursion/groth16
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


## Contract  Verifier
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


