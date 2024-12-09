
# Next.js Starter Project

## Project Integrations

### Frameworks and Core Libraries
- **Next.js 15**: Modern React framework for building server-rendered applications with powerful features like Turbopack for faster builds.
- **React 19**: Core library for building UI components.
- **TypeScript 5**: Type-safe JavaScript for better development experience.

### Code Quality Tools
- **Biome**:
  - Used for linting and formatting.
  - Commands:
    - `pnpm run lint`: Runs Biome linting to check for code quality issues.
    - `pnpm run format`: Formats the code automatically.
    - `pnpm run lint-and-format`: Combines both linting and formatting.
- **Commitlint**:
  - Ensures commit messages follow the **Conventional Commit** format.
  - Integrated via Lefthook for automated checks during commits.

### Automation and Git Hooks
- **Lefthook**:
  - Manages Git hooks for automating pre-commit and commit-message tasks.
  - Automates the following:
    - **Linting**: Runs `pnpm run lint` before committing.
    - **Formatting**: Runs `pnpm run format` on staged files before committing.
    - **Commit Message Validation**: Uses Commitlint to ensure commit messages follow conventions.

### TypeScript Type Definitions
- **@types/node**: Type definitions for Node.js.
- **@types/react**: Type definitions for React.
- **@types/react-dom**: Type definitions for React DOM.

### Package Manager
- **pnpm**: Fast and efficient package manager for managing dependencies.

### Prepare Script
- **`prepare` Script**:
  - Ensures Lefthook is installed automatically when running `pnpm install`.

## Example Workflow

1. **Install Dependencies**:
   ```bash
   pnpm install
   ```

2. **Development**:
   - Start the development server:
     ```bash
     pnpm run dev
     ```
   - Automatically lint and format code:
     - During commits (Lefthook).
     - Manually with:
       ```bash
       pnpm run lint
       pnpm run format
       ```

3. **Committing Changes**:
   - Ensure commit messages follow conventions.
   - Lefthook runs linting, formatting, and Commitlint validation automatically.

4. **Deployment**:
   - Use **Vercel CLI** for seamless deployment:
     ```bash
     vercel
     ```

## Integration Checklist

| **Tool**                | **Purpose**                                       |
|-------------------------|---------------------------------------------------|
| **Next.js**             | Core framework for the application.               |
| **React**               | UI components.                                    |
| **TypeScript**          | Static type checking.                             |
| **Biome**               | Linting and formatting.                           |
| **Commitlint**          | Commit message validation.                        |
| **Lefthook**            | Automates Git hooks for linting and formatting.   |
| **pnpm**                | Efficient package manager.                        |
| **Type Definitions**    | Ensures type safety for Node.js, React, and DOM.  |
