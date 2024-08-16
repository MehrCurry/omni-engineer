# 🧠 Omni Engineer: An AI Agents Powered Developer Console
An intelligent assistant designed to enhance your development workflow.
## 🔍 Overview
Omni Engineer is a console-based tool that integrates AI capabilities into your development process. It offers smart responses to coding queries, file management, web searching, and image processing functionalities.

Omni Engineer is a spiritual successor to [Claude Engineer](https://github.com/Doriandarko/claude-engineer). It was built from my extensive usage of hand-made AI tools, trial and error, and feedback received. Compared to Claude Engineer, this new script allows for more control via simplicity while leaving some of the other functionalities like a fully automated flow, or the ability to run code. 
At the same time, bring some cool new stuff like multi-file editing and save/resume of chats.
I see this framework as more suitable for people who actually want to code with a better assistant on their side, versus something that is fully automatic.

## 🌟 Features
- AI-Powered Responses
- File Management (Add, Edit, Create)
- Web Searching
- Image Processing
- Undo Functionality
- Conversation Save & Load
## 🖥️ Commands
- `/add <filepath>`: Add files to AI context
- `/edit <filepath>`: Edit existing files
- `/new <filepath>`: Create new files
- `/search`: Perform web searches
- `/image <filepath/url>`: Add images to context
- `/clear`: Clear AI memory
- `/reset`: Reset the session
- `/diff`: Toggle diff display
- `/history`: View chat history
- `/save`: Save current chat
- `/load`: Load a previous chat
- `/undo <filepath>`: Undo last file edit
## 🚀 Installation
1. Clone the repository:
   ```
   git clone https://github.com/doriandarko/omni-engineer.git
   cd omni-engineer
   ```
2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```
3. Rename the .env.example to .env and add your API Key:
   ```
   OPENROUTER_API_KEY="Your key"
   ```
4. Run the main script:
   ```
   python main.py [--model MODEL] [--openai-api-base BASE_URL] [--openai-api-key API_KEY]
   ```

## 🔧 Configuration
Omni Engineer now uses LiteLLM, which provides a unified interface to various AI models and providers. This allows for greater flexibility in model selection and API usage. The script accepts the following command-line parameters:

- `--model`: Specify the AI model to use (default is "claude-3-sonnet-20240229")
- `--openai-api-base`: Set the base URL for the API (useful for using different providers)
- `--openai-api-key`: Provide the API key directly in the command line

Example usage:
```
python main.py --model gpt-4 --openai-api-base https://api.openai.com/v1 --openai-api-key your_api_key_here
```

These parameters allow you to easily switch between different models or providers without modifying the code.
## 📚 Usage
After launching the console, enter commands or questions as needed. The AI will respond accordingly, assisting with various development tasks.
## 🤖 AI Models
Omni Engineer utilizes OpenRouter to access a variety of AI models. For detailed information on available models and their capabilities, refer to [OpenRouter's documentation](https://openrouter.ai/models).
## 🐛 Issue Reporting
Please use the issue tracker only for reporting actual bugs in the code. This helps keep the issue tracker focused on improving the project's stability and functionality.

## ⭐️ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Doriandarko/omni-engineer&type=Date)](https://star-history.com/#Doriandarko/omni-engineer&Date)
