# Secure Chat System

Secure Chat System is a Python-based chat application designed for secure communication over a network. It consists of both server and client components, allowing multiple users to connect, exchange encrypted messages, and maintain their online presence securely.

## Features

### Server

- **Multi-client Support**: The server can handle multiple client connections simultaneously.
- **User Authentication**: Users can register accounts or log in securely using usernames and passwords.
- **Message Encryption**: Messages exchanged between users are encrypted to ensure confidentiality.
- **Message Storage**: The server stores messages for offline users and delivers them upon login.
- **Online Status**: The server manages users' online status and prevents multiple logins with the same account.

### Client

- **User Authentication**: Clients can create accounts or log in securely using usernames and passwords.
- **Encrypted Communication**: Messages exchanged between clients are encrypted to ensure confidentiality.
- **Online Status**: Clients can check the online status of other users before sending messages.
- **Message Storage**: Clients can retrieve missed messages sent to them while they were offline.
- **Colorful Interface**: Both the server and client interfaces include colorful banners and text styling.


## Security Measures

### End-to-End Encryption
- **Encryption Algorithm**: AES (Advanced Encryption Standard) is utilized for encrypting messages exchanged between clients. Encryption and decryption are performed only at the server and receiver, ensuring end-to-end encryption.
- **Confidentiality**: Messages are encrypted before transmission and decrypted upon reception, preventing unauthorized access to message content.

### Password Storage
- **Hashing Algorithm**: SHA-256 (Secure Hash Algorithm 256-bit) is employed to securely store user passwords in the database.
- **Preventing Attacks**: Storing hashed passwords mitigates the risk of attacks, such as Man-in-the-Middle (MIM) attacks and unauthorized access to the database.


## Setup

1. Clone this repository.
2. Install the required dependencies listed in `requirements.txt` for both the server and client components.
3. Start the server by running `server.py`.
4. Run the client application `client.py` and follow the prompts to create an account or log in.

## Usage

### Server

1. Start the server by running `server.py`.
2. Clients can connect to the server using a TCP client, such as Telnet, or a custom client application.

### Client

1. Run the client application `client.py`.
2. Choose to create a new account or log in with existing credentials.
3. Use the available features to search for users, send encrypted messages, fetch missed messages, and logout.

## Dependencies

- `pymongo`: MongoDB driver for Python.
- `colorama`: Cross-platform library for colored terminal text.
- `pyfiglet`: Library for creating ASCII text banners.
- `pycryptodome`: Cryptographic library for encryption and decryption.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
