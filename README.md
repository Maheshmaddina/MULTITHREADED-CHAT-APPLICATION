# INTERACTIVE-QUIZ-APPLICATION

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: MAHESH MADDINA

*INTERN ID*:CT06DF1416

*DOMAIN*: JAVA PROGRAMMING

*DURATION*: 6 WEEKS

*MENTOR*: NEELA SANTOSH

#DESCRIPTIONS

# Description of ChatClient and ChatServer Java Application
The ChatClient and ChatServer are simple Java programs built using sockets and multithreading to enable real-time communication between a client and a server. This basic chat application demonstrates how Java handles network connections and parallel communication streams.
SOURCE : VISUAL STUDIO CODE.

 # ChatServer.java
The ChatServer is responsible for listening for incoming client connections on a specified port (e.g., 1234). It uses a ServerSocket to accept connections and maintains a list of client sockets. For each client, it creates a new thread to handle communication.

When a client sends a message, the server reads the message using a BufferedReader and then broadcasts it to all other connected clients using a PrintWriter. This broadcast mechanism enables group chat functionality. Synchronization is used to safely handle concurrent access to the list of clients.

Key features:

Uses ServerSocket for connection handling.

Spawns a new thread for each client (ClientHandler).

Supports multiple clients using multithreading.

Broadcasts messages from one client to all others.

# ChatClient.java
The ChatClient connects to the server using a Socket. It starts two simultaneous operations:

A background thread listens for and displays messages received from the server.

The main thread reads user input and sends it to the server.

The client uses a BufferedReader to read input from the console and from the server. A PrintWriter sends messages to the server. If the user types "exit", the client terminates the connection.

Key features:

Connects to the server using Socket.

Reads user input and sends messages to the server.

A separate thread listens for incoming messages.

Graceful exit when the user types "exit".

# Communication Flow
The server runs and waits for clients.

Clients connect and send/receive messages.

The server relays each client’s message to all others.

Clients display messages in real time.

Typing "exit" closes the client connection.

# Technologies Used
Java Sockets (Socket, ServerSocket)

I/O Streams (BufferedReader, PrintWriter)

Multithreading (Thread, Runnable)

Basic Synchronization (synchronized block)

This project demonstrates the core concepts of client-server architecture and concurrent programming in Java. It forms the foundation for more advanced applications like group chat apps, messaging systems, or multiplayer games.



# OUTPUT
Client side 

If someone from sever sends a message

you will in this terminal

now as a client:

you will see:

When you type Exit:

the client will disconnect

if there is a connection problem, the client terminal will show like this:

