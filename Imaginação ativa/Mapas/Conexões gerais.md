
flowchart LR
    SP["01 · São Paulo"]
    SUB["02 · Cidade Submersa"]
    FLO["03 · Floresta Verde-Musgo"]
    BACK["04 · Backrooms"]
    RES["05 · Resort Entre Dimensões"]
    CEM["06 · Cemitério e Ponte"]
    CAT["07 · Catedral e Castelo"]
    CAV["08 · Caverna da Cobrinha"]
    UNI["09 · Cidade Universitária"]
    IDE["10 · Identidades e Transformações"]

    SP -->|"Enchente e fresta"| SUB
    SP -.->|"Passagem urbana"| UNI
    SP -.->|"Elevador ou corredor"| BACK
    SP -.->|"Mudança de cenário"| IDE
    SP -.->|"Shopping gigante"| RES

    SUB -.->|"Templo das raízes"| FLO
    SUB -.->|"Elevador submerso"| BACK
    SUB -.->|"Correnteza profunda"| CEM
    SUB -.->|"Lago subterrâneo"| CAV

    FLO <-.->|"Trilha e caverna"| CAV
    FLO <-.->|"Floresta do resort"| RES
    FLO -.->|"Símbolos e rumores"| CAT

    BACK <-.->|"Corredores dimensionais"| RES
    BACK <-.->|"Escadaria universitária"| UNI
    BACK <-.->|"Sala dos espelhos"| IDE
    BACK -.->|"Cripta"| CAT

    RES -.->|"Dimensão medieval"| CAT
    RES <-.->|"Mudança de identidade"| IDE
    RES -.->|"Travessia da ponte"| CEM

    CEM -.->|"Cerimônia simbólica"| CAT
    CEM <-.->|"Símbolo do touro"| IDE

    CAV <-.->|"Arquivo de investigação"| UNI
    UNI <-.->|"Ruas e faculdade"| SP
    UNI -.->|"Papéis sociais"| IDE

    classDef urban fill:#355e79,color:#fff,stroke:#91bad4,stroke-width:2px
    classDef water fill:#235e87,color:#fff,stroke:#85c5e7,stroke-width:2px
    classDef nature fill:#315f49,color:#fff,stroke:#98c9a9,stroke-width:2px
    classDef liminal fill:#5a4678,color:#fff,stroke:#b29bd2,stroke-width:2px
    classDef mystery fill:#764b58,color:#fff,stroke:#d2a0ad,stroke-width:2px

    class SP,UNI urban
    class SUB water
    class FLO,CAV nature
    class BACK,RES,IDE liminal
    class CEM,CAT mystery
