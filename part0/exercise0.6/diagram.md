```mermaid
sequenceDiagram
    participant Browser
    participant Server

    Browser->>Server: User types note and clicks Save
    Browser->>Server: HTTP POST to /new_note_spa with JSON data
    Server-->>Browser: HTTP 201 Created
    Browser->>Browser: Update UI with new note
```    