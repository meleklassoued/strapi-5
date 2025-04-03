# Strapi v5 Boilerplate Project

A modern, Docker-ready Strapi v5 boilerplate with PostgreSQL, optimized for scalable content management.

## 🚀 Features

- Strapi v5 with TypeScript
- Docker containerization
- PostgreSQL database integration
- RESTful API & GraphQL support
- Role-based access control (RBAC)
- Media library with multiple providers
- API documentation (OpenAPI/Swagger)
- Automated testing setup
- CI/CD pipeline configurations

## 🔮 Upcoming Features

- [ ] Code Quality & Formatting

  - ESLint configuration for consistent code style
  - Prettier setup for automatic code formatting
  - EditorConfig for cross-editor consistency

- [ ] Git Hooks & Conventional Commits

  - Husky for pre-commit and pre-push hooks
  - Commitlint for conventional commit messages
  - Lint-staged for running linters on staged files

- [ ] CI/CD Pipeline
  - GitHub Actions workflow for:
    - Automated testing
    - Code quality checks
    - Build verification
    - Docker image publishing
    - Automated deployments

## 🔧 Prerequisites

- Docker Desktop
- Node.js (>=18.x)
- npm (>=9.x) or yarn (>=1.22.x)

## 🛠 Quick Start

1. Clone and setup:

```bash
git clone <repository-url>
cd my-strapi-project
cp .env.example .env
```

2. Start with Docker:

```bash
make compose-dev
```

Access points:

- Admin Panel: http://localhost:1337/admin
- API Endpoint: http://localhost:1337/api

## 📦 Project Structure

```
.
├── config/                  # Strapi configurations
├── database/               # Database migrations & seeds
├── src/
│   ├── admin/             # Admin customizations
│   ├── api/               # Content-types & routes
│   ├── extensions/        # Strapi extensions
│   └── plugins/           # Custom plugins
├── public/                # Static files
├── tests/                 # Test suites
├── types/                 # TypeScript definitions
├── docker-compose.yml     # Docker compose config
└── Dockerfile            # Container definition
```

## 🔑 Environment Setup

Key variables in your `.env`:

```env
HOST=0.0.0.0
PORT=1337
APP_KEYS="your-keys-here"
API_TOKEN_SALT="your-salt"
ADMIN_JWT_SECRET="your-secret"
JWT_SECRET="your-jwt-secret"

# Database
DATABASE_CLIENT=postgres
DATABASE_HOST=postgres
DATABASE_PORT=5432
DATABASE_NAME=strapi
DATABASE_USERNAME=strapi
DATABASE_PASSWORD=strapi
```

## 🛠 Development

Start development server:

```bash
npm run develop
# or with yarn
yarn develop
```

Run tests:

```bash
npm run test
# or with yarn
yarn test
```

## 🚀 Deployment

1. Build for production:

```bash
npm run build
# or
yarn build
```

2. Start production server:

```bash
npm run start
# or
yarn start
```

## 🔒 Security Features

- JWT authentication
- API token strategy
- Rate limiting
- CORS configuration
- Security headers
- SQL injection prevention


## 🛟 Support & Resources

- [Strapi v5 Documentation](https://docs.strapi.io)
- [Strapi Community Discord](https://discord.strapi.io)
- [Strapi Blog](https://strapi.io/blog)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
