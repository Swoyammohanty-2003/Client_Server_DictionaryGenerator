# Client-Server Dictionary Project

## 📌 Project Overview
This project implements a **Client-Server Dictionary System** in Java using **Socket Programming**.  
The client sends a keyword to the server, and the server responds with the corresponding definition if found in the dictionary.  
If the word is not found, the server notifies the client.

---

## 🛠️ Features
- Client-Server communication using **TCP Sockets**.
- Dictionary lookup functionality.
- Supports multiple keywords stored in a text file (`Dictionary.txt`).
- Handles unknown keywords gracefully.
- Simple and easy-to-use console-based interface.
- Admin client & server for managing dictionary entries.

---

## 📂 Project Structure
```
├── src/
│   ├── Client.java            # Client-side code
│   ├── Server.java            # Server-side code
│   ├── CrunchAdminClient.java # Extended Client (admin functionalities)
│   ├── CrunchAdminServer.java # Extended Server (admin functionalities)
│   ├── Dictionary.txt         # Dictionary file with word definitions
│
├── bin/                       # Compiled class files
├── Output Client Side.png     # Sample output screenshot
```

---

## ⚙️ Requirements
- **Java JDK 8+** (Recommended: JDK 19 as used in testing)
- Any IDE or terminal to run Java programs (e.g., VS Code, IntelliJ, Eclipse, or Command Prompt)

---

## ▶️ How to Run

### 1. Compile the Programs
```bash
javac Server.java Client.java CrunchAdminServer.java CrunchAdminClient.java
```

### 2. Run the Server
```bash
java Server
```

### 3. Run the Client
```bash
java Client
```

### 4. Enter a Keyword
- Example Input:  
  ```
  Enter the word to search: java
  ```
- Example Output:  
  ```
  Dictionary from Server:
  Java: Java is a general-purpose programming language that is class-based, object-oriented, and designed to have as few implementation dependencies as possible.
  ```

---

## 📖 Dictionary File
The `Dictionary.txt` file stores predefined keywords and their meanings.

Example entries:
```
Java: Java is a general-purpose programming language...
Python: Python is an interpreted high-level...
Network: A collection of devices connected together...
Artificial Intelligence: AI is the ability of a computer...
```



## 🔐 Admin Mode (CrunchAdminClient & CrunchAdminServer)
Alongside the basic client-server dictionary, an **admin mode** is implemented:  

- `CrunchAdminServer.java` → Extended server to handle admin requests.  
- `CrunchAdminClient.java` → Client tool for admins to:  
  - Add new dictionary entries  
  - Update existing definitions  
  - Remove dictionary entries  

This enables **dynamic dictionary management** without modifying `Dictionary.txt` manually.

---

## 🚀 Future Enhancements
- Add **multi-client support** using threads.
- Implement **add/remove dictionary entries** (admin features fully functional).
- Create a **GUI-based client**.
- Support for **database-backed dictionary** instead of a text file.

---

