flowchart TB
    L["Lucas"]
    G["Gabi"]
    P["Pedro"]

    subgraph C["01 · Mundo cotidiano"]
        R["Ruas de São Paulo"]
        USP["USP e faculdade"]
        FF["Fast-food"]
        SHOP["Shopping gigante"]
        BTG["BTG e escritórios"]
        AP["Apartamento elevado"]
    end

    subgraph A["02 · Arquitetura impossível"]
        E["Elevadores e escadas"]
        PR["Prédio gigantesco"]
        BACK["Backrooms"]
        COR["Corredores infinitos"]
    end

    subgraph N["03 · Natureza e profundezas"]
        FLO["Floresta"]
        CAB["Cabine verde-musgo"]
        ON["Onça mansa"]
        CAV["Caverna"]
        COB["Cobrinha"]
        SUB["Cidade submersa"]
    end

    subgraph M["04 · Outros territórios"]
        RES["Resort e piscinas"]
        CAT["Catedral"]
        CAST["Castelo"]
        OBS["Observador misterioso"]
        POR["Portais"]
        CEM["Cemitério"]
        PON["Ponte de madeira"]
    end

    L --> R
    G --> R
    L --> BTG
    L --> SUB
    P --> SUB
    L --> RES
    G --> RES

    R --- USP
    R --- FF
    R --- SHOP
    R --- BTG
    R --- AP

    PR --- E
    E --- BACK
    BACK --- COR

    FLO --- CAB
    CAB --- ON
    FLO --- CAV
    CAV --- COB

    CEM --- PON

    SHOP -.-> BACK
    AP -.-> PR
    BTG -.-> E
    COR -.-> POR
    POR -.-> FLO
    POR -.-> SUB
    RES -.-> SUB
    CAST -.-> OBS
    OBS -.-> BACK

    SHOP <--> PR
    CAB <--> CAV
    SUB <--> BACK
    CAT <--> OBS

    classDef person fill:#245c91,color:#fff,stroke:#82b8e5
    classDef everyday fill:#355c76,color:#fff,stroke:#83abc2
    classDef liminal fill:#57446f,color:#fff,stroke:#ad91d0
    classDef nature fill:#315e47,color:#fff,stroke:#8fbea1
    classDef mystery fill:#713e4e,color:#fff,stroke:#d18da3

    class L,G,P person
    class R,USP,FF,SHOP,BTG,AP everyday
    class E,PR,BACK,COR liminal
    class FLO,CAB,ON,CAV,COB,SUB nature
    class RES,CAT,CAST,OBS,POR,CEM,PON mystery