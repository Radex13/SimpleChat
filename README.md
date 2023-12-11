# SimpleChat

Simple Real-Time Chat is a minimalistic chat application built with Node.js and Turso, providing real-time communication and storing messages in a Turso database.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Environment Variables](#environment-variables)
- [Contact](#contact)

## Installation

To set up the Simple Real-Time Chat locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/Radex13/SimpleChat.git

2. Navigate to the project directory:
   ```bash
   cd simple-real-time-chat

3. Install dependencies:
   ```bash
   npm install

4. Create a .env file in the project root and add the following environment variables:
   ```bash
   DB_TOKEN=your-turso-token
   DB_URL="libsql://your-turso-database-url"

5.  Run the application:
    ```bash
    npm start

6. Access the chat application in your browser at http://localhost:3000.

## Usage
Simple Real-Time Chat allows users to:
* Join chat room.
* Send and receive real-time messages.

## Environment Variables
The application uses the following environment variables, specified in the .env file:
  ```bash
  DB_TOKEN: "Your Turso database token"
  DB_URL: "Your Turso database URL"
```
## Contact
For any inquiries or feedback, please contact us at [your-email@example.com].
