## Hospital Management System - Capgemini Sprint Evaluation Project

## Project Structure

```text
hms-microservices/
│
├── README.md               # Project overview and documentation
├── .gitignore              # Git ignore rules for IDEs and build files
├── docker-compose.yml      # Orchestration for all services and databases
├── docs/                   # Technical documentation and guides
│   ├── architecture.md     # System architecture overview
│   ├── api-reference.md    # API endpoints and payload formats
│   ├── er-diagram.md       # Database entity relationship diagrams
│   └── setup-guide.md      # Step-by-step local development setup
│
├── config-server/          # Spring Cloud Config Server for centralized configuration
├── eureka-server/          # Netflix Eureka for service registration and discovery
├── api-gateway/            # Spring Cloud Gateway for routing and security
│
├── services/               # Core business logic microservices
│   └── README.md           # Placeholder for service-specific documentation
│
├── scripts/                # Utility scripts for development and deployment
│   ├── start-all.sh        # Script to launch all services locally
│   ├── stop-all.sh         # Script to gracefully stop all services
│   └── db-init.sql         # SQL script for database initialization
│
└── postman/                # API testing collections
    └── hms-collection.json # Postman collection for the HMS API
```

## Folder Explanations

- **`config-server/`**: Manages externalized configuration across all microservices.
- **`eureka-server/`**: Allows services to find and communicate with each other without hard-coding hostnames.
- **`api-gateway/`**: The unified entry point for all client requests, providing load balancing and authentication.
- **`services/`**: This folder will contain the functional microservices (e.g., Auth, User, Patient, Appointment).
- **`docs/`**: Central hub for developers to understand the design and maintenance of the system.
- **`scripts/`**: Automation tools to simplify common tasks like starting the entire infrastructure.
