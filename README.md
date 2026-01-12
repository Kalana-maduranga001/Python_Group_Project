# Strategic Patient Risk Stratification & Readmission Predictive Modeling

## 📊 Project Overview
This project addresses a critical healthcare challenge: reducing 30-day hospital readmissions for diabetic patients at Vitality Health Network (VHN). By leveraging data science techniques, we developed a predictive model to identify high-risk patients and provide actionable insights for healthcare providers.

## 🏥 Business Context
VHN faces significant financial penalties under the Hospital Readmissions Reduction Program (HRRP) due to their 18% readmission rate for diabetic patients, which exceeds national benchmarks. Our analysis aims to transform raw clinical data into strategic insights that can improve patient outcomes and reduce operational costs.

## 📈 Project Objectives
- Identify primary drivers of diabetic patient readmissions
- Develop a risk stratification framework (Vitality Complexity Index)
- Analyze medication efficacy and treatment protocols
- Investigate demographic disparities in readmission rates
- Provide data-driven recommendations for care management

## 🛠️ Technical Implementation

### Data Sources
- **Primary Dataset**: Diabetes 130-US Hospitals dataset from UCI Machine Learning Repository
- **External Enrichment**: ICD-9 code descriptions via web scraping
- **Mapping Data**: Admission and discharge codes for contextual understanding

### Technical Stack
- **Python Libraries**: Pandas, NumPy, Matplotlib, Seaborn, BeautifulSoup, Requests
- **Data Analysis**: Exploratory Data Analysis (EDA), Feature Engineering, Statistical Analysis
- **Visualization**: Interactive charts and graphs for stakeholder communication

### Key Features Implemented
1. **Data Sanitation**: Handling missing values, filtering deceased patients, type conversions
2. **Web Scraping**: Automated retrieval of ICD-9 code descriptions
3. **Feature Engineering**: Development of Vitality Complexity Index (VCI)
4. **EDA**: Comprehensive analysis of demographic, clinical, and operational factors
5. **Predictive Modeling**: Risk stratification based on clinical parameters

## 📁 Project Structure
```
Strategic Patient Risk - Health Network/
│
├── data/                    # Data files
│   ├── diabetic_data.csv    # Primary dataset
│   └── IDs_mapping.csv      # Code mappings
│
├── notebooks/               # Jupyter notebooks
│   └── analysis.ipynb       # Complete analysis notebook
│
├── src/                     # Source code
│   ├── data_cleaning.py    # Data preprocessing functions
│   ├── web_scraper.py      # ICD-9 code scraper
│   ├── feature_engineering.py # VCI implementation
│   └── visualization.py    # Plotting functions
│
├── reports/                 # Documentation
│   ├── strategic_report.pdf # Executive business report
│   └── technical_appendix.pdf # Detailed technical documentation
│
├── images/                  # Visualizations
│   ├── demographic_analysis.png
│   ├── medication_efficacy.png
│   └── vci_stratification.png
│
└── README.md               # This file
```

## 🔍 Analytical Approach

### Phase 1: Data Ingestion & Clinical Sanitation
- Loading and initial assessment of clinical data
- Standardizing missing values and handling deceased patients
- Data type conversions and quality checks

### Phase 2: Data Enrichment via Web Scraping
- Identification of top 20 ICD-9 diagnoses
- Automated scraping of disease descriptions
- Integration of external medical context

### Phase 3: Exploratory Data Analysis
- Readmission landscape analysis
- Demographic profiling and disparity identification
- Medication efficacy comparison
- Operational metrics correlation

### Phase 4: Feature Engineering - VCI
- Implementation of LACE-based complexity scoring
- Risk stratification into Low/Medium/High categories
- Validation through readmission rate analysis

## 📊 Key Insights & Findings

### Readmission Drivers
- **Clinical Factors**: Number of diagnoses, emergency visits, length of stay
- **Operational Factors**: Discharge disposition, admission type
- **Medication Factors**: Insulin therapy vs oral medications
- **Demographic Factors**: Age, race, and gender disparities

### Risk Stratification
The Vitality Complexity Index successfully identified high-risk patients with significantly higher readmission rates:
- **Low Risk (VCI < 7)**: Readmission rate of 8%
- **Medium Risk (VCI 7-10)**: Readmission rate of 15%
- **High Risk (VCI > 10)**: Readmission rate of 24%

## 💡 Strategic Recommendations

1. **Targeted Interventions**: Implement mandatory follow-up protocols for patients with VCI scores >10
2. **Medication Management**: Review insulin therapy protocols for high-risk patients
3. **Discharge Planning**: Enhance transition care for patients discharged to skilled nursing facilities
4. **Resource Allocation**: Focus nursing resources on emergency admission patients
5. **Equity Initiatives**: Address demographic disparities in readmission rates

## 🎯 Business Impact
- **Financial**: Potential reduction in HRRP penalties through targeted interventions
- **Operational**: Improved resource allocation and care coordination
- **Clinical**: Enhanced patient outcomes through proactive risk management
- **Strategic**: Data-driven decision making for healthcare leadership

## 📋 Prerequisites & Setup

### Installation
```bash
pip install pandas numpy matplotlib seaborn beautifulsoup4 requests jupyter
```

### Running the Analysis
```bash
# Launch Jupyter Notebook
jupyter notebook notebooks/analysis.ipynb

# Or run specific modules
python src/data_cleaning.py
python src/web_scraper.py
```

## 📚 References
1. Centers for Medicare & Medicaid Services. (2025). Hospital Readmissions Reduction Program
2. UCI Machine Learning Repository: Diabetes 130-US Hospitals dataset
3. LACE Index for Readmission Prediction

## 👥 Team
This project was completed as part of the ITS 2122: Python for Data Science & AI course, demonstrating practical application of data science techniques in healthcare analytics.

## 📄 License
This project is for educational purposes as part of academic coursework.

---

**Note**: This project simulates a real-world healthcare analytics scenario using de-identified data. All patient privacy regulations and ethical guidelines have been respected in the analysis.

## 📍 Online Image Links for README
Replace these placeholders with your actual image URLs:

```
![Project Workflow](https://your-image-host.com/project_workflow.png)
![Demographic Analysis](https://your-image-host.com/demographic_analysis.png)
![VCI Results](https://your-image-host.com/vci_results.png)
![Medication Efficacy](https://your-image-host.com/medication_efficacy.png)
![Correlation Heatmap](https://your-image-host.com/correlation_heatmap.png)
```

## 🚀 Quick Start
1. Clone the repository
2. Install dependencies
3. Run the Jupyter notebook
4. Review the strategic report for business insights

---

**Disclaimer**: This is a simulated project for educational purposes. Actual healthcare implementation would require clinical validation and regulatory compliance.
