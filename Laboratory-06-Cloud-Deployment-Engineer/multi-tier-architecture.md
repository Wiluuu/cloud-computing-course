# Multi-Tier Architecture Overview

## The Web/Application Tier
The web/application tier serves as the front-facing layer of the architecture. Its primary role is to host the application code (Nextcloud), manage user sessions, render the graphical user interface in web browsers, and handle incoming HTTP requests from users.

## The Database Tier
The database tier acts as the backend data storage layer (MariaDB). Its role is to securely store persistent data, including user accounts, permissions, configuration settings, and metadata related to files uploaded to the private cloud storage system.

## Why Separate Them?
Separating the web server and the database into two distinct containers follows the crucial software design principle of "separation of concerns." If both components were packed into a single container, updating or scaling the web interface would risk disrupting database operations, and a failure in one service could crash the entire application stack. Isolation enhances security, maintainability, and scalability, allowing administrators to manage resources independently.
