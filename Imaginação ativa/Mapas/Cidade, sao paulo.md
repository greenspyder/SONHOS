
flowchart TD
    RUA["Ruas de São Paulo"]

    subgraph URB["Cidade cotidiana"]
        CASA["Casa"]
        BTG["Escritórios e trabalho"]
        USP["USP e faculdade"]
        FF["Fast-food"]
        SHOP["Shopping gigante"]
        AP["Apartamento elevado"]
    end

    subgraph TRANS["Rupturas possíveis"]
        ALAR["Alarme de incêndio"]
        ENCH["Enchente"]
        ELE["Elevador estranho"]
        COR["Corredor desconhecido"]
        ESC["Escadaria sem fim"]
    end

    subgraph DEST["Destinos"]
        SUB["Cidade Submersa"]
        BACK["Backrooms"]
        RES["Resort"]
        FLO["Floresta Verde-Musgo"]
    end

    RUA --> CASA
    RUA --- BTG
    RUA --- USP
    RUA --- FF
    RUA --- SHOP
    RUA --- AP

    BTG --> ALAR
    CASA --> ENCH
    ENCH --> SUB

    AP -.-> ELE
    ELE -.-> BACK
    SHOP -.-> COR
    COR -.-> RES
    USP -.-> ESC
    ESC -.-> BACK
    RUA -.-> FLO

    classDef city fill:#345b75,color:#fff,stroke:#8eb3ce
    classDef rupture fill:#704a56,color:#fff,stroke:#cb9ca7
    classDef dest fill:#315d49,color:#fff,stroke:#8fbea0

    class RUA,CASA,BTG,USP,FF,SHOP,AP city
    class ALAR,ENCH,ELE,COR,ESC rupture
    class SUB,BACK,RES,FLO dest
