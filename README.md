# Telecom User Service

User management microservice for the Telecom platform.

## Architecture

- **Language:** Go 1.21
- **Framework:** Standard library (net/http)
- **Deployment:** Cloud Run
- **Container Registry:** Artifact Registry

## Endpoints

- `GET /health` - Health check
- `GET /api/v1/users` - List all users
- `GET /api/v1/users/profile` - Get user profile

## Development

Build locally:
```bash
go build -o user-service ./cmd/api
```

Run locally:
```bash
./user-service
```

Service runs on port 8080.

## Deployment

Automatic deployment on push to main branch via GitHub Actions CI/CD.

## CI/CD Pipeline

- Build Docker image
- Push to Artifact Registry
- Deploy to Cloud Run
