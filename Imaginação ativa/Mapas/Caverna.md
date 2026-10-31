
flowchart TD
    ENT["Entrada da caverna"]

    subgraph CAV["01 · Caverna"]
        GAL["Galeria rochosa"]
        COB["Pequena cobrinha"]
        VIN["Cobrinha se prende a Lucas"]
        AJU["Cobrinha ajuda Lucas"]
        LAG["Lago subterrâneo"]
        FOS["Passagem estreita"]
    end

    subgraph COM["02 · Espaços cotidianos"]
        PAD["Padaria sofisticada"]
        DOC["Sobremesas"]
        GABI["Gabi"]
        BOL["Bolsa desaparecida"]
    end

    subgraph INV["03 · Investigação"]
        INS["Instruções sobre arma"]
        DET["Gabi como detetive/delegada"]
        PIS["Busca pela bolsa"]
        ARQ["Arquivo de pistas"]
        SEG["Responsável pelo desaparecimento"]
    end

    subgraph EXIT["04 · Conexões"]
        FLO["Floresta Verde-Musgo"]
        UNI["Cidade Universitária"]
        SUB["Cidade Submersa"]
    end

    ENT --> GAL
    GAL --> COB
    COB --> VIN
    VIN --> AJU

    PAD --> DOC
    PAD --> GABI
    GABI --> BOL
    BOL --> INS
    BOL --> PIS
    PIS --> DET

    GAL -.-> LAG
    GAL -.-> FOS
    PIS -.-> ARQ
    ARQ -.-> SEG

    ENT <-.-> FLO
    FOS -.-> UNI
    LAG -.-> SUB

    classDef real fill:#315e48,color:#fff,stroke:#9cc5a7
    classDef mystery fill:#584771,color:#fff,stroke:#b09bce
    classDef exit fill:#285e82,color:#fff,stroke:#91bdd8

    class ENT,GAL,COB,VIN,AJU,PAD,DOC,GABI,BOL,INS,PIS,DET real
    class LAG,FOS,ARQ,SEG mystery
    class FLO,UNI,SUB exit
