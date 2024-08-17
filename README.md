# 🧠 Omni Engineer: An AI-Powered Developer Console
An intelligent assistant designed to enhance your development workflow with flexible model selection.

## 🔍 Overview
Omni Engineer is a console-based tool that integrates AI capabilities into your development process. It offers smart responses to coding queries, file management, web searching, and image processing functionalities. The latest update introduces model-specific parameters, allowing users to choose and configure different AI models for various tasks.

Omni Engineer is a spiritual successor to [Claude Engineer](https://github.com/Doriandarko/claude-engineer). It was built from extensive usage of hand-made AI tools, trial and error, and feedback received. Compared to Claude Engineer, this new script allows for more control via simplicity while introducing new functionalities like multi-file editing, save/resume of chats, and now, flexible model selection.

This framework is suitable for developers who want to code with an advanced AI assistant, offering customization options to tailor the experience to their needs.

## 🌟 Features
- AI-Powered Responses with Flexible Model Selection
- File Management (Add, Edit, Create)
- Web Searching
- Image Processing
- Undo Functionality
- Conversation Save & Load
- Model-Specific Configuration Options
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
3. Rename the .env.example to .env and add your API Keys:
   ```
   DEFAULT_API_KEY="Your default model API key"
   EDITOR_API_KEY="Your editor model API key"
   ```
4. Run the main script with optional configuration:
   ```
   python main.py [--default-model MODEL] [--editor-model MODEL] [--default-api-base BASE_URL] [--editor-api-base BASE_URL] [--default-api-key API_KEY] [--editor-api-key API_KEY]
   ```

## 🔧 Configuration
Omni Engineer now supports model-specific parameters, allowing for greater flexibility in AI model selection and configuration. The script accepts the following command-line parameters:

- `--default-model`: Specify the AI model to use for default completion (default is "claude-3-sonnet-20240229")
- `--editor-model`: Specify the AI model to use for editor completion (default is "openai/gcp/gemini-pro-1.5")
- `--default-api-base`: Set the base URL for the default model API
- `--editor-api-base`: Set the base URL for the editor model API
- `--default-api-key`: Provide the API key for the default model
- `--editor-api-key`: Provide the API key for the editor model

Example usage:
```
python main.py --default-model gpt-4 --editor-model claude-3-opus-20240229 --default-api-base https://api.openai.com/v1 --editor-api-base https://api.anthropic.com --default-api-key your_openai_key --editor-api-key your_anthropic_key
```

These parameters allow you to easily configure different models for various tasks within the application. You can also set these values in the .env file for persistent configuration.
## 📚 Usage
After launching the console, enter commands or questions as needed. The AI will respond accordingly, assisting with various development tasks. You can use different models for default interactions and editing tasks by configuring the appropriate parameters.

### Model-Specific Parameters
- Default Model: Used for general interactions and responses.
- Editor Model: Specifically used for code editing tasks.

You can configure these models separately, allowing you to optimize performance for different types of tasks. For example, you might use a more powerful model for complex code editing, while using a faster model for general queries.
## 🤖 AI Models
Omni Engineer utilizes OpenRouter to access a variety of AI models. For detailed information on available models and their capabilities, refer to [OpenRouter's documentation](https://openrouter.ai/models).
## 🐛 Issue Reporting
Please use the issue tracker only for reporting actual bugs in the code. This helps keep the issue tracker focused on improving the project's stability and functionality.

## ⭐️ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Doriandarko/omni-engineer&type=Date)](https://star-history.com/#Doriandarko/omni-engineer&Date)
