# Workflow

The **module3_task** workflow is a GitHub Actions workflow that automates the validation of our website's codebase. This workflow is triggered on a daily basis, as well as whenever there is a new code push to the main branch of the repository.

The workflow consists of three steps:

- Clone the repository
- Use ubuntu-22.04 as the virtual machine
- Execute the make help command to validate that the Makefile is present and implements the help target

By automating the validation process, the module3_task0 workflow ensures that our codebase is always ready to be deployed and that the build process is up to date. Additionally, it provides us with an easy way to monitor the health of our codebase and catch errors before they make it into production.
