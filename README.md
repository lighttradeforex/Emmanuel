flowchart LR
    A[GitHub Desktop 🖥️ <br/> GIT Versioning <br/> <i>aka Google Docs History</i>] --> B[Firebase Studio 🔥 <br/> Frontend HTML & CSS Mastery <br/> <i>aka Paint + W3Schools</i>]
    B --> C[Markup Language 🧾 <br/> README + FlowCharts (Mermaid) <br/> <i>aka PowerPoint</i>]
    C --> D[Database Management 💾 <br/> Supabase SQL Tables <br/> <i>aka Excel</i>]
    D --> E[AI Tools 🤖 <br/> Gemini / Jules / Windsurf / CODEX <br/> <i>JavaScript Backend</i>]
    E --> A

    subgraph Legend
        L1[🖥️ GitHub = Version History like Google Docs]
        L2[🔥 Firebase = Design & Frontend like Paint]
        L3[🧾 Markup = Docs & Diagrams like PowerPoint]
        L4[💾 Supabase = Database like Excel]
        L5[🤖 AI Tools = Automate JS backend (replaces IT personnel)]
    end

    classDef dev fill:#0366d6,stroke:#fff,color:#fff;
    classDef ui fill:#ff9f43,stroke:#fff,color:#fff;
    classDef doc fill:#00b894,stroke:#fff,color:#fff;
    classDef db fill:#0984e3,stroke:#fff,color:#fff;
    classDef ai fill:#6c5ce7,stroke:#fff,color:#fff;

    class A dev;
    class B ui;
    class C doc;
    class D db;
    class E ai;
