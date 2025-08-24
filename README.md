# Amazon-Global-Software-Market-Analysis-2025
A comprehensive data science project analyzing Amazon's bestselling software products across 10 global markets to extract business intelligence and market insights.

<img width="794" height="400" alt="image" src="https://github.com/user-attachments/assets/148fd3f3-4002-4d8b-a1f5-0c9c4fdb6373" />


## Project Overview

This repository contains a complete analysis of 999 bestselling software products from Amazon across India, USA, Canada, Australia, Germany, France, Italy, Spain, Japan, and Mexico for 2025.

### Key Findings
- **48.3%** market fragmentation in "Other" software category
- **Kaspersky** leads customer satisfaction (4.54★) despite 8.2% market share
- **European markets** command premium pricing (Germany: $4,315 avg)
- **Budget segment** (<$50) shows highest satisfaction (4.20★)
- **Cybersecurity** category demonstrates best quality-satisfaction ratio

## Business Value

- Market entry strategy recommendations
- Competitive positioning insights
- Regional pricing optimization
- Customer satisfaction benchmarking
- Investment opportunity identification

## Tech Stack

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Plotly** - Interactive visualizations
- **Jupyter Notebook** - Development environment

## Project Structure

```
├── amazon-bestsellers-global-software-market-analysis.ipynb    
├── Amazon_bestsellers_items_2025.csv
├── requirements.txt               
└── README.md                         
```

## Getting Started

### Prerequisites
- Python 3.7+
- Jupyter Notebook
- Git

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/aysannazarmohamady/Amazon-Global-Software-Market-Analysis-2025
cd Amazon-Global-Software-Market-Analysis-2025
```

2. **Create virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Launch Jupyter Notebook**
```bash
jupyter notebook
```

5. **Open and run** `amazon-bestsellers-global-software-market-analysis.ipynb`

## Key Visualizations

The analysis includes comprehensive visualizations covering:

- Market share distribution across countries and brands
- Price vs. rating correlation analysis
- Category performance benchmarking
- Geographic market penetration mapping
- Customer satisfaction trends
- Competitive landscape analysis

## Analysis Methodology

### Data Preprocessing
- Missing value handling and imputation
- Currency normalization to USD
- Brand and category extraction from product titles
- Price segmentation and feature engineering

### Exploratory Data Analysis
- Descriptive statistics and distribution analysis
- Correlation analysis between key variables
- Outlier detection and treatment
- Geographic and categorical segmentation

### Business Intelligence
- Market share and competitive positioning
- Price elasticity and regional variations
- Customer satisfaction benchmarking
- Strategic recommendation framework

## Dataset Information

- **Source**: Amazon Bestsellers 2025 Dataset
- **Size**: 999 products × 12 features
- **Coverage**: 10 countries (IN, US, CA, AU, DE, FR, IT, ES, JP, MX)
- **Categories**: Cybersecurity, Productivity Suites, Operating Systems, Digital Credits
- **Key Metrics**: Ratings, Reviews, Pricing, Rankings

## Key Insights

### Market Leadership
- Microsoft leads in volume (12.4% share) across all regions
- Kaspersky dominates quality metrics (4.54★ average rating)
- Market fragmentation creates opportunities for new entrants

### Pricing Strategy
- European markets accept premium pricing (3-5x higher than competitive markets)
- Budget segment (<$50) shows surprisingly high satisfaction
- Regional arbitrage opportunities exist

### Customer Satisfaction
- 22.8% of products achieve 4.5+ star ratings
- Cybersecurity category leads satisfaction (4.28★)
- Review volume doesn't linearly correlate with rating quality
  
<img width="593" height="399" alt="image" src="https://github.com/user-attachments/assets/40785e5f-b255-43e3-bcac-1e8dbfab552b" />

## Usage Examples

```python
# Load and preprocess data
import pandas as pd
from src.data_preprocessing import clean_data, extract_features

df = pd.read_csv('data/Amazon_bestsellers_items_2025.csv')
df_clean = clean_data(df)
df_features = extract_features(df_clean)

# Analyze market share by region
market_analysis = df_features.groupby(['country', 'brand']).size().unstack()
print(market_analysis)

# Price analysis by category
price_analysis = df_features.groupby('category')['price_usd'].describe()
print(price_analysis)
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.


## Links

- **Kaggle Notebook**: [Complete Analysis](https://www.kaggle.com/code/aysannm/amazon-bestsellers-global-software-market-analysis)
- **Medium Article**: [Business Insights from Amazon's Global Software Market](https://medium.com/@aysan.nazarmohamady/amazon-software-market-report-2025-pricing-competition-and-customer-satisfaction-analysis-a7b604f4cb6c)
- **Dataset Source**: [Amazon Bestsellers 2025](https://www.kaggle.com/datasets/sanskar21072005/amazon-best-sellers-2025/data)

## Author

**Aysan**
- LinkedIn: [aysan-nazarmohammadi]([your-linkedin-url](https://www.linkedin.com/in/aysan-nazarmohammadi-0b72b51a6/))
- Medium: [aysan.nazarmohamady]([your-medium-profile](https://medium.com/@aysan.nazarmohamady))

## Acknowledgments

- Amazon for providing comprehensive marketplace data
- Kaggle community for dataset availability and feedback
- Open source Python community for excellent data science tools

---

⭐ **Star this repository if you found it helpful!**

*For questions or collaboration opportunities, feel free to reach out via GitHub issues or direct contact.*
