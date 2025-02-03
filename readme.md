# GradSchool Seminar on Feb. 3rd 2025: AI-pair-programming with aider and cline

## Workshop Setup / Prerequisites
- Ensure you have Python 3.10 or later installed. If not, download it from [python.org](https://www.python.org/downloads/).
- Git is also necessary [download git](https://git-scm.com/downloads).
- For cline an IDE is needed- I recommend using VS Code (e.g. portable version) [get VS Code portable](https://code.visualstudio.com/docs/editor/portable)
---

## 🔧 Installing Aider

[aider](https://aider.chat/) is an AI-assisted coding tool working based on git and is a terminal tool. To install it, follow these steps:

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

# add aider to your path


# Change directory into your code base
cd /to/your/project

# Work with GPT-4o-mini on your code
aider --model gpt-4o-mini --api-key openai=your-key-goes-here

# Or start via config:
aider --config .aider-openai.conf.yml # with gpt-4o-mini & o3-mini via OpenAI-API
aider --config .aider-deepseek.conf.yml # with deepseek-V3 & deepseek-R1 via GLHF-API

```
For the usage and command-overview in aider see:
> * https://aider.chat/docs/usage.html
> * https://aider.chat/docs/usage/commands.html
> * https://aider.chat/docs/usage/tips.html

Aider is highly versatile so you could use an `.aider.conf.yaml` to configure certain things like "architect model", "editor-model", "command-line-behavior", etc.
see `.aider.conf.yaml` and use it as an example and have a look here: [aider-config](https://aider.chat/docs/config.html)

---

## 🛠️ Integrating Cline in VS Code

[cline](https://github.com/cline/cline) is a coding ai agent extension that can be easily set up in VS Code:

1. **Installation:**
   - Open VS Code
   - Press `Ctrl + Shift + X` or navigate to `Extensions` (on the left)
   - type cline and install the extension
   - after installation: click on the new cline icon on the left menu

2. **Necessary settings:**
   - choose api provider: for us OpenAI
   - add api-key
   - go to settings and choose "GPT-4o-mini"

3. **Lets go:**
   - start the extension in a fresh workspace, let it create and activate a venv and type your plans or what you want to build.
     
---

### 🚀 Ready for the Workshop!
After installation, you can now use aider and cline directly in VS Code terminal or as IDE-extension. Enjoy the workshop! 🎉

### 🎓 Lets try the examples...
See example prompts in `examples.md`or be brave and test it with your own projects
