
# Conversational RAG Chatbot

This project implements a Conversational Retrieval-Augmented Generation (RAG) chatbot using Langchain, Groq API, Google Generative AI embeddings, and ChromaDB. The chatbot is built to answer domain-specific queries based on provided documents.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/username/repository-name.git
    ```

2. Navigate to the project directory:
    ```bash
    cd repository-name
    ```

3. Create and activate a virtual environment (optional but recommended):
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

4. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

5. Set up environment variables for the API keys. You can use a `.env` file or manually set them:
    ```bash
    export GROQ_API_KEY=your_groq_api_key
    export LANGCHAIN_API_KEY=your_langchain_api_key
    ```

## Usage

1. Run the notebook to initialize the model and create the knowledge base from your document.
2. Launch the chatbot interface using the Gradio app to interact with the system.

### Example:

```bash
gr.ChatInterface.launch(share=True)
```

Once launched, you can ask questions like:

- What is Machine Learning?
- What is Data Mining?
- List applications of Machine Learning Algorithms.

The Gradio interface will display the chatbot and respond with answers based on the document content.

## Features

- **Conversational RAG Chatbot**: Responds to queries using a RAG model that retrieves relevant information and generates answers.
- **ChromaDB for Document Storage**: Stores embeddings for efficient retrieval.
- **Google Generative AI Embeddings**: Utilizes embeddings from Google Generative AI for better language understanding.
- **Gradio Interface**: A user-friendly interface to interact with the chatbot.

## Project Structure

```
repository-name/
│
├── data/               # Directory to store input documents
├── src/                # Source code for chatbot
│   ├── chatbot.py      # Chatbot logic
│   └── utils.py        # Utility functions
├── notebooks/          # Jupyter notebooks
│   └── Coversational_RAG_chatbot_langchain.ipynb  # Main notebook
├── requirements.txt    # Required Python packages
└── README.md           # Project documentation
```

## Contributing

1. Fork the project.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Submit a pull request.

## License

This project is licensed under the MIT License.

## Acknowledgements

- [Langchain](https://github.com/hwchase17/langchain)
- [Groq](https://groq.com/)
- [Gradio](https://gradio.app/)
- [ChromaDB](https://docs.trychroma.com/)
