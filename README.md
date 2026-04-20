# ask - A Minimalist Bash LLM Interface

`ask` is a lightweight, POSIX-compliant command-line tool designed to interact with OpenAI-compatible Chat Completion APIs. It is built for speed and portability, requiring only standard Unix utilities.

## Features
- **Zero Heavy Dependencies:** Built using only `bash`, `curl`, and `jq`.
- **Environment Driven:** Securely handles API credentials via environment variables.
- **Pipe Support:** seamlessly integrates into shell pipelines.
- **Concise Output:** Optimized for CLI usage with "no-yapping" system prompts.

## Installation
Ensure you have `jq` installed:
- **macOS:** `brew install jq`
- **Linux:** `sudo apt-get install jq`

Clone the repository and make the script executable:
```bash
git clone https://github.com/calcisher/shell-llm-interface.git 20220602036_Hasan_Berk_Görgülü
chmod +x ask
```
