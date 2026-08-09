<<<<<<< HEAD
=======
# 🛍️ Shopping Behaviour Analysis

<p align="center">
  <b>End-to-End Customer Analytics using Python, PostgreSQL & Power BI</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/PostgreSQL-SQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Power_BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter">
</p>

---

##  Overview

**Shopping Behaviour Analysis** is an end-to-end data analytics project focused on understanding customer purchasing behaviour from retail transaction data.

The project follows a complete analytics workflow:

**Data Cleaning → Exploratory Analysis → Feature Engineering → SQL Analysis → KPI Development → Power BI Visualization → Business Insights**

Python is used for data preparation and exploratory analysis, PostgreSQL is used for structured SQL-based analysis, and Power BI transforms the results into an interactive business dashboard.

The goal is not only to analyse the data, but to translate customer transactions into **meaningful business insights that can support marketing, sales, customer retention, and decision-making.**

---

## 🎯 Business Questions

This project investigates questions such as:

* Which product categories generate the highest sales?
* Which products are purchased most frequently?
* Which customer segments contribute the most to revenue?
* How does purchasing behaviour vary across age groups and genders?
* Which locations generate the highest sales?
* How does subscription status affect customer purchasing behaviour?
* What is the relationship between discounts and purchase behaviour?
* How frequently do customers make purchases?
* Which payment methods are most popular?
* Which seasons show stronger purchasing activity?
* How do customer ratings vary across products and categories?
* Can previous purchasing behaviour help identify high-value customers?

These questions form the foundation of the Python analysis, PostgreSQL queries, and Power BI dashboard.

---

# 🧰 Tech Stack

| Technology              | Role in the Project                         |
| ----------------------- | ------------------------------------------- |
| 🐍 **Python**           | Data cleaning, preprocessing and analysis   |
| 🐼 **Pandas**           | Data manipulation and transformation        |
| 🔢 **NumPy**            | Numerical operations                        |
| 📓 **Jupyter Notebook** | Interactive data analysis                   |
| 🐘 **PostgreSQL**       | SQL querying and business analysis          |
| 📈 **Power BI**         | Interactive dashboard and KPI visualization |
| 🔧 **Git & GitHub**     | Version control and project documentation   |

---

# 🔄 End-to-End Workflow

```text
                    ┌──────────────────┐
                    │   Raw Dataset    │
                    └────────┬─────────┘
                             │
                             ▼
                  ┌─────────────────────┐
                  │ Data Cleaning        │
                  │ & Preprocessing      │
                  └──────────┬──────────┘
                             │
                             ▼
                  ┌─────────────────────┐
                  │ Exploratory Data     │
                  │ Analysis             │
                  └──────────┬──────────┘
                             │
                             ▼
                  ┌─────────────────────┐
                  │ Feature Engineering │
                  └──────────┬──────────┘
                             │
                             ▼
                  ┌─────────────────────┐
                  │ PostgreSQL           │
                  │ SQL Analysis         │
                  └──────────┬──────────┘
                             │
                             ▼
                  ┌─────────────────────┐
                  │ KPIs & Business      │
                  │ Metrics              │
                  └──────────┬──────────┘
                             │
                             ▼
                  ┌─────────────────────┐
                  │ Power BI Dashboard   │
                  └──────────┬──────────┘
                             │
                             ▼
                  ┌─────────────────────┐
                  │ Business Insights    │
                  │ & Recommendations    │
                  └─────────────────────┘
```

---

# 📂 Repository Structure

```text
shopping-behaviour-analysis/
│
├── 📁 assets/
│   └── powerbi-dashboard.png
│
├── 📁 code/
│   └── Customer_shopping.ipynb
│
├── 📁 raw_data/
│   └── customer_shopping_behavior.csv
│
│
├── 📄 requirements.txt
├── 📄 README.md
└── 📄 LICENSE
```

### Directory Description

**`code/`**
Contains the main Jupyter Notebook with the complete Python-based analysis.

**`raw_data/`**
Contains the original dataset used as the input for the project.


**`assets/`**
Contains visual assets used in the documentation, including the Power BI dashboard screenshot.

**`requirements.txt`**
Contains the Python dependencies required to reproduce the analysis.

---

# 📊 Dataset

The dataset contains customer-level shopping transactions covering demographic information, purchasing behaviour, product information, discounts, subscriptions, shipping, payment methods, and purchase frequency.

### Dataset Location

```text
raw_data/customer_shopping_behavior.csv
```

### Dataset Information

| Feature                  | Description                            |
| ------------------------ | -------------------------------------- |
| `Customer ID`            | Unique customer identifier             |
| `Age`                    | Customer age                           |
| `Gender`                 | Customer gender                        |
| `Item Purchased`         | Name of purchased product              |
| `Category`               | Product category                       |
| `Purchase Amount (USD)`  | Transaction purchase amount            |
| `Location`               | Customer location                      |
| `Size`                   | Product size                           |
| `Color`                  | Product colour                         |
| `Season`                 | Season associated with the transaction |
| `Review Rating`          | Customer rating                        |
| `Subscription Status`    | Customer subscription status           |
| `Shipping Type`          | Selected shipping method               |
| `Discount Applied`       | Whether a discount was applied         |
| `Promo Code Used`        | Whether a promotional code was used    |
| `Previous Purchases`     | Number of previous purchases           |
| `Payment Method`         | Payment method used                    |
| `Frequency of Purchases` | Customer purchasing frequency          |

---

# 🧹 Data Preparation

Before performing analysis, the dataset is inspected and prepared for downstream processing.

### Data preparation includes:

* Loading the dataset with Pandas
* Inspecting rows, columns and data types
* Identifying missing values
* Checking duplicate records
* Validating numerical columns
* Checking categorical consistency
* Standardizing data where required
* Validating purchase amounts and ratings
* Performing descriptive statistical analysis
* Preparing the cleaned dataset for SQL and Power BI

The resulting dataset provides a consistent foundation for further analysis.

---

# 🔎 Exploratory Data Analysis

The exploratory analysis focuses on understanding different dimensions of customer behaviour.

## 👥 Customer Behaviour

Analysis includes:

* Customer age distribution
* Gender-wise purchasing behaviour
* Purchase frequency
* Previous purchase behaviour
* Subscription status
* Customer spending patterns

## 🛍️ Product Performance

Analysis includes:

* Most frequently purchased products
* Product category performance
* Average purchase amount
* Product ratings
* Size preferences
* Colour preferences

## 💰 Sales Analysis

Analysis includes:

* Revenue by category
* Revenue by location
* Seasonal sales patterns
* Average transaction value
* Discount usage
* Promotional code usage

## 💳 Transaction Behaviour

Analysis includes:

* Payment method preferences
* Shipping method preferences
* Subscription behaviour
* Discount vs non-discount purchases
* Purchase frequency patterns

---

# 🐘 PostgreSQL Analysis

After data preparation, the cleaned dataset is analysed using **PostgreSQL**.

SQL is used to transform raw transaction data into business-oriented metrics and aggregations.

### Key SQL analysis areas

* Total and average purchase amounts
* Category-level performance
* Product-level rankings
* Customer segmentation
* Location-based analysis
* Subscription comparisons
* Discount analysis
* Promotional campaign analysis
* Payment method distribution
* Purchase frequency analysis

PostgreSQL provides a structured analytical layer between the cleaned dataset and the final visualization stage.

---

# 📈 Power BI Dashboard

The final analytical layer is an interactive **Power BI dashboard** designed to communicate the most important findings clearly.

## Dashboard Preview

<img width="765" height="440" alt="Dashboard" src="https://github.com/user-attachments/assets/bd465ca9-684d-4548-b63b-cc329b812075" />

### Dashboard Components

The dashboard focuses on key business metrics and customer behaviour, including:

* 💰 **Revenue & Purchase KPIs**
* 🛒 **Purchase Volume**
* 👥 **Customer Demographics**
* 📦 **Product & Category Performance**
* 📍 **Location-wise Analysis**
* 🔄 **Subscription Behaviour**
* 🎟️ **Discount & Promo Analysis**
* ⭐ **Customer Ratings**
* 📅 **Seasonal Trends**
* 💳 **Payment Method Analysis**
* 🚚 **Shipping Preferences**

The dashboard is designed to allow stakeholders to quickly identify trends, compare customer segments, and understand purchasing behaviour.

---


### 3. Commit and push the image

```bash
git add assets/powerbi-dashboard.png
git commit -m "Add Power BI dashboard preview"
git push
```

GitHub will automatically render the image inside this README.

---

# 💡 Business Insights

The analysis can be used to identify patterns and opportunities across several business dimensions.

### Customer Insights

Understand which customer groups demonstrate higher purchase frequency, spending, or engagement.

### Product Insights

Identify high-performing products and categories that contribute significantly to overall sales.

### Marketing Insights

Evaluate the relationship between discounts, promotional codes, subscriptions, and customer purchasing behaviour.

### Geographic Insights

Compare customer purchasing activity across different locations.

### Seasonal Insights

Identify changes in purchasing behaviour across different seasons.

### Customer Retention

Use previous purchase behaviour and subscription information to understand customer engagement and identify potentially valuable customer segments.

---

# 📤 Data Export

After cleaning and transformation, the processed dataset can be exported for use in PostgreSQL or Power BI.

Example:

```python
cleaned_df.to_csv(
    "outputs/data/cleaned_customer_shopping.csv",
    index=False
)
```

This creates:

```text
outputs/data/cleaned_customer_shopping.csv
```

The resulting file can then be loaded into PostgreSQL or imported into Power BI.

---

# 🚀 Getting Started

## Prerequisites

Install the following before running the project:

* Python 3.8+
* Git
* Jupyter Notebook / JupyterLab
* PostgreSQL
* Power BI Desktop *(for dashboard development)*

---

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/rehan909100/shopping-behaviour-analysis.git
```

```bash
cd shopping-behaviour-analysis
```

---

## 2️⃣ Create a Virtual Environment

### Windows

```bash
python -m venv .venv
```

Activate it:

```bash
.venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv .venv
```

Activate it:

```bash
source .venv/bin/activate
```

---

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

If `requirements.txt` has not been created yet:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

Then generate the dependency file:

```bash
pip freeze > requirements.txt
```

---

## 4️⃣ Launch Jupyter

Run:

```bash
jupyter notebook
```

or:

```bash
jupyter lab
```

Open:

```text
code/Customer_shopping.ipynb
```

Run the notebook cells sequentially.

---

# 🔁 Reproducibility

The project can be reproduced using the following workflow:

```text
Clone Repository
      ↓
Create Virtual Environment
      ↓
Install Dependencies
      ↓
Load Raw Dataset
      ↓
Run Jupyter Notebook
      ↓
Generate Cleaned Dataset
      ↓
Load Data into PostgreSQL
      ↓
Run SQL Analysis
      ↓
Connect Data to Power BI
      ↓
Build / Refresh Dashboard
```

The project uses repository-relative paths wherever possible to avoid machine-specific file paths.

---

# 🧪 Data Validation

The analysis incorporates basic validation checks to improve data reliability.

These include:

* Row and column count verification
* Missing-value inspection
* Duplicate detection
* Data-type validation
* Numerical range checks
* Categorical value consistency
* Purchase amount validation
* Review rating validation
* Before-and-after cleaning comparisons

---

# 📦 Python Requirements

Core dependencies:

```text
pandas
numpy
jupyter
```

Generate the complete environment specification with:

```bash
pip freeze > requirements.txt
```

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

### Development workflow

```bash
git checkout -b feature/your-feature
```

Make your changes and commit them:

```bash
git add .
git commit -m "Describe your changes"
```

Push the branch:

```bash
git push origin feature/your-feature
```

Then open a Pull Request.

---


# 👨‍💻 Author

## Md Rehan Umair

**B.Tech —**
**National Institute of Technology, Tiruchirappalli**

Interested in **Data Analytics, Software Development, Machine Learning, and Data-Driven Problem Solving.**

### 🔗 GitHub

[@rehan909100](https://github.com/rehan909100)

---

# ⭐ Support

If you found this project useful or interesting, consider giving the repository a ⭐ on GitHub.

**Thanks for visiting!**
