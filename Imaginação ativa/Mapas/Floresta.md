
flowchart TD
    EN["Entrada da floresta"]

    subgraph FLO["Floresta antiga"]
        TRI["Trilha principal"]
        CLA["Clareira silenciosa"]
        ON["Onça mansa"]
        ARV["Árvores antigas"]
        PL["Placa dos colonizadores"]
    end

    subgraph CAB["Cabine verde-musgo"]
        POR["Porta da cabine"]
        CHU["Sala dos chuveiros"]
        DES["Desenhos apagados"]
        ANI["Figuras de animais"]
        PARE["Parede escondida"]
    end

    subgraph MIS["Encontros e mistérios"]
        HOM["Homem vestido de preto"]
        AV["Aviso: não acreditar nos rumores"]
        HIST["História dos colonizadores"]
        SEG["Significado dos desenhos"]
    end

    subgraph SAI["Passagens para outros territórios"]
        RAIZ["Passagem pelas raízes"]
        CAV["Caverna da cobrinha"]
        RES["Floresta do resort"]
        CID["Cidade Submersa"]
    end

    EN --> TRI
    TRI --> POR
    POR --> CHU
    CHU --> DES
    DES --> ANI
    TRI --> ON
    TRI --> HOM
    HOM --> AV
    TRI --> PL
    PL --> HIST

    TRI -.-> CLA
    CLA -.-> ARV
    DES -.-> PARE
    ANI -.-> SEG
    SEG <-.-> HIST

    ARV -.-> CAV
    ARV -.-> RES
    PARE -.-> RAIZ
    RAIZ -.-> CID

    classDef real fill:#315d46,color:#fff,stroke:#91c5a3
    classDef mystery fill:#584771,color:#fff,stroke:#b09bce
    classDef exit fill:#285d83,color:#fff,stroke:#8bb8d7

    class EN,TRI,ON,POR,CHU,DES,ANI,HOM,AV,PL,HIST real
    class CLA,ARV,PARE,SEG mystery
    class RAIZ,CAV,RES,CID exit
