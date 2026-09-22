# \# Intelli-Query

# 

# \*\*Conversational Business Intelligence for your CSV data.\*\*

# 

# Intelli-Query is an AI-powered Business Intelligence dashboard that lets you explore CSV datasets using \*\*plain English instead of writing SQL manually\*\*.

# 

# Upload a CSV, ask a question such as \*“Show total revenue by region”\* or \*“Who are the top 5 customers by spending?”\*, and Intelli-Query uses \*\*Google Gemini 2.5 Flash\*\* to understand your request, generate the appropriate SQL query, execute it against your data, and present the results as interactive charts, tables, and concise insights.

# 

# > \*\*Ask your data questions. Get SQL. See the answer.\*\*

# 

# !\[Intelli-Query Dashboard](https://i.imgur.com/placeholder.png)

# 

# \---

# 

# \## ✨ Features

# 

# \### 🤖 Natural Language → SQL

# 

# Ask questions about your data in everyday language. Gemini interprets your request and automatically generates the corresponding SQL query.

# 

# \### 📊 Interactive Data Visualizations

# 

# Automatically visualize query results using:

# 

# \* Bar charts

# \* Multi-series bar charts

# \* Line charts

# \* Pie charts

# \* Data tables

# 

# \### 📁 CSV Upload \& Schema Detection

# 

# Upload your own CSV files and Intelli-Query automatically analyzes the dataset structure, detects columns, and makes the data ready for querying.

# 

# \### 💬 Conversational Data Exploration

# 

# Continue asking questions within the same session and maintain a conversational history of your analysis.

# 

# \### 💡 AI-Powered Demo Queries

# 

# Don't know what to ask? Intelli-Query can generate example questions based on your dataset, with filters for:

# 

# \* Chart type

# \* Number of queries

# \* Different analytical use cases

# 

# \### 🔍 Transparent AI Analysis

# 

# Every result shows:

# 

# \* Your original question

# \* Generated SQL

# \* Query explanation

# \* Visualization

# \* Raw result data

# 

# This makes the AI's analysis easier to understand and verify.

# 

# \### 👀 CSV Data Preview

# 

# Inspect your uploaded or selected dataset directly from the dashboard before running queries.

# 

# \### ⚙️ Live API Key Configuration

# 

# Update your Gemini API key directly from the application without restarting the server.

# 

# \### 🚀 Lightweight Architecture

# 

# The backend uses Node.js's built-in HTTP server with \*\*zero npm runtime dependencies\*\*, keeping the project lightweight and easy to run.

# 

# \### 📴 Works Without an API Key

# 

# If no Gemini API key is configured, Intelli-Query can still run using built-in demo queries and local SQL execution.

# 

# \---

# 

# \## 🧠 How Intelli-Query Works

# 

# ```text

# CSV Dataset

# &#x20;    ↓

# Schema Detection

# &#x20;    ↓

# Natural Language Question

# &#x20;    ↓

# Google Gemini 2.5 Flash

# &#x20;    ↓

# Generated SQL Query

# &#x20;    ↓

# In-Process SQL Engine

# &#x20;    ↓

# Query Results

# &#x20;    ↓

# Chart + Table + Explanation

# ```

# 

# The result is a simple conversational workflow for exploring structured data without requiring users to manually write SQL queries.

# 

# \---

# 

# \## 🎯 Example Queries

# 

# Once a dataset is loaded, you can ask questions such as:

# 

# ```text

# Show total revenue by region

# ```

# 

# ```text

# What are the top 5 customers by spend?

# ```

# 

# ```text

# Show monthly sales trends

# ```

# 

# ```text

# Compare online and offline customers

# ```

# 

# ```text

# Which product category generated the highest revenue?

# ```

# 

# ```text

# Show the number of customers in each region

# ```

# 

# Intelli-Query converts these natural-language questions into SQL and presents the results in an appropriate visualization.

# 

# \---

# 

# \## 🖥️ Dashboard

# 

# The dashboard is organized around a simple workflow:

# 

# \*\*Dataset → Question → SQL → Visualization → Insight\*\*

# 

# You can select one of the included datasets or upload your own CSV, ask questions, inspect the generated SQL, and explore the returned data.

# 

# \---

# 

# \## 🛠️ Tech Stack

# 

# | Layer           | Technology                     |

# | --------------- | ------------------------------ |

# | Frontend        | Vanilla HTML, CSS \& JavaScript |

# | Backend         | Node.js                        |

# | Server          | Node.js `http`                 |

# | AI              | Google Gemini 2.5 Flash        |

# | AI Integration  | Gemini REST API                |

# | Visualization   | Chart.js                       |

# | Data Processing | In-process CSV / SQL engine    |

# | Data Format     | CSV                            |

# | Dependencies    | Zero runtime npm dependencies  |

# 

# \---

# 

# \## 📂 Project Structure

# 

# ```text

# intelli-query/

# ├── server.js

# ├── index.html

# ├── style.css

# ├── data/

# │   ├── sales\_demo.csv

# │   ├── customers\_demo.csv

# │   └── Customer Behaviour (Online vs Offline).csv

# ├── .env.example

# ├── .env

# └── package.json

# ```

# 

# \### Key Files

# 

# \* `server.js` — HTTP server, CSV processing, SQL execution and Gemini integration

# \* `index.html` — Dashboard interface

# \* `style.css` — UI styling and animations

# \* `data/` — Built-in sample datasets

# \* `.env.example` — Environment variable template

# \* `.env` — Local secrets and configuration

# 

# \---

# 

# \## 🚀 Quick Start

# 

# \### 1. Clone the repository

# 

# ```bash

# git clone https://github.com/YOUR\_USERNAME/YOUR\_REPO\_NAME.git

# cd YOUR\_REPO\_NAME

# ```

# 

# \### 2. Get a Gemini API Key

# 

# Create a free API key through Google AI Studio:

# 

# https://aistudio.google.com/app/apikey

# 

# Copy the generated key.

# 

# \### 3. Configure Environment Variables

# 

# Create your `.env` file:

# 

# ```bash

# cp .env.example .env

# ```

# 

# Then add your API key:

# 

# ```env

# GEMINI\_API\_KEY=AIzaSy...

# ```

# 

# > \*\*Note:\*\* The API key is optional. Without one, Intelli-Query falls back to built-in demo queries and local SQL execution.

# 

# \### 4. Start the application

# 

# ```bash

# npm start

# ```

# 

# Or:

# 

# ```bash

# node server.js

# ```

# 

# Then open:

# 

# ```text

# http://localhost:3000

# ```

# 

# \---

# 

# \## 📊 Using Intelli-Query

# 

# \### 1. Select a Dataset

# 

# Choose one of the included datasets or upload your own CSV file.

# 

# \### 2. Ask a Question

# 

# Enter a question about your data using natural language.

# 

# \### 3. Generate the Query

# 

# Intelli-Query sends the request to Gemini, which generates the SQL required to answer the question.

# 

# \### 4. Execute \& Analyze

# 

# The generated SQL runs against the loaded CSV data using the in-process query engine.

# 

# \### 5. Explore the Results

# 

# View the answer through:

# 

# \* Interactive visualization

# \* Raw data table

# \* Generated SQL

# \* Query explanation

# 

# You can then continue the conversation with another question.

# 

# \---

# 

# \## 🔐 Environment Variables

# 

# For local development:

# 

# ```env

# GEMINI\_API\_KEY=your\_gemini\_api\_key

# ```

# 

# For public deployment:

# 

# ```env

# GEMINI\_API\_KEY=your\_gemini\_api\_key

# JWT\_SECRET=your\_long\_random\_secret

# JWT\_EXPIRES\_IN=8h

# PORT=3000

# ```

# 

# \### Security Notes

# 

# \* Never commit `.env` to Git.

# \* Never expose your Gemini API key in frontend code.

# \* Use a strong random value for `JWT\_SECRET`.

# \* Do not commit real user information or sensitive datasets.

# \* Keep `data/users.json` out of version control if it contains real user data.

# 

# \---

# 

# \## 🌐 Deployment

# 

# \### Option A — Railway / Render

# 

# 1\. Import the GitHub repository.

# 2\. Configure the required environment variables.

# 3\. Set the build command:

# 

# ```bash

# npm install

# ```

# 

# 4\. Set the start command:

# 

# ```bash

# npm start

# ```

# 

# 5\. Deploy and use the generated HTTPS URL.

# 

# The server listens on `process.env.PORT`, with `3000` used as the local fallback.

# 

# \### Option B — Temporary Public Demo

# 

# For quick demonstrations while running locally:

# 

# ```bash

# cloudflared tunnel --url http://localhost:3000

# ```

# 

# or:

# 

# ```bash

# ngrok http 3000

# ```

# 

# \---

# 

# \## 💡 Why Intelli-Query?

# 

# Traditional BI tools can require users to understand SQL, database structures, or complex dashboard interfaces.

# 

# Intelli-Query provides a simpler interaction model:

# 

# ```text

# Instead of writing SQL:

# &#x20;       ↓

# "SELECT region, SUM(revenue)

# &#x20;FROM sales

# &#x20;GROUP BY region"

# 

# Simply ask:

# &#x20;       ↓

# "Show me total revenue by region."

# ```

# 

# The system handles the translation from natural language to SQL while still exposing the generated query for transparency.

# 

# \---

# 

# \## 🔮 Future Improvements

# 

# Potential extensions include:

# 

# \* Support for Excel and additional data formats

# \* More advanced SQL operations

# \* Automatic anomaly detection

# \* AI-generated business summaries

# \* Follow-up questions using previous query context

# \* Custom dashboard creation

# \* Exportable reports

# \* Additional visualization types

# \* Role-based access control

# \* Persistent datasets and user workspaces

# 

# \---

# 

# \## 📜 License

# 

# Add your preferred license here, such as MIT.

# 

# \---

# 

# \## 👨‍💻 Project

# 

# \*\*Intelli-Query\*\* — turning conversational questions into data-driven answers.

# 

# \*\*Natural Language → SQL → Visualization → Insight\*\*



