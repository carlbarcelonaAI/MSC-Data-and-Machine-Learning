# MSC Event 1: Environment Setup

Choose your preferred environment (**Cloud** or **Local**) and run the setup commands in your terminal.

## ☁️ Option A: GitHub Codespaces (Cloud)

Launch your Codespace from the repository to get started.

1. Open the integrated terminal
2. Run the following commands:

```bash
# 1. Sync packages (using copy mode for cloud storage compatibility)
uv sync --link-mode=copy

# 2. Register the kernel to Jupyter
uv run python -m ipykernel install --user --name msc-event1-kernel --display-name "Python 3.11 (.venv)"
```

➡️ To start coding:  
Open **chicago_analysis.ipynb**, click **Select Kernel** (top right), choose **Jupyter Kernels / Python Environments**, and select **Python 3.11 (.venv)**.

## 💻 Option B: Local Machine

Ensure you have **Python 3.11**, **Git**, and **VS Code** installed.  
Install `uv` via:

- **Mac/Linux**:  
  ```bash
  curl -LsSf https://astral.sh/uv/install.sh | sh
  ```
- **Windows**:  
  ```powershell
  powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
  ```

Then run:

```bash
# 1. Clone the repository and navigate to the project folder
git clone https://github.com/carlbarcelonaAI/MSC-Data-and-Machine-Learning.git
cd MSC-Data-and-Machine-Learning

# 2. Build the virtual environment and sync dependencies
uv sync

# 3. Register the kernel to Jupyter
uv run python -m ipykernel install --user --name msc-event1-kernel --display-name "Python 3.11 (.venv)"
```

➡️ To start coding:  
Open the folder in VS Code (`code .`), open **chicago_analysis.ipynb**, click **Select Kernel** (top right), choose **Python Environments**, and select **Python 3.11 (.venv)**.
