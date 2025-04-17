# Vite React Application

A modern React application built with Vite, TypeScript, and Docker for development and deployment.

## Technology Stack

- **Frontend Framework**: React with TypeScript
- **Build Tool**: Vite
- **Development Environment**: Docker
- **CI/CD**: GitHub Actions
- **Deployment**: GitHub Pages
- **Code Quality**: ESLint with TypeScript support

## Project Setup

### Prerequisites

- [Node.js](https://nodejs.org/) (v20 or later)
- [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/)
- [Git](https://git-scm.com/)

### Local Development

1. Clone the repository:
   ```bash
   git clone <your-repository-url>
   cd vite-react-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

### Docker Development

1. Build and start the development container:
   ```bash
   docker-compose up
   ```

2. Access the application at `http://localhost:5173`

The Docker setup includes:
- Hot reloading for development
- Volume mapping for real-time code updates
- Isolated development environment

## Building for Production

1. Build the application:
   ```bash
   npm run build
   ```

2. The built files will be in the `dist` directory

## Deployment

This application is automatically deployed to GitHub Pages using GitHub Actions. The deployment workflow:

1. Triggers on pushes to the main branch
2. Builds the application
3. Deploys to GitHub Pages

[![Deploy to GitHub Pages](https://github.com/scottc483/TEST-REPO/actions/workflows/deploy.yml/badge.svg)](https://github.com/scottc483/TEST-REPO/actions/workflows/deploy.yml)

### Manual Deployment

To manually trigger a deployment:
1. Go to the "Actions" tab in your GitHub repository
2. Select the "Deploy to GitHub Pages" workflow
3. Click "Run workflow"

## Project Structure

```
vite-react-app/
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions workflow
├── src/                    # Source code
├── public/                 # Static assets
├── dist/                   # Build output
├── Dockerfile.dev          # Development Docker configuration
├── docker-compose.yml      # Docker Compose configuration
├── package.json            # Project dependencies and scripts
└── vite.config.ts          # Vite configuration
```

## Development Tools

- **ESLint**: Code linting with TypeScript support
- **TypeScript**: Type checking and enhanced development experience
- **Vite**: Fast development server and build tool
- **Docker**: Containerized development environment

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.


