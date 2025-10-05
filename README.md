# Recruiter

A NestJS-based recruitment management system built with TypeScript, Prisma, and AdminJS.

⚠️ Currently in development.

---

## Description

This is a recruitment management application built with the [NestJS](https://github.com/nestjs/nest) framework. It provides a robust backend API with an admin interface for managing recruitment processes.

## Tech Stack

- **Framework**: NestJS with TypeScript
- **Database**: MySQL with Prisma ORM
- **Admin Interface**: AdminJS
- **Testing**: Jest
- **Linting**: ESLint with Prettier

## Prerequisites

Before running this application, make sure you have the following installed:

- Node.js (v18 or higher)
- MySQL database
- npm or yarn package manager

## Environment Setup

1. Create a `.env` file in the root directory with the following variables:

```env
DATABASE_URL="mysql://username:password@localhost:3306/recruiter_db"
```

2. Replace the connection string with your actual MySQL database credentials.

## Project setup

```bash
# Install dependencies
$ npm install
# or
$ yarn install

# Generate Prisma client
$ npx prisma generate

# Run database migrations (if any)
$ npx prisma migrate dev
```

## Compile and run the project

```bash
# development
$ npm run start
# or
$ yarn run start

# watch mode (recommended for development)
$ npm run start:dev
# or
$ yarn run start:dev

# production mode
$ npm run start:prod
# or
$ yarn run start:prod
```

The application will be available at:
- API: `http://localhost:3000`
- Admin Interface: `http://localhost:3000/admin`

### Admin Access

Default admin credentials:
- Email: `admin@example.com`
- Password: `password`

> **Note**: Change these default credentials in production!

## Run tests

```bash
# unit tests
$ npm run test
# or
$ yarn run test

# e2e tests
$ npm run test:e2e
# or
$ yarn run test:e2e

# test coverage
$ npm run test:cov
# or
$ yarn run test:cov

# test in watch mode
$ npm run test:watch
# or
$ yarn run test:watch
```

## Database Management

```bash
# View and edit data using Prisma Studio
$ npx prisma studio

# Reset database (development only)
$ npx prisma migrate reset

# Generate Prisma client after schema changes
$ npx prisma generate
```

## Development Commands

```bash
# Format code
$ npm run format
# or
$ yarn run format

# Lint code
$ npm run lint
# or
$ yarn run lint

# Build for production
$ npm run build
# or
$ yarn run build
```

## Project Structure

```
├── prisma/
│   └── schema.prisma          # Database schema
├── src/
│   ├── app.controller.ts      # Main application controller
│   ├── app.module.ts          # Root application module
│   ├── app.service.ts         # Main application service
│   ├── main.ts               # Application entry point
│   └── prisma/               # Prisma module and service
├── test/                     # E2E tests
├── package.json
└── README.md
```

## Features

- RESTful API built with NestJS
- Database management with Prisma ORM
- Admin interface with AdminJS
- TypeScript support
- Comprehensive testing setup
- Code formatting and linting
- Environment-based configuration

## API Documentation

Once the application is running, you can access:

- **API Endpoints**: `http://localhost:3000`
- **Admin Panel**: `http://localhost:3000/admin`

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is [UNLICENSED](LICENSE).
