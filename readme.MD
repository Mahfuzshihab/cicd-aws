# CI/CD Pipeline

This repository contains a simple Continuous Integration / Continuous Deployment (CI/CD) pipeline configured using GitHub Actions.

## Workflow Overview

- The workflow triggers on every push to the repository.
- It runs on an Ubuntu latest virtual environment.
- Steps include:
  - Checking out the repository code.
  - Running simple script commands.
  - Simulating an error (for testing failure handling).

## Workflow Steps

1. **Checkout code:** Uses `actions/checkout@v2` to get the repository content.
2. **Run scripts:** Runs simple `echo` commands to demonstrate step execution.
3. **Simulate error:** Intentionally fails the workflow to demonstrate failure handling.
4. **Additional greetings:** Prints a second greeting message (this step will be skipped if the error step fails).

## Usage

- Push changes to any branch to trigger the workflow.
- View the workflow status and logs in the **Actions** tab of your GitHub repository.

## Notes

- The simulated error step (`exit 1`) is used for demonstration purposes. Remove or comment it out to let the pipeline run successfully.
- Customize the workflow file (`.github/workflows/ci-cd.yml`) to fit your project needs.

---

Feel free to extend this README with more details about your specific build, test, and deployment steps!

