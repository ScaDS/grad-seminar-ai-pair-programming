# GradSchool Seminar on Feb. 3rd 2025: AI-pair-programming with aider and cline

## Workshop Setup
## 🔧 Installing Aider

Aider is an AI-assisted coding tool working based on git and is a terminal tool. To install it, follow these steps:

### 1. Create a Virtual Environment (Recommended)
Depending on your operating system, use the following commands to create and activate a virtual environment:

**Windows (PowerShell):**
```sh
python -m venv aider_env
./aider_env/Scripts/activate
```

**Mac/Linux (bash/zsh):**
```sh
python3 -m venv aider_env
source aider_env/bin/activate
```

### 2. Install Aider
Once the virtual environment is activated, install Aider using:
```sh
python -m pip install aider-install
aider-install

# Change directory into your code base
cd /to/your/project

# Work with GPT-4o on your code
aider --model gpt-4o-mini --api-key openai=your-key-goes-here
```
Ensure you have Python 3.10 or later installed. If not, download it from [python.org](https://www.python.org/downloads/).

---

## 🛠️ Integrating Cline in VS Code

[Cline](https://github.com/cline/cline) is a coding ai agent extension that can be easily set up in VS Code:

1. **Installation:**
   - Open VS Code
   - Press `Ctrl + Shift + X` or navigate to `Extensions` (on the left)
   - type cline and install the extension
   - after installation: click on the new cline icon on the left menu

2. **Necessary settings:**
   - choose api provider: for us OpenAI
   - add api-key
   - go to settings and choose "GPT-4o-mini"


---

### 🚀 Ready for the Workshop!
After installation, you can now use aider and cline directly in VS Code terminal or as IDE-extension. Enjoy the workshop! 🎉

### 🎓 Lets try the examples...
See example prompts in `example.md`
