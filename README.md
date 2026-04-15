# Project Title

## Prerequisites
- Node.js (v14 or higher)
- Docker (v20 or higher)
- MongoDB (local or cloud)

## Local Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/terrionagardner-gif/MCT.git
   ```
2. Navigate to the project directory:
   ```bash
   cd MCT
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Create a `.env` file based on `.env.example` and configure your environment variables.
5. Run the application:
   ```bash
   npm start
   ```

## Docker Setup
1. Build the Docker image:
   ```bash
   docker build -t mct-app .
   ```
2. Run the Docker container:
   ```bash
   docker run -p 3000:3000 mct-app
   ```
3. Access the application at `http://localhost:3000`.

## API Documentation
The API is built with Express. You can find the documentation in the `/docs` directory or view it online (if applicable).

## Testing
1. Run tests with:
   ```bash
   npm test
   ```

## WebSocket Examples
Here are some examples of WebSocket usage:
- **Connecting to WebSocket Server:**
   ```javascript
   const socket = new WebSocket('ws://localhost:3000');
   socket.onopen = () => {
       console.log('Connected to WebSocket server');
   };
   ```

## Example API Calls
- **Get User:**
   ```bash
   curl -X GET http://localhost:3000/api/user
   ```
- **Create User:**
   ```bash
   curl -X POST http://localhost:3000/api/user -d '{"name": "John Doe"}' -H 'Content-Type: application/json'
   ```
