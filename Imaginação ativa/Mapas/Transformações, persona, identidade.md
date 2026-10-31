
flowchart TD
    ENT["Entrada no território"]

    subgraph MET["01 · Estação e cidade"]
        CAR["Metrô Carrão"]
        PLAT["Plataforma"]
        TREM["Trem"]
        MULT["Multidão"]
        RUA["Rua desconhecida"]
    end

    subgraph TRA["02 · Transformações"]
        CAO["Cachorro"]
        HUM["Forma humana"]
        COR["Identidade corintiana"]
        ROU["Mudança de roupas"]
        ROST["Rosto no espelho"]
    end

    subgraph SOC["03 · Identidade social"]
        GRU["Pertencimento ao grupo"]
        JUL["Olhares e julgamentos"]
        PAP["Papéis sociais"]
        MASC["Imagem de masculinidade"]
        SOM["Sombra pessoal"]
    end

    subgraph NUC["04 · Núcleo mutável"]
        ESP["Sala dos espelhos"]
        DUP["Reflexos diferentes"]
        MEM["Memórias pessoais"]
        ESC["Escolha de identidade"]
    end

    subgraph EXIT["05 · Conexões"]
        BACK["Backrooms"]
        BTG["Escritórios"]
        RES["Resort Entre Dimensões"]
        CEM["Cerimônia do Touro"]
    end

    ENT --> CAR
    CAR --> PLAT
    PLAT --> TREM
    PLAT -.-> MULT
    PLAT -.-> RUA

    CAO --> HUM
    HUM --> COR
    HUM -.-> ROU
    ROU -.-> ROST

    COR -.-> GRU
    MULT -.-> JUL
    GRU <-.-> PAP
    PAP -.-> MASC
    JUL -.-> SOM

    ROST -.-> ESP
    ESP -.-> DUP
    DUP -.-> MEM
    MEM -.-> ESC

    ESP -.-> BACK
    PAP -.-> BTG
    ESC -.-> RES
    MASC -.-> CEM

    classDef real fill:#345f7b,color:#fff,stroke:#8ebad5
    classDef symbolic fill:#624875,color:#fff,stroke:#b69bcd
    classDef exit fill:#365e49,color:#fff,stroke:#94c2a5

    class CAR,CAO,HUM,COR real
    class PLAT,TREM,MULT,RUA,ROU,ROST,GRU,JUL,PAP,MASC,SOM,ESP,DUP,MEM,ESC symbolic
    class BACK,BTG,RES,CEM exit
