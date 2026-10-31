
flowchart TD
    CAR["Carro com Lucas, Gabi e Pedro"]

    subgraph CEM["Cemitério noturno"]
        ENT["Entrada do cemitério"]
        PES["Pessoas caminhando em silêncio"]
        LAG["Laguinho"]
        COL["Colar perdido de Gabi"]
        SAN["Santinha encontrada"]
        EST["Estátuas assustadoras"]
    end

    subgraph PON["Travessia da ponte"]
        MAD["Ponte de madeira elevada"]
        MUL["Mulheres mais velhas"]
        LIM["Limite de peso"]
        ONI["História do ônibus que caiu"]
        OUT["Outro lado"]
    end

    subgraph CER["Cerimônia simbólica"]
        PLA["Plataforma circular de concreto"]
        TOU["Grande estátua de touro"]
        APRE["Apresentação misteriosa"]
    end

    subgraph EXIT["Conexões narrativas"]
        SUB["Lago da Cidade Submersa"]
        CAT["Catedral"]
        RES["Resort"]
    end

    CAR --> ENT
    ENT --> PES
    ENT --> LAG
    LAG --> COL
    LAG --> SAN
    LAG --> EST
    ENT --> MAD
    MAD --> MUL
    MUL --> LIM
    MUL --> ONI
    MAD --> OUT
    OUT --> PLA
    PLA --> TOU
    PLA --> APRE

    LAG -.-> SUB
    APRE -.-> CAT
    OUT -.-> RES

    classDef real fill:#59476c,color:#fff,stroke:#b39bc9
    classDef passage fill:#315d79,color:#fff,stroke:#8db8d3
    classDef mystery fill:#714b52,color:#fff,stroke:#ca9ba2

    class CAR,ENT,PES,LAG,COL,SAN,EST,MAD,MUL,LIM,ONI,OUT,PLA,TOU,APRE real
    class SUB,CAT,RES passage
