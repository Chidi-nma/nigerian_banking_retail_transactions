# Nigerian Retail Transactions - Exploratory Data Analysis

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📋 Table of Contents

- [Overview](#overview)
- [Dataset Description](#dataset-description)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Key Features](#key-features)
- [Analysis & Insights](#analysis--insights)
- [Visualizations](#visualizations)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🎯 Overview

This project performs comprehensive **Exploratory Data Analysis (EDA)** on Nigerian retail and Point of Sale (POS) transaction data. The analysis aims to uncover patterns in consumer spending behavior, identify popular merchants and channels, analyze geographic transaction distribution, and detect potential fraud indicators across Nigeria's financial ecosystem.

### Objectives

- 📊 Analyze transaction patterns and trends across different channels (POS, ATM, Mobile)
- 💰 Understand spending behaviors and transaction amount distributions
- 🗺️ Identify geographic hotspots and regional transaction patterns
- 🏪 Discover top merchants and popular merchant categories
- ⏰ Examine temporal patterns in transaction activities
- 🔍 Investigate fraud indicators and transaction security metrics

## 📊 Dataset Description

### Source

The dataset contains Nigerian retail transaction records from various merchants across different states in Nigeria.

### Features

| Column Name              | Description                                 | Data Type |
| ------------------------ | ------------------------------------------- | --------- |
| `transaction_id`         | Unique identifier for each transaction      | String    |
| `account_id`             | Account identifier                          | String    |
| `customer_id`            | Customer identifier                         | String    |
| `timestamp`              | Date and time of transaction                | Datetime  |
| `amount_ngn`             | Transaction amount in Nigerian Naira        | Float     |
| `balance_before_ngn`     | Account balance before transaction          | Float     |
| `balance_after_ngn`      | Account balance after transaction           | Float     |
| `transaction_type`       | Type of transaction (credit/debit)          | String    |
| `channel`                | Transaction channel (POS/ATM/Mobile)        | String    |
| `merchant_category_code` | MCC code for merchant category              | String    |
| `merchant_name`          | Name of merchant                            | String    |
| `location_lga`           | Local Government Area                       | String    |
| `location_state`         | Nigerian state where transaction occurred   | String    |
| `device_id`              | Device identifier (for mobile transactions) | String    |
| `status`                 | Transaction status                          | String    |
| `fraud_flag`             | Boolean flag indicating potential fraud     | Boolean   |

### Dataset Statistics

- **Size**: Full sample of Nigerian retail transactions
- **Format**: CSV (Comma-Separated Values)
- **File Size**: ~18.9 KB
- **Geographic Coverage**: Multiple states across Nigeria

## 📁 Project Structure

```
EDA_nigerian_banking_retail_transactions/
│
├── README.md                                      # Project documentation
├── pos_eda.ipynb                                  # Main Jupyter notebook with EDA
├── nigerian_retail_transactions_full_sample.csv   # Dataset file
│
└── .git/                                          # Git version control
```

## 🚀 Installation

### Prerequisites

- Python 3.9 or higher
- pip package manager
- Jupyter Notebook or JupyterLab

### Setup Instructions

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd EDA_nigerian_banking_retail_transactions
   ```

2. **Create a virtual environment (recommended)**

   ```bash
   python -m venv venv

   # Activate virtual environment
   # On macOS/Linux:
   source venv/bin/activate

   # On Windows:
   venv\Scripts\activate
   ```

3. **Install required packages**

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

   Or create a `requirements.txt` file:

   ```txt
   pandas>=2.0.0
   numpy>=1.24.0
   matplotlib>=3.7.0
   seaborn>=0.12.0
   jupyter>=1.0.0
   ```

   Then install:

   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook**

   ```bash
   jupyter notebook
   ```

5. **Open the notebook**
   - Navigate to `pos_eda.ipynb` in the Jupyter interface
   - Run cells sequentially to reproduce the analysis

## 💻 Usage

### Running the Analysis

1. Ensure all dependencies are installed
2. Place the dataset file (`nigerian_retail_transactions_full_sample.csv`) in the project directory
3. Open `pos_eda.ipynb` in Jupyter Notebook
4. Execute cells in order:
   - Cell 1: Import libraries
   - Cell 2: Load and explore data
   - Cell 3+: Perform various analyses and generate visualizations

### Customizing the Analysis

You can modify the notebook to:

- Filter data by specific date ranges
- Focus on particular states or merchants
- Add additional visualizations
- Perform deeper statistical analysis
- Export results to different formats

## 🔑 Key Features

### Data Processing

- ✅ Automated data loading and validation
- ✅ Missing value detection and handling
- ✅ Timestamp parsing and temporal feature extraction
- ✅ Data type conversions and standardization

### Statistical Analysis

- 📈 Descriptive statistics for numerical features
- 📊 Distribution analysis of transaction amounts
- 🔢 Frequency analysis of categorical variables
- 📉 Outlier detection and analysis

### Visualizations

- 📊 Transaction amount distribution (histograms, box plots)
- 🥧 Transaction type breakdown (pie charts)
- 📊 Channel usage comparison (bar charts)
- 🗺️ Geographic distribution analysis
- 🏪 Top merchants and merchant categories
- ⏰ Temporal patterns (hourly, daily, monthly trends)
- 🔍 Fraud flag analysis

## 📈 Analysis & Insights

The notebook provides insights into:

1. **Transaction Patterns**

   - Most common transaction amounts
   - Distribution of credit vs debit transactions
   - Peak transaction hours and days

2. **Channel Preferences**

   - POS vs ATM vs Mobile usage
   - Channel-specific transaction characteristics

3. **Geographic Trends**

   - States with highest transaction volumes
   - Regional spending patterns
   - Urban vs rural transaction distribution

4. **Merchant Analysis**

   - Top performing merchants
   - Popular merchant categories
   - Industry-specific transaction patterns

5. **Security Metrics**
   - Fraud flag prevalence
   - Transaction success rates
   - Anomaly detection indicators

## 📊 Visualizations

The project includes various visualizations:

- Distribution plots for transaction amounts
- Comparative bar charts for channels and states
- Time series plots for temporal analysis
- Heatmaps for correlation analysis
- Geographic distribution charts
- Box plots for outlier identification

## 🛠️ Technologies Used

- **Python 3.9+**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Matplotlib**: Data visualization
- **Seaborn**: Statistical data visualization
- **Jupyter Notebook**: Interactive development environment

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Contribution Ideas

- Add new visualizations
- Implement machine learning models for fraud detection
- Create interactive dashboards using Plotly or Streamlit
- Add time series forecasting
- Improve data preprocessing pipeline
- Add unit tests

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Contact

**Project Maintainer**: Chidinma

**Project Link**: [GitHub Repository URL]

---

## 📚 Additional Resources

- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Matplotlib Gallery](https://matplotlib.org/stable/gallery/index.html)
- [Seaborn Tutorial](https://seaborn.pydata.org/tutorial.html)
- [Nigerian Payment System Overview](https://www.cbn.gov.ng/)

## 🙏 Acknowledgments

- Data source: Nigerian retail transaction dataset
- Inspired by financial data analysis best practices
- Built with open-source tools and libraries

---

**Note**: This is an educational/analytical project. Ensure compliance with data privacy regulations when working with financial transaction data.

_Last Updated: November 2025_
