# Agent-X

An intellectual proof-of-concept demonstrating an AI agentic tool for autonomous content creation on the X platform. This project leverages the Google Gemini API to dynamically generate context-aware, on-brand content. It serves as a foundational study in using large language models to manage a consistent and engaging digital presence.

## Features

* **Autonomous Content Generation:** Utilizes the Google Gemini API to produce original, coherent posts based on a defined persona and theme.
* **Agentic Behavior:** The core logic simulates an AI agent that can generate content with minimal human intervention.
* **Persona Management:** The system prompt is engineered to guide the AI in adopting a specific tone, style, and domain expertise.
* **Secure API Key Handling:** Employs `python-dotenv` for managing API keys through environment variables, ensuring credentials are not exposed in the codebase.
* **Modular Python Structure:** The code is organized for clarity, maintainability, and future expansion.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

* Python 3.8 or higher installed on your system.
* A Google account to access Google AI Studio.

### Installation

1.  **Clone the Repository**

    ```bash
    git clone [https://github.com/ishitaakolkar/Agent-X.git](https://github.com/ishitaakolkar/Agent-X.git)
    cd your-repo-name
    ```


2.  **Create and Activate a Virtual Environment (Recommended)**

    ```bash
    # For macOS / Linux
    python3 -m venv venv
    source venv/bin/activate

    # For Windows
    python -m venv venv
    venv\Scripts\activate
    ```

3.  **Install Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

### Configuration

1.  **Obtain Your Gemini API Key**

    * Navigate to [Google AI Studio](https://aistudio.google.com/app/apikey).
    * Click "Create API key in a new project" and **copy the key immediately**.

2.  **Set Up the API Key as an Environment Variable**

    For security, you must never commit your API key directly to your repository. Use a `.env` file to manage your key locally.

    * Create a file named `.env` in the root directory of your project.
    * Add the following line, replacing `YOUR_API_KEY` with the key you copied:

    ```ini
    GOOGLE_API_KEY="YOUR_API_KEY"
    ```

    * This `.env` file is already listed in the `.gitignore` file, so it will not be committed to GitHub.

## Usage

To run the AI agent, simply execute the main Python script from your terminal:

```bash
python tweet_generator.py
