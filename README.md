# ci-cd-examples

## Overview

### Continuous Integration (CI) Pipeline:

CI ensures that changes made to the codebase are regularly integrated into a shared repository, and each integration is verified by an automated build and automated tests before being merged into the main branch.

#### CI Steps:

- Linting: Run a linter (e.g., ESLint) to ensure code consistency and style across the codebase.
- Unit Tests: Execute unit tests to verify the functionality of individual components.
- Integration Tests: Run integration tests to ensure that different parts of the application work together correctly.
- Build: Build the application assets (React frontend, Express backend).
- Artifact Generation: Generate artifacts (e.g., Docker images) that can be deployed to various environments.

### Continuous Deployment (CD) Pipeline:

CD automates the deployment process, allowing changes that pass through the CI pipeline to be automatically deployed to the desired environment.

#### CD Steps:

- Deploy to Development: Deploy the built application to a development environment for further testing and validation.
- Deploy to Staging: Deploy the application to a staging environment that closely resembles the production environment. This allows for final pre-production testing.
- Deploy to Production: If all tests pass in the staging environment, automatically deploy the application to the production environment.

## List of examples CI/CD pipelines

- Add .gitlab-ci.yml file to your repository/project
- 

### NodeReactExpressMongo CI/CD Pipeline

This workflow is triggered on pushes to the main branch. It performs 

- linting,
- unit testing,
- integration testing,
- builds the application,
- generates a Docker image,
- and then deploys it to different environments

based on your deployment scripts.

## Read More

- [Read more about building your application](https://docs.gitlab.com/ee/tutorials/build_application.html)
