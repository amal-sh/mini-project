```mermaid
sequenceDiagram
    participant User
    participant SPA
    participant Server

    User->>SPA: Write a new note in the text field
    User->>SPA: Click Save button
    SPA->>Server: Send the new note (text) to the server
    Server->>SPA: Save the note and respond with success
    SPA->>User: Display the new note in the list
