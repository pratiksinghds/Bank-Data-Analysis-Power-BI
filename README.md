## 📊 Banking Data Analysis Project

This project demonstrates a complete data analysis pipeline using banking data—from raw Excel files to a fully interactive Power BI dashboard. It covers data preparation, transformation, visualization, and dashboard design across multiple tools and technologies.

---

### 🧾 Project Workflow

#### 1. 📥 Data Collection
- Source: Raw banking data in `.xlsx` format
- Contains customer demographics, account types, loan details, and transaction history

#### 2. 📄 Data Conversion
- Open Excel file in Microsoft Excel or Pandas
- Save as `.csv` for compatibility with MySQL and Python tools

#### 3. 🛢️ Load Data into MySQL
- Use MySQL Workbench or command line:
  - Create database: `banking_case`
  - Create tables and import CSV using `LOAD DATA INFILE` or Workbench import wizard
- Verify schema and data integrity using SQL queries

#### 4. 🐍 Data Transformation with Pandas
- Load MySQL data into Jupyter Notebook using `mysql.connector` or `SQLAlchemy`
- Clean and transform:
  - Handle missing values
  - Normalize column formats
  - Create derived columns (e.g., age bands, loan categories)
- Save cleaned datasets for visualization

#### 5. 📈 Visualization with Matplotlib & Seaborn
- Generate exploratory plots:
  - Bar charts for loan distribution
  - Pie charts for account types
  - Histograms for credit card balances
  - Heatmaps for correlation analysis
- Use `matplotlib.pyplot` and `seaborn` for styling and layout

#### 6. 📊 Dashboard Creation in Power BI
- Connect Power BI to MySQL using MySQL Connector/NET
- Create DAX measures:
  - `Total Loan = SUM(Bank Loans + Business Lending + Credit Card Balance)`
  - `Total Deposit = SUM(Bank Deposits + Savings + Checking + Foreign Currency)`
- Design 4 interactive dashboard pages:
  1. **Home** – Overview of key metrics
  2. **Loan Analysis** – Breakdown by occupation, income, nationality
  3. **Deposit Analysis** – Account types and deposit trends
  4. **Ask a Question** – Natural language Q&A powered by Power BI insights

---

### 🛠️ Tools & Technologies

| Tool            | Purpose                          |
|-----------------|----------------------------------|
| Excel / CSV     | Raw data input                   |
| MySQL           | Data storage and querying        |
| Python (Pandas) | Data cleaning and transformation |
| Jupyter Notebook| Interactive scripting            |
| Matplotlib      | Static visualizations            |
| Seaborn         | Statistical plots                |
| Power BI        | Dashboard and reporting          |

---

### 📁 Folder Structure

```
├── data/
│   ├── raw_excel/
│   └── cleaned_csv/
├── sql/
│   └── schema_and_import.sql
├── notebooks/
│   └── analysis.ipynb
├── dashboard/
│   └── powerbi.pbix
├── README.md
```
