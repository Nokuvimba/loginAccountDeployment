# Login Account Deployment

Microservices architecture for banking application with Login and Account services.

## Services

- **Login Service** (port 8001): User management and authentication
- **Account Service** (port 8002): Account management and transactions

## Quick Start

```bash
# Run both services
cd microservice-orchestration
docker-compose up --build

# Test communication
cd Account-Microservice
python test_communication.py
```

## Architecture

```
microservice-orchestration/
├── CI-CD_Y4-BankingApp_Login/    # Login microservice
├── Account-Microservice/         # Account microservice
└── docker-compose.yml           # Orchestration
```

## Service Communication

Account service validates users by calling Login service endpoints. Both services use PostgreSQL databases and communicate via HTTP APIs.

See individual service READMEs for detailed documentation.