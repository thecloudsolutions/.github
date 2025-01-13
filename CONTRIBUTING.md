# 📓 Contributing

First and foremost, thank you for considering contributing to Cloud Solutions! We truly appreciate your interest and effort in making our community better. 🧑‍💻 The future of Open Source relies on you!

## 🌟 Code of Conduct

Cloud Solutions is dedicated to providing a welcoming, inclusive, and harassment-free environment for all. Please review our [Code of Conduct](CODE_OF_CONDUCT.md) to understand the behaviors expected within our community and the actions that will not be tolerated.

## 🛠️ Before You Start

### Cloud Solutions Projects

Every Cloud Solutions project is housed in its own repository on GitHub. Before you start contributing, familiarize yourself with the specific project you're interested in. Each repository includes a `README.md` file that provides:

- A project overview.
- Setup instructions.
- Details on running tests.

Feel free to explore and understand the project's structure before diving in.

## 🚀 How To Contribute

### Reporting Bugs

Help us improve by reporting bugs. Here's how:

1. **Search Existing Issues**: Check if the issue is already reported on GitHub.
2. **Submit a Detailed Report**:
   - Use the provided issue template.
   - Include clear steps to reproduce the bug.
   - Provide relevant system details (e.g., OS, environment).

### Suggesting Enhancements

Have an idea for improvement? Follow these steps:

1. Open a feature request via GitHub Issues.
2. Clearly describe the feature, its benefits, and potential use cases.
3. Reference any related issues or discussions if available.

### Contributing Code

If you want to dive into the codebase, here’s how:

1. Search for issues labeled `help-wanted` or `good-first-issue` to get started.
2. Fork the repository and create a new branch.
3. Ensure your changes adhere to our coding standards (see Style Guides).
4. Submit a Pull Request (PR) with a detailed description of your changes.
5. Address any feedback from maintainers promptly.

## 🔄 Pull Requests

To submit a Pull Request:

1. Follow all instructions in the [Pull Request template](.github/PULL_REQUEST_TEMPLATE.md).
2. Ensure all automated tests pass before submitting.
3. Use clear, concise commit messages (refer to our [Style Guide](#StyleGuide)).
4. Mention relevant issues (e.g., “Closes #123”).

Once submitted, a maintainer will review your PR. Additional feedback, testing, or changes may be requested before it is merged.

## 🇽🇾🇿 Versioning

Versioning is an essential part of maintaining consistency and clarity in project releases. Cloud Solutions follows [**Semantic Versioning (SemVer)**](https://semver.org/) principles to communicate the impact of changes effectively. Here's how it works:

1. **patch (`x.y.Z`)**: Used for bug fixes or small updates that do not change functionality.
2. **minor (`x.Y.z`)**: Introduced for new features that remain backward-compatible.
3. **major (`X.y.z`)**: Reserved for changes that are not backward-compatible or represent a significant evolution.
4. **no-release**: If a release does not need to be created, the changes may be labeled as `no-release`.

When creating a Pull Request, contributors do not need to assign version labels. Maintainers will determine the appropriate version increment based on the nature of the changes.

## ⌨️ Style Guide

### Git Commit Messages

- Use present tense (e.g., "Add feature" not "Added feature").
- Keep the first line under 72 characters.
- Explain "why" in the body if necessary.
- Use the imperative mood ("Move source to..." not "Moves source to...")

### Coding Standards

- Adhere to the project’s coding conventions outlined in its `README.md` or style guides.
- Write clean, readable, and maintainable code.

## ☁️ Terraform Contributions

If you're contributing to a Terraform repository, follow these detailed guidelines:

### Documentation Updates

- Always update `README.md` to reflect new variables, outputs, or changes.
- Maintain clear and consistent descriptions for variables and outputs.

### Examples

- Update or add examples in the `examples/` directory.
- Ensure examples use realistic and representative values.
- Confirm examples align with the latest module updates.

### Testing Terraform Modules

1. **Local Testing**:
   - Use `terraform plan` and `terraform apply` to verify changes.
   - Ensure the test environment is isolated (e.g., a dedicated AWS account).
2. **Automated Testing**:
   - Write tests using [Terratest](https://terratest.gruntwork.io/) (Go-based testing framework).
   - Place test cases in the `test/src` directory.
   - Validate changes with assertions on resource outputs.

### Deprecation Guidelines

- Move deprecated variables or resources to `variables-deprecated.tf`.
- Provide clear warnings and fallback mechanisms in the documentation.
- Reference replacement variables or approaches in both code and docs.

### Automated Checks

- Ensure that PRs pass:
  - Linting tools (e.g., `terraform fmt` or `tflint`).
  - Validation with `terraform validate`.
  - Tests in CI/CD pipelines.
- Maintainers will run final tests using isolated environments before merging.

## 🔗 Attribution

This CONTRIBUTING guide is inspired by best practices and tailored for the Cloud Solutions community.

Thank you for your contribution! We’re excited to build a better community together.
