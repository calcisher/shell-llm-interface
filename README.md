# ask - A Bash LLM Interface

`ask` is a lightweight, POSIX-compliant command-line tool designed to interact with OpenAI-compatible Chat Completion APIs. It is built for speed and portability, requiring only standard Unix utilities.

## Requirements
- Bash
- curl
- jq


## Installation
Ensure you have `jq` installed:
- **macOS:** `brew install jq`
- **Linux:** `sudo apt-get install jq`

Clone the repository and make the script executable:
```bash
git clone https://github.com/calcisher/shell-llm-interface.git 20220602036_Hasan_Berk_Görgülü
chmod +x ask
```

## Environment Variables

```bash
export ASK_API_URL="https://api.groq.com/openai/v1/chat/completions"
export ASK_MODEL="llama-3.3-70b-versatile"
export ASK_API_KEY="your-api-key"
```

## Usage

```bash
# direct prompt
./ask "What is the capital of France?"

# piped input 
cat logs.txt | ./ask "Explain these errors:"
```

## Known Limitations

No Streaming: Output is displayed only after the full response is received from the API.

Stateless: The tool does not maintain conversation history; each call is a completely fresh session.

Plain Text: No Markdown rendering or ANSI colors in the terminal output.

Dependencies: Strictly requires curl and jq to be installed on the host machine.

## License

This project is licensed under the **MIT License**.

I chose the **MIT License** because it is highly permissive and lightweight. It encourages open-source collaboration and allows for maximum code reuse with minimal restrictions, which fits the minimalist nature and philosophy of this tool.


