sequenceDiagram
    participant browser
    participant server
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa [{content: "New Note", date: "2023-05-11T09:32:00.186Z"}]
    activate server
    server-->>browser: application/json.
    deactivate server