# A(n almost) complete atlas of Zero-Knowledge Proof technologies

Most of the blocks are clickable!

```mermaid
graph TD
    TypeScript --- SnarkyJS
    Rust ---- Bellman
    Rust --- Halo2
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
    Halo2 --- UltraPLONK
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
    UltraPLONK ---- zkSNARK
    SnarkyJS ---- PLONK
    Cairo --- RAP
    RAP ------ zkSTARK
    
    classDef framework fill:#f94144,color:#fff
    classDef lang fill:#277da1,color:#fff
    classDef compiler fill:#f8961e,color:#000
    classDef intermediate fill:#f9844a,color:#000
    classDef lib fill:#f9c74f,color:#000
    classDef provingSystem fill:#90be6d,color:#000
    classDef algForm fill:#43aa8b,color:#000
    classDef tech fill:#4d908e,color:#fff
    classDef color9 fill:#f3722c,color:#000
    classDef color10 fill:#577590,color:#000
    
    class SnarkyJS framework
    class Circom,ZoKrates,Leo,Noir,Cairo,Lurk,Rust,TypeScript lang
    class R1CS,ACIR,RAP intermediate
    class snarkjs,Bellman,Halo2 lib
    class Groth16,PLONK,Marlin,SnarkPack,Nova,UltraPLONK provingSystem
    class QAP algForm
    class zkSNARK,zkSTARK tech
    
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
    click Halo2 href "https://zcash.github.io/halo2/index.html"
```
```mermaid
graph LR
    subgraph Legend
        direction LR
        Lang([Language])---Framework([Framework])---Compiler([Compiler])---Intermediate([Intermediate Format])---Library([Library])---ProvingSystem([Proving System])---AlgebraicForm([Algebraic Form])---Tech([Technology])
    end
    
    linkStyle default stroke-width:0px;
    
    classDef framework fill:#f94144,color:#fff
    classDef lang fill:#277da1,color:#fff
    classDef compiler fill:#f8961e,color:#000
    classDef intermediate fill:#f9844a,color:#000
    classDef lib fill:#f9c74f,color:#000
    classDef provingSystem fill:#90be6d,color:#000
    classDef algForm fill:#43aa8b,color:#000
    classDef tech fill:#4d908e,color:#fff
    classDef color9 fill:#f3722c,color:#000
    classDef color10 fill:#577590,color:#000
    
    class Framework framework
    class Lang lang
    class Compiler compiler
    class Intermediate intermediate
    class Library lib
    class ProvingSystem provingSystem
    class AlgebraicForm algForm
    class Tech tech
```
---
Inspired by [https://harryr.github.io/zklangs/](https://harryr.github.io/zklangs/).
This diagram is using [Mermaid syntax](https://mermaid-js.github.io/mermaid/#/).
