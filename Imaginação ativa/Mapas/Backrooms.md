
flowchart TD
    ENT["Entrada desconhecida"]

    subgraph ED["Prédio impossível"]
        SAG["Saguão"]
        ESC["Escadarias"]
        ELE["Elevador-gaiola"]
        AND["Andares superiores"]
        VAZ["Vão entre andares"]
    end

    subgraph BACK["Backrooms"]
        COR["Corredores repetidos"]
        SAL["Salas vazias"]
        CRUZ["Cruzamento de corredores"]
        DESC["Escadaria descendente"]
        INF["Níveis inferiores infinitos"]
    end

    subgraph EVENT["Acontecimentos e perigos"]
        CAP["Capacidade limitada do elevador"]
        PER["Perder-se ao tentar subir"]
        QUEDA["Queda de grande altura"]
        SOB["Sobrevivente da queda"]
        OBS["Sensação de observação"]
    end

    subgraph EXIT["Saídas possíveis"]
        SHOP["Shopping gigante"]
        TOR["Torre da Cidade Submersa"]
        RES["Resort entre dimensões"]
        RUA["Ruas de São Paulo"]
    end

    ENT --> SAG
    SAG --> ELE
    ELE --> CAP
    CAP --> ESC
    ESC --> PER
    PER --> COR

    SAG --> QUEDA
    QUEDA --> SOB

    COR --> SAL
    COR --> CRUZ
    COR --> DESC
    DESC --> INF

    ESC -.-> AND
    AND -.-> VAZ
    CRUZ -.-> OBS

    SAL -.-> SHOP
    INF -.-> TOR
    CRUZ -.-> RES
    SAG -.-> RUA

    classDef real fill:#55446e,color:#fff,stroke:#ac96cb
    classDef mystery fill:#355e79,color:#fff,stroke:#8fb6d1
    classDef danger fill:#78454b,color:#fff,stroke:#d1979b

    class ENT,SAG,ESC,ELE,CAP,PER,COR,DESC,INF,QUEDA,SOB real
    class SAL,CRUZ,AND,VAZ,OBS,SHOP,TOR,RES,RUA mystery
