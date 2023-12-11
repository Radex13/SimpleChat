# SimpleChat

Simple Real-Time Chat is a minimalistic chat application built with Node.js and Turso, providing real-time communication and storing messages in a Turso database.

## Table of Contents
- [Setting Up Turso with WSL](#setting-up-turso-with-wsl)
- [Installation](#installation)
- [Usage](#usage)
- [Important](#important)
- [Contact](#contact)

## Setting Up Turso with WSL

If you're using Windows and want to set up Turso, you'll need to use the Windows Subsystem for Linux (WSL). Follow these steps:

1. **Install WSL:**
   Follow the [WSL installation guide](https://docs.microsoft.com/en-us/windows/wsl/install) to install the Windows Subsystem for Linux on your machine.

2. **Install Turso with WSL:**
   Open your WSL terminal and install Turso using the following command:
   ```bash
   curl -sSfL https://get.tur.so/install.sh | bash
   ```
   Login with GitHub
   ```bash
   turso auth login
   ```
   Create the database on Turso Here create random name for the database
   ```bash
   turso db create
   ```
   Take your URL database start with "URL: libsql:" with this command copy for later
   ```bash
   turso db show name-yourdb
   ```
   And finish with the token for you database copy for later
   ```bash
   turso db tokens create name-yourdb
   ```   

## Installation

To set up the Simple Real-Time Chat locally, follow these steps:

1. Clone the repository in WSL:

   ```bash
   git clone https://github.com/Radex13/SimpleChat.git

2. Navigate to the project directory:
   ```bash
   cd simple-real-time-chat

3. Install dependencies:
   ```bash
   npm install

4. Create a .env file in the project root and add the following environment variables:
This URL and TOKEN were copied before.
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

## Usage
If you want delete the database this is the command
   ```bash
    turso db shell name-database
   ```
   ```bash
    DROP TABLE messages;
   ```

## Contact
For any inquiries or feedback, please contact us at ezequielvv103@gmail.com.
