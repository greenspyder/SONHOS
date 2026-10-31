flowchart TB
    CID["Cidade Submersa"]

    CID --> RUAS["Ruas inundadas"]
    CID --> TEMP["Templo antigo"]
    CID --> TORRE["Torre submersa"]
    CID --> PROF["Profundezas"]

    RUAS --> FEN["Fresta original"]
    FEN -->|"Retorno pelo mergulho"| SUP["Superfície — São Paulo"]

    TEMP -.->|"Decifrar os desenhos de animais"| PAS["Passagem coberta de raízes"]
    PAS -.-> FLO["Floresta da Cabine Verde"]

    TORRE -.->|"Ativar mecanismo do elevador"| ELEV["Elevador impossível"]
    ELEV -.-> BACK["Backrooms"]

    PROF -.->|"Seguir correnteza subterrânea"| LAGO["Lago escuro"]
    LAGO -.-> CEM["Cemitério e Ponte de Madeira"]

    CID -.->|"Pedro ainda desaparecido"| BUSCA["Busca permanece ativa"]

    classDef city fill:#245e83,color:#fff,stroke:#85b9d9
    classDef destination fill:#315d47,color:#fff,stroke:#8fc4a0
    classDef mystery fill:#59466e,color:#fff,stroke:#b09bc9
    classDef risk fill:#7a454a,color:#fff,stroke:#d39ba0

    class CID,RUAS,TEMP,TORRE,PROF,FEN city
    class SUP,FLO,BACK,CEM destination
    class PAS,ELEV,LAGO mystery
    class BUSCA risk