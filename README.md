# MetalAgent: Metal Music Recommender System

## Overview

**MetalAgent** is a Kaggle notebook integrated with GitHub, designed to act as a personalized recommendation system for metal music enthusiasts. Using LangGraph and LangChain, MetalAgent provides curated recommendations, explores subgenres, and engages in interactive conversations about recent releases.

## Features

- **Kaggle Integration**: Uses Kaggle datasets for recent releases and subgenre lists.
- **Dynamic Recommendations**: Provides personalized metal music suggestions based on genres or subgenres.
- **Interactive Conversation**: Chatbot functionality for exploring metal genres and band histories.
- **Modular Design**: Built using LangGraph to manage conversation flow and LangChain to process natural language.

## How to Use

### 1. Open the Kaggle Notebook
- The MetalAgent notebook can be accessed on Kaggle. Clone or open it directly in Kaggle for execution.

### 2. Set Up API Keys
- The notebook requires a **Google API Key** from [AI Studio](https://aistudio.google.com/app/apikey) for LangChain integration. Add the key as a Kaggle secret named `GOOGLE_API_KEY`:
  - Go to **Kaggle** → **Account Settings** → **Secrets** → Add `GOOGLE_API_KEY` with your API key value.

### 3. Prepare the Dataset
- Upload the following files to the notebook's Kaggle environment:
  - **Recent Releases File**: `albums_Nov02-Nov08.txt` (or other similar files).
  - **Subgenres List**: `subgenres.txt`.

### 4. Install Required Libraries
Run the following command in a notebook cell:
```python
!pip install -qU 'langgraph==0.2.45' 'langchain-google-genai==2.0.4'
```

### 5. Execute the Notebook
- Follow the cells step by step to initialize the chatbot and begin using MetalAgent.

## Interactions

- **Start the Chat**: 
  - The chatbot will greet you with a welcome message and ask what genre of metal you’re interested in.
  - Example: *"What metal genre do you have in mind today?"*

- **Make Requests**:
  - Examples:
    - "Recommend recent black metal releases."
    - "What are the latest melodic death metal albums?"
    - "Show me the top doom metal albums this week."

- **Exit the Conversation**:
  - Type `q`, `quit`, or `exit` to end the chat.

## Integration with GitHub

The notebook can be pushed to your GitHub repository for version control and collaboration. 

### Steps:
1. **Save Your Notebook**:
   - After editing, save the notebook on Kaggle.
2. **Export to GitHub**:
   - Use Kaggle's **"Link to GitHub"** option.
   - Save the Kaggle notebook.
   - Select your repository and branch for the upload.

## Folder Structure in Kaggle

```
/kaggle/input/
├── week-of-november-08-2024/      # Dataset folder for recent releases
│   └── albums_Nov02-Nov08.txt
├── metal-subgenres/               # Subgenre list folder
│   └── subgenres.txt
MetalAgent.ipynb                   # Notebook file
```

## Contribution

1. Fork the repository on GitHub.
2. Make your changes and submit a pull request.
3. Contributions related to additional subgenre tools, better recommendation algorithms, or live database integration are welcome.

## License

This project is licensed under the MIT License.

## Credits

MetalAgent is built using:
- **LangGraph** for conversation management.
- **LangChain Google GenAI** for natural language processing.
- **Kaggle Datasets** for recent releases and subgenres.

Feedback and contributions are encouraged! 🤘
