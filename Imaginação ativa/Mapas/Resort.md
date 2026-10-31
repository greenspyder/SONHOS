
flowchart TD
    SHOP["Shopping gigante"]

    subgraph RES["Complexo do resort"]
        ENT["Entrada do resort"]
        CIN["Sala de cinema cult"]
        REST["Restaurante"]
        PISC["Piscina"]
        QUA["Alojamentos"]
        FLO["Floresta ao redor"]
    end

    subgraph PESS["Personagens"]
        VIC["Victor e Leozinho"]
        GOR["Amigo da Gabi"]
        LIMA["Lucas Lima"]
        CAB["Rapaz de cabelo comprido"]
    end

    subgraph ESTR["Fenômenos estranhos"]
        POL["Forma de polvo na árvore"]
        MON["Criatura observadora"]
        SOB["Desafio de sobrevivência"]
        DES["Desapego como possível saída"]
        TRO["Mudança de dimensão"]
    end

    subgraph DIM["Dimensões"]
        MED["Mundo medieval"]
        ASS["Mundo assustador"]
        BACK["Backrooms"]
        CAST["Castelo e Catedral"]
    end

    SHOP --> ENT
    ENT --> CIN
    ENT --> REST
    ENT --> PISC
    ENT --> FLO

    REST --> GOR
    REST --> LIMA
    FLO --> POL
    POL --> MON
    PISC --> CAB
    CAB --> DES
    ENT --> SOB
    SOB --> TRO
    TRO --> MED
    TRO --> ASS

    CIN -.-> VIC
    ENT -.-> QUA
    DES <-.-> SOB
    ASS -.-> BACK
    MED -.-> CAST

    classDef real fill:#315d79,color:#fff,stroke:#91bbd4
    classDef mystery fill:#604774,color:#fff,stroke:#b69bcb
    classDef person fill:#35634f,color:#fff,stroke:#9bc7a9

    class SHOP,ENT,CIN,REST,PISC,FLO,GOR,LIMA,POL,MON,CAB,DES,SOB,TRO,MED,ASS real
    class QUA,BACK,CAST mystery
    class VIC person
