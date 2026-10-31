flowchart TD
    subgraph S["01 · Superfície"]
        CASA["Frente de casa"]
        FEST["Festival"]
        ENCH["Grande enchente"]
        PED["Pedras que se abrem"]
    end

    subgraph E["02 · Entrada submersa"]
        FEN["Fresta no chão"]
        MER["Canal de mergulho"]
        AR["Bolsão de ar"]
        PORT["Portal de pedra"]
    end

    subgraph C["03 · Cidade antiga"]
        RUAS["Ruas inundadas"]
        PRACA["Praça central"]
        CASAS["Casas abandonadas"]
        TEMP["Templo submerso"]
        TORRE["Torre do relógio"]
        BIB["Biblioteca inundada"]
    end

    subgraph P["04 · Profundezas"]
        TUN["Túneis inferiores"]
        POCO["Poço profundo"]
        CAM["Câmara lacrada"]
        ORIG["Origem da inundação"]
    end

    subgraph M["05 · Mistérios"]
        PEG["Rastros de Pedro"]
        SOM["Sons através da água"]
        OBS["Presença desconhecida"]
        MEC["Mecanismo antigo"]
    end

    CASA --> FEST
    CASA --> ENCH
    ENCH --> PED
    PED -->|"Pedro cai"| FEN
    FEN -->|"Lucas mergulha"| MER
    MER --> RUAS

    MER -.-> AR
    MER -.-> PORT
    PORT -.-> RUAS

    RUAS <-.-> PRACA
    RUAS <-.-> CASAS
    PRACA <-.-> TEMP
    PRACA <-.-> TORRE
    CASAS <-.-> BIB
    TEMP <-.-> TUN
    TUN <-.-> POCO
    POCO -.-> CAM
    CAM -.-> ORIG

    RUAS -.-> PEG
    TORRE -.-> SOM
    BIB -.-> MEC
    POCO -.-> OBS
    PEG -.-> TUN
    MEC -.-> CAM

    classDef real fill:#24628a,color:#fff,stroke:#82bde0
    classDef invented fill:#514775,color:#fff,stroke:#a79bcb
    classDef danger fill:#78434b,color:#fff,stroke:#c98c94

    class CASA,FEST,ENCH,PED,FEN,MER,RUAS real
    class AR,PORT,PRACA,CASAS,TEMP,TORRE,BIB,TUN,CAM,ORIG,PEG,SOM,MEC invented
    class POCO,OBS danger