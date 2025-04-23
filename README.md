Setup Instructions
Clone the repository

Create and activate a virtual environment:

python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate    # Windows
Install dependencies:

pip install -r requirements.txt
Run the notebooks in order:

First run Nugget.ipynb to collect restaurant data

Then run ragBot.ipynb to query the restaurant information

Usage
Data Collection (Nugget.ipynb)
Scrapes restaurant data from Zomato URLs
Processes and structures the data into a knowledge base
Outputs a CSV file (Restaurants.csv) and JSON knowledge base

Chatbot (ragBot.ipynb)
Loads restaurant data from a PDF (you'll need to convert the CSV to PDF)

Answers natural language questions about:

Restaurant cuisines
Opening hours
Price ranges
Locations

Example Queries
"Which restaurants serve Biryani in Roorkee?"
"What's the price range at Tamarind Restaurant?"
"Which restaurants are open today?"
"Where can I find Italian food in Roorkee?"
