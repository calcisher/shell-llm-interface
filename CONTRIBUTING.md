# Contributing to ask

Thank you for your interest in improving this project! To maintain the minimalist and portable nature of this tool, please follow these guidelines:

## Contribution Process
1. **Fork the Repository:** Create your own copy of the project.
2. **Branching:** Create a feature branch for your changes (`git checkout -b feature/NewFeature`).
3. **Commit Messages:** Use clear and meaningful commit messages that explain the "why" and "what".
4. **Pull Requests:** Open a PR describing your changes in detail.

## Strict Rules
- **No New Dependencies:** Contributions must NOT add any dependencies other than `bash`, `curl`, and `jq`.
- **POSIX Compatibility:** Ensure the script remains portable across different Unix-like environments.
- **Conciseness:** Keep the script logic simple and easy to read.

## Testing
Before submitting a PR, please test the script with:
- Direct arguments: `./ask "test prompt"`
- Piped input: `echo "test" | ./ask "prompt"`
- Combined input: `echo "test" | ./ask "prompt" -`

---
*By contributing to this project, you agree that your contributions will be licensed under the MIT License.*