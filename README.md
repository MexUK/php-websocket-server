# php-websocket-server
A WebSocket Server written in PHP.

This project is very old (2011), and may not work with the latest WebSocket protocol.

This purpose of this project, was to demonstrate an implementation for the server-side aspect of the WebSocket networking protocol, in PHP.

The PHP for this project is written in functional-style coding not OOP-style coding.

An example chatbox application was also provided.

Security was considered for some parts of the server, especially data handling from clients. Such as:

- Ensuring that incoming data which is marked as a control frame is also marked as the final frame in the message.
- Rejecting incoming data to the server which is marked as not having mask data set.

Other idea(s) that were implemented:

- Reset incoming data buffers for client if the server received a frame which is not a continuation frame.

