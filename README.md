# 🤖 AI Agent From Scratch 🚀

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Dependencies](https://img.shields.io/badge/Dependencies-Up%20to%20Date-brightgreen.svg)](https://github.com/RishavB777/AI-Agent-From-Scratch/blob/main/requirements.txt)
![Maintenance](https://img.shields.io/badge/Maintained-Yes-brightgreen.svg)

This project, "AI-Agent-From-Scratch," is a powerful AI agent built from the ground up using Python and Langchain. It's designed to function as a research assistant, capable of answering user queries, conducting web searches, accessing Wikipedia, and saving research output to files.

## ✨ Features

-   **🧠 Intelligent Research Assistant:** The agent is designed to help generate research papers by answering user queries and utilizing various tools.
-   **<0xF0><0x9F><0x97><0x84> Comprehensive Research Response:** Provides structured research responses including topic, summary, sources used, and tools used.
-   **🌐 Web Search:** Integrates DuckDuckGo Search to gather information from the internet.
-   **📚 Wikipedia Access:** Leverages Wikipedia for quick access to a vast repository of knowledge.
-   **💾 Save Research Output:** Includes functionality to save the structured research data to a text file.
-   **🧩 Langchain Integration:** Built using Langchain for creating sophisticated agentic workflows.
-   **🔑 Environment Management:** Uses `python-dotenv` for secure handling of environment variables.
-   **⚙️ Data Validation:** Employs Pydantic for data validation and type hinting, ensuring data consistency.

## ⚙️ Installation

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/RishavB777/AI-Agent-From-Scratch.git](https://github.com/RishavB777/AI-Agent-From-Scratch.git)
    cd AI-Agent-From-Scratch
    ```

2.  **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

3.  **Set up environment variables:**

    * Create a `.env` file in the root directory.
    * Add any necessary API keys or configuration variables to the `.env` file.  (Refer to the documentation of the specific libraries like Anthropic for required variables.)

## 🚀 Usage

1.  **Run the `main.py` script:**

    ```bash
    python main.py
    ```

2.  **Provide a research query when prompted:**

    ```
    What can I help you research? What is the capital of India?
    ```

    The agent will then execute the necessary tools and provide a structured research response.

    ```python
    from main import agent_executer # You might need to adjust this import based on your setup

    if __name__ == "__main__":
        query = input("What can I help you research?")
        raw_response = agent_executer.invoke({"query": query})

        # Process the raw_response (see main.py for parsing)
        print(raw_response)
    ```

## 🛠️ Custom Tools

The project utilizes custom tools defined in `tools.py` to extend the agent's capabilities:

* **`search`:** Uses DuckDuckGo to search the web.
* **`wikipedia`:** Queries Wikipedia for information.
* **`save_text_to_file`:** Saves the research output to a text file.

## 🙏 Acknowledgements

-   The amazing developers of [Langchain](https://www.langchain.com/)
-   The Wikimedia Foundation for providing access to [Wikipedia](https://www.wikipedia.org/)
-   The contributors to [Langchain Community](https://github.com/langchain-ai/langchain/tree/master/libs/community)
-   The team at [Anthropic](https://www.anthropic.com/) for their powerful language models
-   The creators of [python-dotenv](https://pypi.org/project/python-dotenv/)
-   The maintainers of [Pydantic](https://pydantic.dev/)
-   The developers of [DuckDuckGo Search](https://duckduckgo.com/)
