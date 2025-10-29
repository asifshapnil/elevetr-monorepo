# Elevetr Monorepo

This is a monorepo containing the Elevetr Job Assistant project with both backend and frontend applications.

## Structure

```
elevetr/
├── Job-Assistant/          # Backend API (NestJS)
├── job-assistant-fe/       # Frontend (React + Vite)
├── package.json            # Root package.json with workspace config
└── README.md              # This file
```

## Prerequisites

- Node.js >= 18.0.0
- npm >= 8.0.0

## Getting Started

### Install Dependencies

```bash
# Install all dependencies for both projects
npm run install:all

# Or install individually
npm run install:backend
npm run install:frontend
```

### Development

```bash
# Run both backend and frontend in development mode
npm run dev:all

# Or run individually
npm run dev:backend    # Backend on port 3000
npm run dev:frontend   # Frontend on port 3001
```

### Building

```bash
# Build both projects
npm run build:all

# Or build individually
npm run build:backend
npm run build:frontend
```

### Testing

```bash
# Run tests for both projects
npm run test:all

# Or test individually
npm run test:backend
npm run test:frontend
```

### Cleaning

```bash
# Clean all node_modules and build artifacts
npm run clean
```

## Individual Project Commands

### Backend (Job-Assistant)
```bash
cd Job-Assistant
npm run start:dev    # Development
npm run build        # Production build
npm run start:prod   # Production start
npm test            # Run tests
```

### Frontend (job-assistant-fe)
```bash
cd job-assistant-fe
npm run dev         # Development
npm run build       # Production build
npm run preview     # Preview production build
npm test           # Run tests
```

## Environment Variables

Each project has its own environment configuration:
- Backend: `Job-Assistant/.env`
- Frontend: `job-assistant-fe/.env`

## Deployment

Each project can be deployed independently or together using the monorepo structure.

## Contributing

1. Make changes in the respective project directory
2. Test your changes using the appropriate npm scripts
3. Commit changes to the monorepo
4. Push to the main repository
