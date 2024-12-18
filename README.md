# Vue 3 Project Template with Husky, Lint-Staged, Conventional Commits, ESLint, and Prettier

This project template provides a basic setup for a Vue 3 application using the most common packages to ensure clean and consistent code. It includes pre-configured tools for:

- Linting code with ESLint for JavaScript and Vue files
- Automatically formatting code with Prettier
- Managing Git hooks with Husky
- Running linters on staged files with lint-staged
- Enforcing Conventional Commits for consistent commit messages

## Project Setup

Follow these steps to get your development environment up and running.

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn (package managers)

#### Clone the repository

```
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```

#### Install dependencies

Install the project dependencies using npm or yarn:

**With npm:**

```
npm install
```

**With yarn:**

```
yarn install
```

#### Setup Husky and Lint-Staged

The project uses Husky for running Git hooks and lint-staged to ensure that only the files you’ve changed are linted and formatted before committing. These tools are automatically set up when you install dependencies.

- Pre-commit hook will run lint-staged, which will run linters (ESLint, Prettier) on your staged files before committing.

#### Commit Convention (Conventional Commits)

The project follows the Conventional Commits specification for commit messages. Here's the basic format:

```
<type>(<scope>): <message>

<type> can be one of:
- feat: a new feature
- fix: a bug fix
- docs: documentation changes
- style: code style changes (white-space, formatting, etc.)
- refactor: code refactoring
- test: adding or updating tests
- chore: maintenance tasks
```

You can use tools like [Commitizen](https://commitizen-tools.github.io/commitizen/) to help you generate the proper commit messages.


#### Linting and Formatting

- ESLint is used to enforce coding standards in JavaScript and Vue files.
- Prettier is used to format the code for consistent style.

Run the following command to lint and format your code manually:

**With npm:**

```
npm run lint
npm run format
```

**With yarn:**

```
yarn lint
yarn format
```

#### Lint and Format Check

To check for linting errors or formatting issues, you can run:

**With npm:**

```
npm run lint:check
npm run format:check
```

**With yarn:**

```
yarn lint:check
yarn format:check
```

#### Husky Configuration
The project is configured with Husky to enforce pre-commit hooks. The hooks include:

- Pre-commit: runs lint-staged to lint and format staged files
- Commit-msg: checks commit messages to follow the Conventional Commit format

### Links

- [Vue 3](https://vuejs.org/)
- [Husky](https://typicode.github.io/husky/)
- [Lint-Staged](https://github.com/lint-staged/lint-staged)
- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- [ESLint](https://eslint.org/)
- [Prettier](https://prettier.io/)