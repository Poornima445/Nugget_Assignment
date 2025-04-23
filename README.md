# Restaurant Chatbot with RAG and Zomato Scraper

A comprehensive system for collecting restaurant data from Zomato and answering natural language queries about restaurants using a Retrieval-Augmented Generation (RAG) approach.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Example Queries](#example-queries)
- [File Structure](#file-structure)
- [Troubleshooting](#troubleshooting)
- [License](#license)

## Features

- **Web Scraper**: Collects restaurant data from Zomato, including:
  - Basic information (name, contact details)
  - Location data
  - Cuisine types
  - Opening hours
  - Price ranges

- **Knowledge Base Builder**: Processes and structures scraped data into:
  - CSV format for easy analysis
  - JSON knowledge base for efficient querying

- **Chatbot Interface**: Answers natural language questions about restaurants using:
  - Vector similarity search
  - GPT-2 language model
  - Context-aware responses

## Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager
- Jupyter Notebook

### Setup Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/restaurant-chatbot.git
   cd restaurant-chatbot
   ```

2. **Create and activate a virtual environment**
   - Linux/Mac:
     ```bash
     python -m venv venv
     source venv/bin/activate
     ```
   - Windows:
     ```cmd
     python -m venv venv
     venv\Scripts\activate
     ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Install Jupyter Notebook (if not already installed)**
   ```bash
   pip install notebook
   ```

## Usage

### Data Collection Phase

1. Run the `Nugget.ipynb` notebook:
   ```bash
   jupyter notebook Nugget.ipynb
   ```
   - Scrapes restaurant data from predefined Zomato URLs
   - Saves the data to `Restaurants.csv`
   - Builds a structured knowledge base (`data.json`)

2. **Convert CSV to PDF**:
   - Use any CSV to PDF converter (LibreOffice, online tools, etc.)
   - Save the PDF as `respdfdata.pdf` in the project root

### Chatbot Phase

1. Run the `ragBot.ipynb` notebook:
   ```bash
   jupyter notebook ragBot.ipynb
   ```
   - The chatbot will load the knowledge base and respond to queries

## Example Queries

Try asking:

```python
"Which restaurants serve Biryani in Roorkee?"
"What's the price range at Tamarind Restaurant?"
"Which restaurants are open today?"
"Where can I find Italian food in Roorkee?"
"Show me vegetarian restaurants near Civil Lines"
"What's the phone number for Olive Multicuisine Restaurant?"
```

