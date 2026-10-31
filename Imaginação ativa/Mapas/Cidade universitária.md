
flowchart TD
    RUA["Ruas de São Paulo"]

    subgraph EXT["01 · Cidade universitária"]
        USP["Campus da USP"]
        AV["Avenidas e caminhos"]
        PRAC["Praça universitária"]
        LAN["Lanchonete"]
        PORT["Portão da faculdade"]
    end

    subgraph FAC["02 · Faculdade gigantesca"]
        SAG["Saguão principal"]
        COR["Corredores extensos"]
        SAL["Salas de aula"]
        DIR["Faculdade de Direito"]
        BIB["Biblioteca"]
        ESC["Escadaria monumental"]
    end

    subgraph MIS["03 · Pessoas e mistérios"]
        GABI["Gabi"]
        AMI["Amiga de Gabi"]
        BOL["Bolsa perdida"]
        DOC["Documentos e instruções"]
        ARQ["Arquivo restrito"]
        OBS["Pessoa desconhecida"]
    end

    subgraph EXIT["04 · Saídas"]
        CAV["Caverna da Cobrinha"]
        BACK["Backrooms"]
        SHOP["Shopping Gigante"]
        RUA2["Retorno à cidade"]
    end

    RUA -.-> USP
    USP -.-> AV
    AV -.-> LAN
    AV -.-> PRAC
    PRAC -.-> PORT

    PORT -.-> SAG
    SAG -.-> COR
    COR -.-> SAL
    COR -.-> DIR
    COR -.-> BIB
    COR -.-> ESC

    GABI --> DIR
    GABI --> BOL
    BOL --> DOC
    AMI -.-> LAN
    BIB -.-> ARQ
    ARQ -.-> OBS

    ESC -.-> BACK
    ARQ -.-> CAV
    SAG -.-> SHOP
    PORT -.-> RUA2

    classDef urban fill:#355e79,color:#fff,stroke:#8fb8d2
    classDef mystery fill:#5c4771,color:#fff,stroke:#b59bcc
    classDef person fill:#315e49,color:#fff,stroke:#98c4a6

    class RUA,USP,AV,PRAC,LAN,PORT,SAG,COR,SAL,DIR,BIB,ESC urban
    class ARQ,OBS,CAV,BACK,SHOP,RUA2 mystery
    class GABI,AMI,BOL,DOC person
