# 🛍️ Customer Feedback Analysis & AI-Powered Response Generator

## 📌 Project Overview

This project analyzes customer reviews using Python and Pandas to identify critical feedback, explore common complaints, and understand customer satisfaction patterns. It also uses Generative AI to generate personalized and empathetic customer support apology emails for negative reviews.

## 🎯 Project Objectives

* 🧹 Clean and preprocess customer review data.
* ⭐ Identify high-rating and critical reviews using rule-based filtering.
* 🔎 Analyze common complaint keywords and their frequency.
* 📊 Explore customer feedback patterns across different products.
* 🤖 Generate personalized apology emails using Generative AI.

## 🛠️ Technologies Used

| Technology                    | Purpose                              |
| ----------------------------- | ------------------------------------ |
| 🐍 Python                     | Data processing and analysis         |
| 🐼 Pandas                     | Data cleaning and manipulation       |
| 🔤 Regular Expressions (`re`) | Text cleaning                        |
| 🔢 `collections.Counter`      | Complaint keyword frequency analysis |
| ✨ Google Gemini API           | AI-generated customer support emails |
| 📓 Jupyter Notebook           | Implementation and documentation     |

## ⚙️ Project Workflow

### 1. 🧹 Data Wrangling

* Load and inspect the customer feedback dataset.
* Identify and handle missing values.
* Clean review text by standardizing case and removing special characters.
* Prepare the data for analysis.

### 2. 📊 Rule-Based Filtering & Insights

* Identify high-rating reviews with ratings of 4 or 5.
* Identify critical reviews with ratings of 1 or 2.
* Analyze review counts across different products.
* Count predefined complaint-related keywords to identify common customer issues.

### 3. 🤖 AI-Powered Customer Outreach

* Select three detailed negative reviews from the critical feedback.
* Send review text to the Google Gemini API.
* Generate short, personalized, and empathetic apology emails that address the specific complaints.

## 📂 Dataset

The project uses a sample retail customer feedback dataset with the following columns:

| Column          | Description                        |
| --------------- | ---------------------------------- |
| `Review_ID`     | Unique review identifier           |
| `Product`       | Product associated with the review |
| `Rating`        | Customer rating from 1 to 5        |
| `Review_Text`   | Original customer feedback         |
| `Customer_Name` | Customer name                      |
| `Review_Date`   | Date of the review                 |

The dataset includes positive, neutral, and negative reviews, along with missing values to demonstrate data-cleaning techniques.

## 🚀 Installation & Setup

### Prerequisites

* Python 3.x
* Jupyter Notebook
* A Google Gemini API key for the AI-powered section

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd customer-feedback-analysis
```

### 2. Install Dependencies

```bash
pip install pandas google-genai
```

### 3. Run the Notebook

1. Place the dataset CSV file in the project directory.
2. Open `customer_feedback_analysis.ipynb` in Jupyter Notebook.
3. Run the cells sequentially to follow the analysis workflow.

### 🔑 Configure the Gemini API Key

Obtain an API key through [Google AI Studio](https://aistudio.google.com/). Store it securely as an environment variable named `GEMINI_API_KEY`.

Example Python code to access the key:

```python
import os

api_key = os.getenv("GEMINI_API_KEY")

if not api_key:
    raise ValueError("Please configure your GEMINI_API_KEY.")
```

⚠️ **Security Note:** Never hardcode your API key in your notebook or commit it to GitHub.

## 📈 Key Learning Outcomes

* Data cleaning and preprocessing using Pandas
* Rule-based filtering and exploratory data analysis
* Text processing with regular expressions
* Keyword frequency analysis using `Counter`
* Integration of a Generative AI API
* Automated drafting of customer support emails

## ⚠️ Limitations

* Complaint detection depends on a predefined keyword list and may miss synonyms or complaints expressed in different words.
* AI-generated emails should be reviewed before being sent to customers.
* The sample dataset is intended for demonstrating the project workflow and may not represent real-world customer feedback at scale.

## 🏁 Conclusion

This project demonstrates how Python-based data analysis and Generative AI can work together to simplify customer feedback management. By identifying critical reviews and generating personalized support responses, the solution provides a practical example of combining data analytics with AI-powered automation.

---

⭐ If you find this project useful, feel free to explore the code and adapt it for your own customer feedback analysis projects.

👨‍💻 Author
Anish Parulekar

Data Analytics & Data Science Learner
