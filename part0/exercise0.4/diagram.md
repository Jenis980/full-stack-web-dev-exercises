flowchart LR
    subgraph Browser
        A[User enters GET https://studies.cs.helsinki.fi/exampleapp/]
        B[Browser requests HTML document]
        C[Browser requests GET https://studies.cs.helsinki.fi/exampleapp/kuva.png]
        D[Browser renders the page with the image]
    end

    subgraph Server
        H[Server sends HTML document]
        I[Server sends kuva.png file]
    end

    A --> B
    B --> H
    H --> C
    C --> I
    I --> D
