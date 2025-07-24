[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=19976284&assignment_repo_type=AssignmentRepo)
# Testing and Debugging MERN Applications

This project demonstrates comprehensive testing strategies for a MERN stack application, including unit testing, integration testing, and end-to-end testing, along with debugging techniques.

## Project Overview

This is a monorepo MERN stack application using pnpm workspaces, configured with:
- Client-side React testing using Jest and React Testing Library
- Server-side API testing using Jest and Supertest
- End-to-end testing using Cypress
- In-memory MongoDB testing setup

## Project Structure

```
project/
├── client/                 # React front-end
│   ├── src/               
│   │   └── tests/         # Client-side tests
│   │       ├── setup.js   # Test setup configuration
│   │       └── unit/      # Unit tests for React components
│   └── package.json       # Client dependencies
├── server/                # Express.js back-end
│   ├── tests/            # Server-side tests
│   │   ├── setup.js      # Test setup configuration
│   │   └── integration/  # Integration tests for API endpoints
│   └── package.json      # Server dependencies
├── jest.config.js        # Jest configuration
├── package.json          # Root dependencies
└── pnpm-workspace.yaml   # Workspace configuration
```

## Tech Stack

- **Package Manager**: pnpm@10.5.1
- **Testing Frameworks**:
  - Jest v29.7.0 (Unit & Integration Testing)
  - React Testing Library v14.1.2 (React Component Testing)
  - Cypress v13.6.1 (End-to-End Testing)
  - Supertest v6.3.3 (API Testing)
- **Development Tools**:
  - MongoDB Memory Server v9.1.3 (Database Testing)

## Getting Started

1. **Prerequisites**
   - Node.js (v18 or higher)
   - pnpm (v10.5.1 or higher)
   - MongoDB (for local development)

2. **Installation**
   ```bash
   # Install dependencies for all workspaces
   pnpm install
   ```

3. **Running Tests**

   Client Tests:
   ```bash
   # In the client directory
   pnpm test              # Run all tests with coverage
   pnpm test:unit        # Run only unit tests
   pnpm test:e2e         # Run Cypress end-to-end tests
   ```

   Server Tests:
   ```bash
   # In the server directory
   pnpm test              # Run all tests with coverage
   pnpm test:unit        # Run only unit tests
   pnpm test:integration # Run only integration tests
   ```

## Test Coverage Requirements

The project aims for comprehensive test coverage:
- Unit Tests: Minimum 70% coverage
- Integration Tests: Key API endpoints and data flows
- End-to-End Tests: Critical user journeys

## Available Test Suites

### Client-Side Tests
- Component Unit Tests (`client/src/tests/unit/`)
  - Button component tests
  - Other React component tests

### Server-Side Tests
- API Integration Tests (`server/tests/integration/`)
  - Posts endpoint tests
  - Other API endpoint tests

## Debugging

The project includes various debugging configurations:
- Jest debugging setup
- React component debugging tools
- API endpoint testing utilities

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Resources

- [Jest Documentation](https://jestjs.io/docs/getting-started)
- [React Testing Library Documentation](https://testing-library.com/docs/react-testing-library/intro/)
- [Supertest Documentation](https://github.com/visionmedia/supertest)
- [Cypress Documentation](https://docs.cypress.io/)
- [MongoDB Testing Best Practices](https://www.mongodb.com/blog/post/mongodb-testing-best-practices) 