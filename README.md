# A(n almost) complete atlas of Zero-Knowledge Proof technologies

Most of the blocks are clickable!

```mermaid
graph TD
    Rust ------ Bellman
    Rust ------ arkworks
    Rust ----- Halo2
    Halo2 --- UltraPLONK
    snarkjs --- PLONK
    arkworks --- Groth16
    Bellman --- PLONK
    R1CS ---- snarkjs
    R1CS --- PLONK
    R1CS --- Groth16
    Lurk ------- Groth16
    TypeScript --- SnarkyJS
    snarkjs --- Groth16
    R1CS ---- arkworks
    SnarkyJS ------ PLONK
    Circom ----- snarkjs 
    arkworks --- Marlin
    arkworks --- gm17
    arkworks --- gemini
    gm17 --- QAP
    gemini --- QAP
    Groth16 --- QAP
    Nova --- QAP
    Noir ---- ACIR
    Marlin --- QAP
    Lurk ------- SnarkPack[SnarkPack+]
    Lurk ------- Nova
    Leo ---- R1CS
    ZoKrates ---- R1CS
    Circom ---- R1CS
    SnarkPack --- QAP
    PLONK --- QAP
    UltraPLONK ---- zkSNARK
    ACIR ----- PLONK
    ACIR ----- Groth16
    ACIR ----- Marlin
    QAP --- zkSNARK
    Cairo ---- RAP
    RAP ------- zkSTARK
    
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
    class snarkjs,Bellman,Halo2,arkworks lib
    class Groth16,PLONK,Marlin,SnarkPack,Nova,UltraPLONK,gm17,gemini provingSystem
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
    click arkworks href "https://github.com/arkworks-rs/"
    click gm17 href "https://github.com/arkworks-rs/gm17"
    click gemini href "https://github.com/arkworks-rs/gemini"
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
