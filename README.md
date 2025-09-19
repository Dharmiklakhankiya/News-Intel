# News Research Tool 📰✨

A smart News Research Tool that uses GenAI, LangChain, HuggingFace, and LLMs to analyze news articles. Just enter URLs, ask questions, and get instant, source-backed answers—all in a simple Streamlit interface.

## 🚀 Features

-   **Multi-URL Processing**: Input up to 3 news article URLs for analysis.
-   **AI-Powered Q&A**: Ask questions in natural language about the content of the provided articles.
-   **Source-Backed Answers**: Every answer is accompanied by the source URL from which the information was extracted.
-   **Simple Web Interface**: Easy-to-use interface built with Streamlit.
-   **Efficient Data Handling**: Uses FAISS for efficient similarity search and vector storage.

## 🛠️ Tech Stack

-   **Frontend**: [Streamlit](https://streamlit.io/)
-   **LLM Orchestration**: [LangChain](https://www.langchain.com/)
-   **LLM & Embeddings**: [Hugging Face](https://huggingface.co/) (Mistral, Sentence Transformers)
-   **Vector Store**: [FAISS](https://github.com/facebookresearch/faiss) (Facebook AI Similarity Search)
-   **Programming Language**: Python

## 📋 Getting Started

Follow these instructions to set up and run the project on your local machine.

### Prerequisites

-   Python 3.8+
-   A Hugging Face API Token. You can get one [here](https://huggingface.co/settings/tokens).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/News-Research-Tool-main.git
    cd News-Research-Tool-main
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    venv\Scripts\activate  # On Windows
    # source venv/bin/activate  # On macOS/Linux
    ```

3.  **Install the required dependencies:**
    Create a `requirements.txt` file with the following content:
    ````text
    // filepath: c:\Users\User\Desktop\News-Research-Tool-main\requirements.txt
    streamlit
    langchain
    langchain-huggingface
    python-dotenv
    unstructured
    libmagic
    python-magic-win64
    sentence-transformers
    faiss-cpu
    tiktoken
    ````
    Then run:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up environment variables:**
    Create a file named `.env` in the root directory of the project and add your Hugging Face API token:
    ```env
    # filepath: c:\Users\User\Desktop\News-Research-Tool-main\.env
   "
    ```

### Usage

1.  **Run the Streamlit application:**
    Open your terminal in the project's root directory and run:
    ```bash
    streamlit run main.py
    ```

2.  **Use the application:**
    -   Your web browser will open with the application running.
    -   Enter the URLs of the news articles you want to research in the sidebar.
    -   Click the "Process URLs" button.
    -   Wait for the tool to load the data, split the text, and create embeddings. You will see status updates on the screen.
    -   Once processing is complete, an input box will appear. Type your question about the articles and press Enter.
    -   The tool will display the answer along with the sources it used.

## 📂 Project Structure

```
News-Research-Tool-main/
├── .env                # Environment variables (Hugging Face API token)
├── main.py             # Main Streamlit application script
├── requirements.txt    # Python dependencies
├── vector_index.pkl    # Generated file to store the vector index
└── README.md           # This file
```

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.