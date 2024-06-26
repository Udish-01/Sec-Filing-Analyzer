
# SEC Filings Analyzer

SEC Filings Analyzer is a full-stack application designed to visualize and analyze financial data extracted from SEC filings. It offers interactive functionalities for visualizing key financial metrics over time, retrieving filing dates, and extracting summarized insights with sentiment analysis.

## Tech Stack

### Backend

- **Flask**: A lightweight WSGI web application framework. It is chosen for its simplicity and flexibility in building web APIs. Flask is easy to set up and is suitable for projects where a straightforward approach to handling HTTP requests is preferred.
- **Flask-CORS**: A Flask extension required to handle Cross-Origin Resource Sharing (CORS), allowing the frontend hosted on a different domain to interact with the backend.
- **Plotly**: Used for creating interactive graphs that can be easily converted to JSON format for web rendering. Plotly's comprehensive graphing library allows for sophisticated visualizations.
- **Pandas**: Utilized for data manipulation and analysis. It is particularly effective in handling tabular data.
- **Requests**: This library is instrumental for performing HTTP requests to external APIs and handling the responses, which is crucial for fetching SEC filing data.
- **Transformers and NLTK**: These libraries are used for natural language processing, which is necessary for analyzing and summarizing the textual content of SEC filings.

### Frontend

- **React**: A JavaScript library for building user interfaces, chosen for its efficiency and reusability of components. React's state management makes it ideal for handling the dynamic aspects such as user inputs and visual data rendering.
- **Axios**: A promise-based HTTP client for the browser and node.js. Axios is used for making HTTP requests from the frontend to the backend. It is preferred over the native Fetch API due to its wide browser support and ease of handling responses.
- **React-Plotly.js**: A plotly.js wrapper that makes it easy to create interactive plots using Plotly with React. This is used for rendering the financial graphs based on SEC data.
- **CSS**: For styling the frontend components. The simplicity of CSS is leveraged to keep the user interface clean and responsive without overcomplicating the design.

## Features

- **Interactive Visualizations**: Generate and view interactive graphs of financial metrics such as assets and earnings per share.
- **Filing Dates Retrieval**: Access a list of filing dates for selected companies.
- **Insights Extraction**: Analyze and summarize textual content from SEC filings, highlighting the sentiment and key points.

## Setup and Installation

1. Clone the repository:
	 ```bash
   git clone https://github.com/Udish-01/sec-filings-analyser.git
   cd sec-filings-analyzer
   ``` 

2.  Set up the backend:
	   ```bash
	cd backend
    pip install -r requirements.txt
    python app.py
    ``` 
    
3.  Set up the frontend:
    
	   ```bash
	cd frontend
    npm install
    npm start
    ```    
4.  Open the browser to `http://localhost:5173` to use the application.