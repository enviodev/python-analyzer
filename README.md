# Python-Analyzer

You can use this code to easily analyze and manipulate indexed data frome envio that is held in postgres.

# Setup Guide for Python Projects with Rye and Jupyter Notebook in VS Code

This guide provides a step-by-step process for setting up a Python development environment using `rye`, a package manager for Python that simplifies managing Python versions and dependencies. This is especially useful for users transitioning from Node.js to Python. We'll also cover how to configure a Jupyter Notebook in Visual Studio Code to use the Python environment created by `rye`.

## Installation Steps

### 1. Install Rye

`rye` is a modern package manager for Python that offers an experience similar to what Node.js developers are accustomed to with `npm`, `yarn`, `pnpm`, or `bun`. It helps in managing Python versions and project dependencies effortlessly.

To install `rye`, open your terminal or command prompt and execute the following command:

```bash
curl -sSf https://rye-up.com/get | bash
```

This command fetches and runs the rye installation script. It's a quick process that prepares rye for use on your machine.

### 2. Initialize The Project with Rye

Simply run:

```bash
rye sync
```

This command initializes rye for our project. It creates a .venv virtual environment and installs the correct version of Python along with any dependencies defined in a rye.toml file.

### 3. Configuring VS Code and Jupyter Notebook

To work with Jupyter Notebooks in Visual Studio Code, you'll need to install the ms-python.python and ms-toolsai.jupyter extensions if you haven't done so already.

Open VS Code and navigate to the Extensions view by clicking on the square icon on the sidebar or pressing Ctrl+Shift+X.
Search for "Python" and install the extension provided by Microsoft (ms-python.python).
Search for "Jupyter" and install the Jupyter extension provided by Microsoft (ms-toolsai.jupyter).
After installing these extensions, open your project in VS Code and create a new Jupyter Notebook file (.ipynb).

To select the Python interpreter from the .venv created by rye:

Click on the Python version in the bottom-left corner of the VS Code window.
Choose "Enter interpreter path..." > "Find..."
Navigate to your project directory, and select the Python interpreter inside the .venv directory.
Your Jupyter Notebook is now configured to use the Python environment managed by rye.
