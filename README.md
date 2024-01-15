About Client -Server Chat application
Chat System Overview:
This is a simple chat system with a server and multiple clients. The server manages connections and relays messages between clients.

Server Code (server.py):
Start the Server:

Run the server.py file. It will start listening for incoming connections on a specific IP address (192.168.100.12) and port (1234).
Client Connections:

Clients connect to the server by running the client.py file and providing a unique username.
Client Code (client.py):
Enter Username:

When you run the client, it prompts you to enter a username.
Click the "Join" button after entering a username.
Chat Interface:

You'll see a chat window with a text entry box to type your messages and a "Send" button to send messages.
Send Messages:

Type a message in the text entry box and click "Send."
Your message will be sent to the server, which then broadcasts it to all connected clients.
Receive Messages:

You'll also see messages from other clients in the chat window.
Leave the Chat:

Close the client window to leave the chat. The server will be notified, and your username will be removed from the active clients.
Breakdown of the Code:
Server (server.py):
Initialization:
Creates a server socket and binds it to a specific IP address and port.
Listening for Clients:
Listens for incoming connections in an infinite loop.
Spawns a new thread for each connected client to handle messages.
Client (client.py):
User Interface:
Provides a simple GUI with entry boxes for username and messages.
Connecting to Server:
Connects to the server using the specified IP and port.
Sends the chosen username to the server.
Listening for Messages:
Runs a separate thread to continuously listen for messages from the server.
Sending Messages:
Sends messages typed by the user to the server.
Instructions for Running:
Server:

Run server.py to start the server.
Clients:

Run client.py for each client you want to connect.
Enter a unique username and click "Join."
Chatting:

Type messages in the client's text entry box and click "Send."
Messages will be displayed in the chat window for all connected clients.
Exiting:

Close the client window to leave the chat.
Final Notes:
Error Handling:

Some basic error handling is included for network operations.
Any issues connecting or receiving messages will be shown in the console.
