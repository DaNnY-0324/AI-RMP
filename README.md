# AI Rate My Professor Assistant

This project demonstrates how to build an AI-powered assistant that utilizes Retrieval-Augmented Generation (RAG) to provide accurate, context-aware responses about professors and courses. The assistant leverages Pinecone for vector storage and retrieval, and OpenAI's API for generating human-like responses.

## Table of Contents

- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Features

- **AI-Powered Responses**: Uses OpenAI's GPT-3.5 model to generate responses.
- **Vector Search**: Integrates Pinecone for efficient vector-based retrieval.
- **Seamless Integration**: Built using Next.js, React, and Material-UI for a modern and responsive UI.

## Setup

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS version recommended)
- [Python 3.6+](https://www.python.org/downloads/)
- Pinecone and OpenAI API keys

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/ai-rate-my-professor.git
   cd ai-rate-my-professor
   ```

2. **Set up the python environment:**

   ```python -m venv venv
      source venv/bin/activate  # On Windows: venv\Scripts\activate
      pip install -r requirements.txt
   ```

3. **Install Node.js dependencies:**

   ```npm install

   ```

4. **Create a .env.local file in the root directory with the following content:**

   ```PINECONE_API_KEY=your_pinecone_api_key
      OPENAI_API_KEY=your_openai_api_key
   ```

5. **Set up Pinecone and OpenAI:**

   ```Run the setup_rag.py script to initialize the Pinecone index and upload the review data:
      python setup_rag.py
   ```

6. **Run the development server:**

   ```npm run dev

   ```

## Usage

1. Open the application in your browser.
2. Interact with the AI assistant by typing questions about professors and courses.
3. The assistant will retrieve relevant information and generate responses based on the data stored in Pinecone and the capabilities of the OpenAI model.

## Project Structure

.
├── app/
│ ├── api/
│ │ └── chat/
│ │ └── route.js # API route for handling chat interactions
│ ├── page.tsx # Main page with the chat UI
├── public/
├── styles/
├── .env.local # Environment variables (not included in the repository)
├── setup_rag.py # Python script for setting up Pinecone and OpenAI
├── requirements.txt # Python dependencies
├── package.json # Node.js dependencies and scripts
├── README.md # Project documentation
└── .gitignore # Files to be ignored by Git

## Technologies Used:

### Frontend: Next.js, React, Material-UI

### Backend: Python, Pinecone, OpenAI API

### Database: Pinecone for vector storage and retrieval

### Environment Management: Python Virtual Environment (venv), dotenv

## Additional Notes:

- Replace the placeholder text (`your_pinecone_api_key`, `your_openai_api_key`, `your-username`) with the actual values relevant to your setup.
- If you have additional steps or custom configurations, you can include those in the `README.md` as well.
- Ensure that any sensitive information, like API keys, is excluded from the repository using the `.gitignore` file and stored securely in your `.env.local` file.
