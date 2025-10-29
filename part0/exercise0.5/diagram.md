```mermaid
sequenceDiagram
    participant Browser
    participant Server

    Browser->>Server: Fetch HTML (https://studies.cs.helsinki.fi/exampleapp/spa)
    Server-->>Browser: Return HTML
    Browser->>Server: Fetch JavaScript (spa.js)
    Server-->>Browser: Return JavaScript
    Browser->>Server: Fetch JSON data (data.json)
    Server-->>Browser: Return JSON data
    Browser->>Browser: Render notes dynamically using JavaScript
```    