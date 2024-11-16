# How the Handshake Works
## Initiation:
The Judge establishes a secure connection to the server using SSL.
## Request:

The Judge sends a handshake packet containing metadata (problems, runtimes, id, key) to identify itself and its capabilities.
## Response Handling:

The Judge waits for a response from the server. If the response contains `"name": "handshake-success"`, the handshake is considered successful.
Otherwise, it logs an error and may attempt to reconnect.
