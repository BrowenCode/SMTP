# SMTP
A working, retro-style Simple Mail Transfer Protocol Client and Server that utilizes TCP sockets &amp; self-written string parsing. Written for a course on Networking Services and Protocols

Client.py is a SMTP Client program which takes two arguments: a domain name for a machine that hosts an SMTP server application, and a port number. The client takes a user-entered email, verifies the grammar of the user information as defined by RFC 821, and establishes a connection with the specified server via the specified port. Consequently, the client sends a sequence of valid SMTP messages to the server in order to transfer the email.

Server.py is a SMTP Server program which takes a single arguement: a port number. Once online, the server waits for connections from SMTP client programs on the specified port. It then receives and verifies the grammar of commands from those connections. Once a complete sequence of SMTP commands have been received the server stores the email file in the local directory.
