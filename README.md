# Book Finder

A modern web application for discovering and exploring books using the Open Library API. Built with React, Material-UI, and Node.js.

![Book Finder Demo](https://via.placeholder.com/800x400.png?text=Book+Finder+Demo)

## Features

- 🔍 Search for books by title, author, or subject
- 📚 View detailed book information including descriptions and publication details
- 🌓 Light and dark theme support
- 📱 Fully responsive design that works on all devices
- ⚡ Fast and efficient search with instant results
- 🔄 Infinite scroll for browsing search results
- 📱 Mobile-friendly navigation with drawer menu

## Tech Stack

- **Frontend**: React 18, Material-UI 5, React Router 6
- **Backend**: Node.js, Express
- **API**: Open Library API
- **Build Tools**: Vite (or Create React App)

## Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher) or yarn

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/book-finder.git
cd book-finder
```

### 2. Install dependencies

For the root directory (if using workspaces):
```bash
npm install
```

For the server:
```bash
cd server
npm install
```

For the client:
```bash
cd ../client
npm install
```

### 3. Set up environment variables

1. Create a `.env` file in the root directory:
   ```env
   PORT=5000
   NODE_ENV=development
   CLIENT_URL=http://localhost:3000
   ```

2. Create a `.env` file in the client directory:
   ```env
   REACT_APP_API_URL=http://localhost:5000
   ```

### 4. Start the development servers

In the root directory, run:
```bash
# Start both client and server concurrently
npm run dev

# Or start them separately:
# Terminal 1 (server):
cd server && npm run dev

# Terminal 2 (client):
cd client && npm start
```

The application should now be running at:
- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## Available Scripts

### Client
- `npm start` - Start the development server
- `npm run build` - Build for production
- `npm test` - Run tests
- `npm run lint` - Lint the code
- `npm run format` - Format the code

### Server
- `npm start` - Start the production server
- `npm run dev` - Start the development server with nodemon
- `npm test` - Run tests

## Project Structure

```
book-finder/
├── client/                  # Frontend React application
│   ├── public/              # Static files
│   └── src/
│       ├── components/      # Reusable components
│       ├── pages/           # Page components
│       ├── services/        # API services
│       ├── App.js           # Main App component
│       └── index.js         # Entry point
│
├── server/                  # Backend Express server
│   ├── node_modules/
│   ├── server.js           # Main server file
│   └── package.json
│
├── .env.example            # Example environment variables
├── .gitignore
└── README.md
```

## Environment Variables

### Server
- `PORT` - Port to run the server on (default: 5000)
- `NODE_ENV` - Environment (development/production)
- `CLIENT_URL` - URL of the frontend for CORS

### Client
- `REACT_APP_API_URL` - URL of the backend API

## Contributing

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Make your changes and commit them: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Open Library](https://openlibrary.org/) for providing the book data
- Material-UI for the awesome UI components
- All the open-source libraries used in this project
