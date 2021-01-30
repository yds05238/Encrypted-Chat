# Chat using Encryption

Chat program between a single client and a single server. Uses RSA Encryption to secure keys and AES Encryption to secure longer messages.

## Steps of Key Generation/Exchange

1. Client creates its public and private keys (RSA).

2. Client sends its public key with the initial message to Server.

3. Once Server gets the initial message, Server creates the AES symmetrical encryption key.

4. Server encrypts AES key with Client's public key.

5. Server sends the encrypted AES key with the acknowledge
   message to Client.

6. Once Client gets the acknowledge message, Client decrypts the AES key using its private key.

7. From now on, both Client and Server can use the AES key to encrypt and decrypt.

## Requirements

- gcc/g++
- C++

## Usage

1. Compile server.cpp using compile-server.sh
2. Start server (server 12345)
3. Compile client.cpp using compile-client.sh
4. Start client (client 127.0.0.1 12345)
5. Send chats (both directions)
