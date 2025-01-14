```mermaid
sequenceDiagram
    participant User
    participant Page
    participant Server

    User->>Page: Write something into the text field
    User->>Page: Click Save button
    Page->>Server: Send the new note (text) to the server
    Server->>Page: Save the note and respond with success
    Page->>User: Show the new note on the page
