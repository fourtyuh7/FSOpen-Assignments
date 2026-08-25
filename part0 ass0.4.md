  ---
config:
  layout: fixed
---
flowchart LR
    A["Browser requests GET to example app/new note"] --> B["Server receives request"]
    B --> C["Sends back to Browser"]
    D["Browser requests GET to HTML, example app/notes"] --> B
    E["Browser requests GET to CSS, example app/main.css"] L_E_B_0@--> B
    F["Browser requests GET to Javascript & its JSON data"] --> B
    n1["1st"]
    n2["2nd"]
    n3["3rd"]

    n1@{ shape: text}
    n2@{ shape: text}
    n3@{ shape: text}
     A:::browser
     B:::server
     C:::response
     C:::response
     D:::browser
     E:::browser
     F:::browser
    classDef browser fill:#f0f9ff,stroke:#38bdf8
    classDef server fill:#f0fdf4,stroke:#4ade80
    classDef response fill:#fef2f2,stroke:#f87171
    style n1 color:#000000
    style n2 color:#000000
    style n3 color:#000000

    L_E_B_0@{ curve: linear }
