# AI Coding Agent Guidelines for DevSecOps Tic Tac Toe Project

Welcome to the DevSecOps Tic Tac Toe project! This document provides essential guidelines for AI coding agents to be productive in this codebase. Please follow these instructions to ensure consistency and alignment with the project's architecture and conventions.

## Project Overview

This project implements a Tic Tac Toe game with the following features:
- **Frontend**: Built with React, TypeScript, and Tailwind CSS.
- **Game Logic**: Encapsulated in `src/utils/gameLogic.ts`.
- **Components**: Modular React components for the board, squares, score tracking, and game history.
- **DevSecOps Pipeline**: Kubernetes manifests for deployment and CI/CD workflows.

## Key Files and Directories

- `src/components/`: Contains React components. Follow the existing modular structure.
- `src/utils/gameLogic.ts`: Centralized game logic. Ensure any updates maintain the integrity of game rules.
- `kubernetes/`: Deployment configurations for Kubernetes.
- `.github/workflows/ci-cd.yml`: Defines the CI/CD pipeline.
- `README.md`: Provides an overview of the project and setup instructions.

## Development Workflow

### Setting Up the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/devsecops-demo.git
   cd devsecops-demo
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

### Testing
- Unit tests are located in `src/__tests__/`.
- Run tests with:
  ```bash
  npm test
  ```

### Building for Production
- Create a production build with:
  ```bash
  npm run build
  ```

## Project-Specific Conventions

- **Component Structure**: Each React component should be self-contained with its styles and logic.
- **Game Logic**: Any changes to `gameLogic.ts` must preserve the rules outlined in `README.md`.
- **Styling**: Use Tailwind CSS for all styling. Avoid inline styles unless necessary.
- **Testing**: Write unit tests for all new utilities and components.

## Integration Points

- **Kubernetes**: Ensure any changes to `kubernetes/` files align with the CI/CD pipeline.
- **CI/CD**: Validate changes against the pipeline defined in `.github/workflows/ci-cd.yml`.

## Examples

### Adding a New Component
1. Create the component in `src/components/`.
2. Write unit tests in `src/__tests__/`.
3. Import and use the component in `App.tsx`.

### Updating Game Logic
1. Modify `src/utils/gameLogic.ts`.
2. Update or add tests in `src/__tests__/gameLogic.test.ts`.
3. Verify the game rules remain consistent.

---

For any questions or clarifications, refer to the `README.md` or consult the CI/CD pipeline logs.