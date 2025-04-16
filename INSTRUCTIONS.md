# Roo Code Workshop - Setup Instructions

## Goal

Set up Roo Code in Visual Studio Code and connect it to Google Gemini 2.5 Pro using a local Python environment.

## Prerequisites

* Laptop with internet access
* Visual Studio Code
* Python 3.7+ installed (locally)
* Google Account (for Gemini access)

## Tools - Step-by-Step Instructions

1. **Install Visual Studio Code**
    * Download from: <https://code.visualstudio.com>
    * Follow the installer instructions for your OS (Windows/macOS/Linux).

2. **Install Python**
    * Download from: <https://www.python.org/downloads>
    * Install Python with the option to "Add Python to PATH" checked.
    * Confirm installation:
        * Open a terminal in VS Code (`View` > `Terminal`).
        * Run:

            ```bash
            python --version
            ```

3. **Install Python Extension in VS Code**
    * In VS Code, go to Extensions (`Ctrl+Shift+X` or `Cmd+Shift+X`).
    * Search for `Python`.
    * Click `Install` on the official Microsoft extension.

4. **Install Roo Code Extension**
    * In VS Code, open Extensions (`Ctrl+Shift+X` or `Cmd+Shift+X`).
    * Search for: `Roo Code`.
    * Click `Install`.

5. **Set Up a Python Virtual Environment**
    * Open the VS Code terminal.
    * Create a virtual environment:

        ```bash
        python -m venv venv
        ```

    * Activate it:
        * Windows: `venv\Scripts\activate`
        * macOS/Linux: `source venv/bin/activate`
    * Install Flask (if needed for your project, like the example):

        ```bash
        pip install flask
        ```

6. **Get a Google Gemini API Key**
    * Visit: <https://aistudio.google.com>
    * Sign in with your Google account.
    * Go to `API Keys` and create one.
    * Copy your new API key.

7. **Configure Roo Code to Use Google Gemini**
    * Click the Roo Code icon in the left sidebar.
    * Click the Settings icon (gear symbol).
    * In the API configuration area:
        * Provider: Choose `Google Gemini`.
        * API Key: Paste your key.
        * Model: `gemini-2.5-pro` (or your preferred model).
    * Click `Save`/`Apply`.

8. **Test Roo Code**
    * Try this prompt:

        ```
        Create a Flask API with GET /books and POST /books endpoints
        ```

    * Roo Code should generate working code (e.g., in an `app.py` file if you have one open).

---

[x] Done!

You're now ready to:

* Build APIs
* Explore Boomerang features
* Let Roo Code act as your AI pair programmer!
