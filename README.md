# Files Manager

Files Manager is a comprehensive back-end project designed to simulate a real-world file storage and management platform. This project encapsulates essential back-end development skills, including user authentication, database operations with MongoDB, caching with Redis, and handling background tasks. It serves as a practical application of the back-end trimester knowledge acquired in the ALX Software Engineering program, focusing on JavaScript, Node.js, Express, MongoDB, and Redis.

## Project Overview

The objective of this project is to create a platform that allows users to upload and manage files. Key features include:

- **User Authentication:** Secure user authentication using tokens.
- **File Management:** Ability to list, upload, change permissions, and view files.
- **Image Processing:** Generate thumbnails for uploaded images to enhance performance and user experience.
- **Data Storage:** Utilize MongoDB for persistent storage of user and file information.
- **Caching:** Implement Redis for efficient data caching, enhancing the application's performance.
- **Background Processing:** Use background jobs for tasks such as thumbnail generation and welcome email sending, ensuring the application remains responsive.

## Technologies

- **Back-End:** JavaScript (ES6), Node.js, Express.js
- **Database:** MongoDB (NoSQL database for storing user and file data)
- **Cache:** Redis (For caching and temporary data storage)
- **Task Queue:** Bull (For managing background jobs)
- **Other Libraries:** Mocha (for testing), Nodemon, Image-thumbnail, Mime-Types

## Setup and Installation

1. **Prerequisites:**
    - Node.js (version 12.x.x)
    - MongoDB (Running on default port 27017 or set via environment variables)
    - Redis (Running on default port or set via environment variables)
    - Git

2. **Clone the repository:**
    ```sh
    git clone https://github.com/your-github-username/alx-files_manager.git
    cd alx-files_manager
    ```

3. **Install dependencies:**
    ```sh
    npm install
    ```

4. **Environment Variables:**
    Create a `.env` file in the root directory and set the following variables:
    - `PORT`: Port for the server (default: 5000)
    - `DB_HOST`: MongoDB host (default: localhost)
    - `DB_PORT`: MongoDB port (default: 27017)
    - `DB_DATABASE`: Database name (default: files_manager)
    - `FOLDER_PATH`: Path for storing uploaded files (default: /tmp/files_manager)

5. **Running the application:**
    - Start the server:
        ```sh
        npm start
        ```
    - Start the worker (in a separate terminal):
        ```sh
        npm run start-worker
        ```

## API Endpoints

- `GET /status`: Check the health of the application.
- `GET /stats`: Get statistics about users and files.
- `POST /users`: Create a new user.
- `GET /connect`: Authenticate a user.
- `GET /disconnect`: Log out a user.
- More endpoints for file management detailed in the API documentation.

## Project Structure

- `controllers/`: Contains controller files for handling API endpoint logic.
- `routes/`: Defines the API endpoints and associates them with their respective controllers.
- `utils/`: Utility classes for database and caching operations.
- `worker.js`: Background job processing.
- `server.js`: Entry point for the application.

## Learning Objectives

By the end of this project, I have solidified my knowledge in:

- Building APIs with Express.js
- User authentication mechanisms
- Data manipulation with MongoDB
- Implementing caching using Redis
- Background job processing
- Image processing for thumbnails

## License

This project is provided for educational purposes only. It is not affiliated with any actual file storage platform.

---

**Author:** [Joseph-Njoro](https://github.com/Joseph-Njoro)
