# ECDSA Node

This project is an assignment for Week 1 of the Ethereum Development Bootcamp at Alchemy University. The goal is to gain a deeper understanding of blockchain development by building a simple system that incorporates Public Key Cryptography to securely transfer funds between accounts.

## Project Overview

In this project, we have a simple React front-end that communicates with a centralized server. The server handles the transfer of balances between accounts. To ensure that only the rightful owner of an account can initiate transfers, we use Elliptic Curve Digital Signatures (ECDSA). This ensures that transfers are only authorized by users possessing the appropriate private key.

### Goal: Implement ECDSA

1. **Secure Transfers with Digital Signatures**:
   - Only the user with the corresponding private key can create a valid signature to move funds.
   - The server verifies the signature before transferring funds between accounts.

2. **Prevent Replay Attacks**:
   - Consider the security implications, such as the risk of a valid signature being intercepted and reused maliciously.

## Setup Instructions

### Video Instructions
For a comprehensive project overview and setup instructions, watch the following video:

[Project Overview and Instructions](https://www.loom.com/share/0d3c74890b8e44a5918c4cacb3f646c4)

### Written Instructions

To set up the project locally, follow these steps:

1. **Code Editor**:
   - Download and install a code editor (VSCode is recommended).

2. **Clone the Repository**:
   - Run the following command in your terminal to clone the repository:
     ```sh
     git clone https://github.com/alchemyplatform/ecdsa-node.git
     ```

3. **Run the Client and Server**:
   - Follow the instructions in the repository's README to run both the client and the server as separate processes.

### Client Setup

The client is a React app using Vite. To start the client:

1. Open a terminal in the `/client` folder.
2. Run `npm install` to install all dependencies.
3. Run `npm run dev` to start the application.
4. Access the app at [http://127.0.0.1:5173/](http://127.0.0.1:5173/).

### Server Setup

The server is a Node.js application using Express. To start the server:

1. Open a terminal in the `/server` folder.
2. Run `npm install` to install all dependencies.
3. Run `node index` to start the server.
4. The server should connect to the default port (3042) automatically.

   _Hint_: Use [nodemon](https://www.npmjs.com/package/nodemon) to automatically restart the server on changes:
   ```sh
   npm install -g nodemon
   nodemon index
