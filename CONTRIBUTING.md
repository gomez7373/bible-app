
# Contributing to Bible App

We welcome contributions to the Bible App project! Whether you're fixing a bug, adding a new feature, or improving documentation, your contributions are valued.

---

## Getting Started

### Fork and Clone the Repository
1. Fork the repository on GitHub.
2. Clone your forked repository to your local machine:
   ```bash
   git clone https://github.com/your-username/bible-app.git
   cd bible-app
   ```

### Set Up Your Environment
1. Install dependencies for both the frontend and backend:

   - **Backend**:
     ```bash
     cd backend
     npm install
     cp .env.example .env  # Configure your .env file
     npm run dev           # Start backend server
     ```

   - **Frontend**:
     ```bash
     cd frontend
     npm install
     npm start             # Start React development server
     ```

2. Ensure the app is running on `http://localhost:3000`.

---

## Coding Standards

### General Guidelines
- Write clean, readable, and well-documented code.
- Follow the existing file and directory structure.
- Ensure your code passes all existing tests.

### Frontend Standards
- Use functional React components and React hooks where applicable.
- Ensure the UI is responsive and accessible.
- Use `styled-components`, `TailwindCSS`, or other project-approved libraries for styling.

### Backend Standards
- Follow RESTful API design principles.
- Use proper HTTP status codes for API responses.
- Validate user inputs and handle errors gracefully.

### Testing
- Write unit tests for all new features.
- Use `Jest` for testing both frontend and backend.
- Run tests before submitting changes:
  ```bash
  npm test
  ```

---

## Making Changes

### Branching Model
- Use the following branching model for collaboration:
  - `main`: Stable production-ready code.
  - `develop`: Latest code under active development.
  - `feature/branch-name`: New features or enhancements.
  - `bugfix/branch-name`: Bug fixes.

### Create a Feature Branch
1. Create a branch for your changes:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. Make your changes and commit them:
   ```bash
   git add .
   git commit -m "Add your feature description"
   ```

3. Push the branch to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

---

## Submitting Your Work

### Open a Pull Request
1. Navigate to the original repository on GitHub.
2. Click on the "Pull Requests" tab and open a new pull request.
3. Provide a detailed description of your changes and link to any relevant issues.

### Pull Request Checklist
- [ ] Code follows the project's style guidelines.
- [ ] Changes are tested and passing locally.
- [ ] Documentation is updated (if necessary).

---

## Reporting Issues

### Found a Bug?
1. Check the [Issues](https://github.com/your-username/bible-app/issues) section to see if it’s already reported.
2. If not, create a new issue and include:
   - Steps to reproduce the issue.
   - Expected and actual behavior.
   - Relevant screenshots or logs (if any).

### Have a Feature Request?
1. Check the [Issues](https://github.com/your-username/bible-app/issues) section to see if it's already suggested.
2. If not, create a new issue with:
   - A clear explanation of the feature.
   - How it will benefit the project.

---

## Need Help?
Feel free to reach out by opening a GitHub issue or contacting the project maintainers.

Thank you for contributing to the Bible App!
