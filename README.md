# A(n almost) complete atlas of Zero-Knowledge Proof technologies

Most of the blocks are clickable!

```mermaid
graph TD
    TypeScript --- SnarkyJS
    Rust ---- Bellman
    Circom ---- snarkjs 
    Circom --- R1CS
    snarkjs --- PLONK
    snarkjs --- Groth16
    R1CS --- snarkjs
    R1CS --- PLONK
    R1CS --- Groth16
    ZoKrates --- R1CS
    Leo --- R1CS
    Bellman --- PLONK
    Noir --- ACIR
    Marlin --- QAP
    Lurk ----- Groth16
    Lurk ----- SnarkPack[SnarkPack+]
    Lurk ----- Nova
    Groth16 --- QAP
    PLONK --- QAP
    SnarkPack --- QAP
    Nova --- QAP
    ACIR ---- PLONK
    ACIR ---- Groth16
    ACIR ---- Marlin
    QAP --- zkSNARK
    SnarkyJS ---- PLONK
    Cairo --- RAP
    RAP ------ zkSTARK
    
    subgraph Legend
        direction LR
        Lang([Language])---Framework([Framework])---Compiler([Compiler])---Intermediate([Intermediate Format])---Library([Library])---ProvingSystem([Proving System])---AlgebraicForm([Algebraic Form])---Tech([Technology])
    end
    
    classDef framework fill:#f94144,color:#fff
    classDef lang fill:#277da1,color:#fff
    classDef compiler fill:#f8961e
    classDef intermediate fill:#f9844a
    classDef lib fill:#f9c74f
    classDef provingSystem fill:#90be6d
    classDef algForm fill:#43aa8b
    classDef tech fill:#4d908e,color:#fff
    classDef color9 fill:#f3722c
    classDef color10 fill:#577590
    
    class Framework,SnarkyJS framework
    class Lang,Circom,ZoKrates,Leo,Noir,Cairo,Lurk,Rust,TypeScript lang
    class Compiler compiler
    class Intermediate,R1CS,ACIR,RAP intermediate
    class Library,snarkjs,Bellman lib
    class ProvingSystem,Groth16,PLONK,Marlin,SnarkPack,Nova provingSystem
    class AlgebraicForm,QAP algForm
    class Tech,zkSNARK,zkSTARK tech
    
    click Circom href "https://docs.circom.io/"
    click ZoKrates href "https://zokrates.github.io/"
    click Leo href "https://leo-lang.org/"
    click Noir href "https://docs.aztec.network/developers/noir"
    click snarkjs href "https://github.com/iden3/snarkjs"
    click Cairo href "https://eprint.iacr.org/2021/1063.pdf"
    click RAP href "https://eprint.iacr.org/2021/1063.pdf"
    click Lurk href "https://github.com/lurk-lang"
    click SnarkPack href "https://research.protocol.ai/blog/2021/snarkpack-how-to-aggregate-snarks-efficiently/"
    click Nova href "https://github.com/microsoft/Nova"
    click Bellman href "https://github.com/matter-labs/bellman"
    click Rust href "https://www.rust-lang.org/"
    click SnarkyJS href "https://github.com/o1-labs/snarkyjs"
    click TypeScript href "https://www.typescriptlang.org/"
    click ACIR href "https://noir-lang.github.io/book/acir.html"
    click PLONK href "https://eprint.iacr.org/2019/953.pdf"
    click Groth16 href "https://eprint.iacr.org/2016/260.pdf"
    click Marlin href "https://eprint.iacr.org/2019/1047.pdf"
    click zkSTARK href "https://eprint.iacr.org/2018/046.pdf"
```
---
Inspired by [https://harryr.github.io/zklangs/](https://harryr.github.io/zklangs/).
This diagram is using [Mermaid syntax](https://mermaid-js.github.io/mermaid/#/).
