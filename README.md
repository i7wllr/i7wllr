# Online Chat Application

## Description
This is a simple online chat application built in Java that enables multiple users to communicate through a central server. The application utilizes socket programming to manage client-server communication and provides a basic text-based interface for user interaction.

## Features
- Multiple clients can connect to a central server.
- Users can send and receive messages in real-time.
- Simple text-based user interface for input and display.

## Requirements
- Java Development Kit (JDK) 8 or higher.
- An IDE (e.g., Eclipse, IntelliJ IDEA) or a text editor.

## How to Run the Application

### 1. Clone or Download the Project
Download the project files to your local machine or clone the repository from GitHub.

### 2. Open the Project in Your IDE
- Create a new Java project in your IDE.
- Add the `ChatServer.java` and `ChatClient.java` files to the project.

### 3. Run the Server
1. Locate the `ChatServer.java` file.
2. Right-click on `ChatServer.java` and select **Run As > Java Application**.
3. The server will start and listen for incoming client connections.

### 4. Run the Client
1. Open a new instance of your IDE or a new terminal window.
2. Locate the `ChatClient.java` file.
3. Right-click on `ChatClient.java` and select **Run As > Java Application**.
4. Repeat this step in multiple windows to simulate multiple clients.

### 5. Using the Chat Application
- Once the server is running, you can start typing messages in the client console.
- Messages sent from one client will be broadcast to all connected clients.

## Implementation Details

### Server (`ChatServer.java`)
- The server listens on a specified port (default: 12367).
- Each connected client is handled in a separate thread using the `ClientHandler` class.
- The server maintains a set of `PrintWriter` objects for all connected clients to facilitate message broadcasting.

### Client (`ChatClient.java`)
- The client connects to the server using the localhost address.
- The user can send messages through the console, which are sent to the server.
- Incoming messages from the server are handled in a separate thread, allowing for simultaneous sending and receiving of messages.

## Screenshot
![Chat Application Screenshot](path_to_your_screenshot.png)

## License
This project is open-source and available for use and modification.

## Contact
For any questions or suggestions, feel free to reach out to [Your Name] at [your.email@example.com].
