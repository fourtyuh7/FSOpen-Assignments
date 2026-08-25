sequenceDiagram
    participant browser
    participant server

   ```mermaid
        Graph TB
        A[Browser requests GET to example app/new note] --> B[Server receives request]
        B --> C[Sends back to Browser]
        C --> D[Browser requests GET to HTML, example app/notes] --> B
        B --> C
        C --> E[Browser requests get to CSS, example app/main .cs] --> B
        B --> C

   ```
