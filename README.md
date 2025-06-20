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
Client side:

![Image](https://github.com/user-attachments/assets/235d90f8-b3a6-407d-95d2-f7836c077b7d)


If someone from sever sends a message:

![Image](https://github.com/user-attachments/assets/06a8c353-b632-43a0-9dd8-44f584a2f864)



you will in this terminal:

![Image](https://github.com/user-attachments/assets/b24c1a17-be9e-41a0-9a26-3a5547120961)



now as a client:

![Image](https://github.com/user-attachments/assets/8f26ac7b-5827-407e-8651-11d5772b702b)



you will see:

![Image](https://github.com/user-attachments/assets/88313031-f359-44bc-92cc-bd849ef2b70d)



When you type Exit:
![Image](https://github.com/user-attachments/assets/d194d471-d8d9-41e8-a8c5-ad93b423923a)



the client will disconnect:

![Image](https://github.com/user-attachments/assets/23794f0c-af55-4c4d-91d4-e13c6f36249d)



if there is a connection problem, the client terminal will show like this:

![Image](https://github.com/user-attachments/assets/a28c113e-d375-4db1-b05e-62da2780c6dc)

