sequenceDiagram

    Note right of browser: El usuario escribe una nota y hace clic en "Save"

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 Created (sin redirección)
    deactivate server

    Note right of browser: El navegador actualiza la lista de notas dinámicamente sin recargar la página
