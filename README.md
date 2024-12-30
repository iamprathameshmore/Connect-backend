# Connect Backend

This repository contains the backend implementation for the Connect chat application. Built using Node.js and Express, it provides secure, real-time communication features, including WebSocket-based chat and user authentication.

## Features

- **Real-Time Chat:** Supports WebSocket-based communication for real-time messaging.
- **User Authentication:** Secure user login and registration using JWT.
- **Database Integration:** MongoDB for efficient and scalable data storage.
- **RESTful APIs:** Provides APIs for user and chat management.
- **Scalable Architecture:** Designed to handle multiple concurrent users.

## Requirements

- Node.js 14.0 or later
- MongoDB 4.0 or later
- npm 6.0 or later

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/connect-backend.git
   ```

2. Navigate to the project directory:
   ```bash
   cd connect-backend
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add the following variables:
     ```env
     PORT=5000
     MONGO_URI=your-mongodb-connection-string
     JWT_SECRET=your-jwt-secret
     ```

5. Start the development server:
   ```bash
   npm run dev
   ```

6. The server will run at `http://localhost:5000`.

## API Endpoints

### Authentication
- `POST /api/auth/register`: Register a new user.
- `POST /api/auth/login`: Login an existing user.

### Chat
- `GET /api/chat`: Fetch all chat messages.
- `POST /api/chat`: Send a new chat message.

### Users
- `GET /api/users`: Fetch all users.
- `GET /api/users/:id`: Fetch a user by ID.

## WebSocket Integration

- WebSocket connection is established at `/ws`.
- Supports sending and receiving chat messages in real-time.

## Development Scripts

- `npm run dev`: Starts the development server with hot-reloading.
- `npm run start`: Starts the production server.
- `npm run lint`: Runs linting checks.

## Contributing

Contributions are welcome! To contribute:

1. Fork this repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request detailing your changes.

## License

Connect Backend is released under the [MIT License](LICENSE).

## Acknowledgments

- Special thanks to the Node.js and MongoDB communities for their excellent tools and documentation.
- Thanks to all contributors who have helped improve this project.

---

For any issues or suggestions, feel free to open an issue in this repository. Your feedback is greatly appreciated!
