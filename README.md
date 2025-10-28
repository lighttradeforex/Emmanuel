flowchart TD

    A[GitHub Desktop 🖥️] -->|Version Control| B[Firebase Studio 🎨]
    B -->|Frontend HTML & CSS Mastery| C[Markup Language 🧾]
    C -->|Documentation & Flowcharts| D[Database Management 💾]
    D -->|Data Storage & SQL Queries| E[AI Tools 🤖]

    subgraph "GitHub Workflow Overview"
        A:::github
        B:::frontend
        C:::markup
        D:::database
        E:::backend
    end

    E -->|Automation & Scripting| A

    %% Styling
    classDef github fill:#0366d6,stroke:#fff,stroke-width:2px,color:#fff;
    classDef frontend fill:#ff9f43,stroke:#fff,stroke-width:2px,color:#fff;
    classDef markup fill:#00b894,stroke:#fff,stroke-width:2px,color:#fff;
    classDef database fill:#0984e3,stroke:#fff,stroke-width:2px,color:#fff;
    classDef backend fill:#6c5ce7,stroke:#fff,stroke-width:2px,color:#fff;
