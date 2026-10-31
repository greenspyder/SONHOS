
flowchart TD
    ENT["Entrada do território"]

    subgraph CAT["Catedral"]
        PORT["Portões principais"]
        NAV["Nave central"]
        ALT["Altar"]
        VIT["Vitrais"]
        CRIP["Cripta"]
    end

    subgraph CAST["Castelo"]
        PAT["Pátio interno"]
        ESC["Escadaria de pedra"]
        TOR["Torre"]
        SAL["Grande salão"]
        MUR["Muralhas"]
    end

    subgraph FIG["Figuras e fenômenos"]
        DEM["Presenças demoníacas"]
        OBS["Figura observadora"]
        SOM["Vozes distantes"]
        SIM["Símbolos desconhecidos"]
    end

    subgraph EXIT["Saídas propostas"]
        MED["Dimensão medieval do resort"]
        BACK["Backrooms"]
        CEM["Cerimônia do touro"]
    end

    ENT --> PORT
    PORT --> NAV
    NAV --> ALT
    NAV -.-> VIT
    ALT -.-> CRIP
    CRIP -.-> SOM
    NAV --> DEM

    ENT -.-> PAT
    PAT -.-> ESC
    ESC -.-> TOR
    PAT -.-> SAL
    SAL -.-> SIM
    TOR -.-> OBS
    PAT -.-> MUR

    MUR -.-> MED
    CRIP -.-> BACK
    ALT -.-> CEM

    classDef core fill:#654553,color:#fff,stroke:#d19ca9
    classDef mystery fill:#594671,color:#fff,stroke:#b39acc
    classDef exit fill:#315c7d,color:#fff,stroke:#92b8d2

    class ENT,PORT,NAV,ALT,DEM core
    class VIT,CRIP,PAT,ESC,TOR,SAL,MUR,OBS,SOM,SIM mystery
    class MED,BACK,CEM exit
