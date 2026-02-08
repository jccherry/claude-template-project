# Backend

## Overview

<!-- Describe the backend: language, framework, architecture pattern (MVC, clean architecture, etc.). -->

## Project Structure

```
src/
├── routes/        # Route/controller definitions
├── services/      # Business logic
├── models/        # Data models / entities
├── middleware/     # Request middleware (auth, logging, etc.)
├── utils/         # Shared helpers
└── config/        # Configuration and env loading
```

## Key Dependencies

| Package | Purpose | Version |
|---------|---------|---------|
| <!-- e.g. Express --> | <!-- HTTP framework --> | <!-- ^4.x --> |

## API Design

<!-- REST, GraphQL, gRPC? Document the API style and any conventions (versioning, error format, pagination). -->

### Endpoints

<!-- List key endpoints or link to an OpenAPI spec. -->

| Method | Path | Description | Auth |
|--------|------|-------------|------|
| <!-- GET --> | <!-- /api/v1/users --> | <!-- List users --> | <!-- Yes --> |

## Authentication & Authorization

<!-- Describe the auth strategy: JWT, sessions, OAuth, API keys. -->
<!-- Document role-based access control if applicable. -->

## Error Handling

<!-- Describe the error handling pattern: error codes, response format, logging. -->

## Environment Variables

| Variable | Description | Required | Default |
|----------|-------------|----------|---------|
| <!-- DATABASE_URL --> | <!-- Postgres connection string --> | <!-- Yes --> | <!-- — --> |
| <!-- PORT --> | <!-- Server port --> | <!-- No --> | <!-- 3000 --> |

## Running Locally

```bash
# Install dependencies
# npm install

# Run dev server
# npm run dev

# Run in production mode
# npm start
```

## Notes

<!-- Rate limiting, caching strategy, external service integrations, known limitations. -->
