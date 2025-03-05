# HACK-UK Website

## Contributing Guide

Welcome to the **HACK-UK Website** project. This guide will help you understand our branching structure and how to contribute effectively.

### Branching Structure

We use a structured approach to manage our development workflow. Below is an overview of the branches and their purposes:

- **[main](https://github.com/HackUK/HackUK-Main/tree/main)** (Deployment Branch)
  - This is the branch where the actual website is deployed.
  - Changes should only be merged into this branch after thorough testing.
  - All updates come from the `[development](https://github.com/HackUK/HackUK-Main/tree/development)` branch.

- **[development](https://github.com/HackUK/HackUK-Main/tree/development)** (Active Development Branch)
  - This is the primary branch for active development.
  - All new features and changes should be directly added to this branch.
  - No need to create separate feature branches—just push your updates here.

- **[pre-development](https://github.com/HackUK/HackUK-Main/tree/pre-development)** (Initial Setup Branch)
  - This was the original branch created using HTML and CSS.
  - It serves as a reference for the early stages of the project.
  - No active development occurs in this branch.

### Commit Message
- **Types of commits:**
     - `feat:` → Adding a new feature (e.g., `feat: add contact form`)
     - `fix:` → Fixing a bug (e.g., `fix: resolve navbar alignment issue`)
     - `change:` → Making general changes (e.g., `change: update footer styles`)
     - `docs:` → Updating documentation (e.g., `docs: update contributing guide`)
     - `style:` → Formatting, missing semicolons, etc. (e.g., `style: fix indentation in CSS`)
     - `chore:` → Maintenance tasks (e.g., `chore: update dependencies`)

   - Example commit:
     ```sh
     git commit -m "feat: add dark mode toggle"
     ```
### How to Contribute

1. **Make Changes Directly in `development`**
   - Instead of creating a new branch, make your updates directly in the `development` branch.
   - Example:
     ```sh
     git checkout development
     ```

2. **Commit Your Changes**
   - After making changes, stage and commit them:
     ```sh
     git add .
     git commit -m "Brief description of changes"
     ```

3. **Push Your Changes**
   - Push your updates directly to the `development` branch:
     ```sh
     git push origin development
     ```

4. **Merge into `main` (Deployment)**
   - Once all features are tested and stable in `development`, they will be merged into `main` for deployment.

### Additional Notes
- Always pull the latest changes before making updates:
  ```sh
  git pull origin development
  ```
- Communicate with the team before making major changes.
- Follow best practices for code organization and readability.

