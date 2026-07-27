# Census Demographic Analysis & Local Planning

A data-analysis project using a mock census dataset to identify demographic and socio-economic patterns and translate them into evidence-based local planning recommendations.

The project demonstrates a complete analytical workflow: **data inspection, cleaning, validation, feature engineering, exploratory analysis, visualisation, interpretation and decision support**.

## Project Context

The fictional town is situated between two larger cities. The analysis was designed to answer two practical planning questions:

1. What should be developed on an available plot of land?
2. Which area should receive additional local-government investment?

Options included housing, transport, religious facilities and healthcare development, alongside investment in education, employment/training, old-age care and general infrastructure.

## Dataset

The mock census dataset contains demographic and household information including age, marital status, gender, occupation, religion, household structure and infirmity.

The raw dataset contained missing values, inconsistent categories and implausible entries that required cleaning before analysis. The source dataset is not included in this repository. See [`data/README.md`](data/README.md).

## Data Cleaning & Validation

The analysis included:

- inspecting columns, data types and missing values;
- handling missing or unresolved demographic information;
- standardising inconsistent categorical values;
- checking duplicate household records;
- validating ages and treating implausible values;
- cleaning free-text occupation information.

## Feature Engineering

Residents were grouped into six age bands: Children (0–17), Young Adults (18–24), Early Career (25–40), Mid-age (41–64), Retired (65–80) and Elderly (81+).

Additional features included an infirmity indicator and broader occupation categories suitable for aggregation and visualisation.

## Demographic Findings

### Age Distribution

| Age Group | Population |
|---|---:|
| Children (0–17) | 1,784 |
| Young Adults (18–24) | 812 |
| Early Career (25–40) | 1,894 |
| Mid-age (41–64) | 2,204 |
| Retired (65–80) | 645 |
| Elderly (81+) | 199 |

The population is dominated by working-age adults, while the sizeable child population indicates meaningful current and future demand for education and community infrastructure.

### Employment Profile

Key proportions included Students **26.36%**, Retired **8.76%**, Technology **7.54%**, Unemployed **6.62%**, Engineering **4.80%**, Management **4.13%** and Healthcare **2.44%**.

The large student population was particularly important to the transport recommendation because the fictional town itself does not contain a university.

### Religion

Christianity represented **42.55%** of the population and no religious affiliation **41.53%**, followed by Unknown **13.11%**, Islam **1.42%**, Hinduism **0.94%** and Sikhism **0.35%**.

### Infirmity

**99.06%** had no recorded infirmity and **0.94%** had a recorded infirmity. Although current recorded infirmity is low, the older population remains relevant when considering longer-term healthcare planning.

## Evidence-Based Recommendations

### Development Recommendation: Train Station

The analysis recommends using the available land for a **train station**. The recommendation is supported by the substantial student population and residents likely to commute to neighbouring cities. Improved transport connectivity could support education access, employment mobility and wider economic activity.

### Investment Recommendation: Education

The recommended local-government investment priority is **schooling and education**. There are **1,784 children aged 0–17**, alongside a substantial early-career population that may contribute to future household and family growth.

## Analytical Workflow

```text
Raw Census Data
      ↓
Data Inspection
      ↓
Cleaning & Validation
      ↓
Feature Engineering
      ↓
Exploratory Data Analysis
      ↓
Visualisation
      ↓
Demographic Interpretation
      ↓
Local Planning Recommendations
```

## Technologies

**Python • Pandas • NumPy • Matplotlib • Seaborn • Jupyter Notebook • Data Cleaning • Exploratory Data Analysis • Feature Engineering • Data Visualisation**

## Repository Structure

```text
census-demographic-analysis/
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
├── notebooks/
│   └── census_demographic_analysis.ipynb
├── data/
│   └── README.md
└── results/
    └── figures/
```

## Installation

```bash
git clone https://github.com/Ape-programmer/census-demographic-analysis.git
cd census-demographic-analysis
python -m venv .venv
pip install -r requirements.txt
```

Place the dataset according to `data/README.md`, then launch Jupyter from the repository root.

## Key Skills Demonstrated

- real-world-style data cleaning;
- categorical standardisation;
- demographic feature engineering;
- exploratory analysis;
- clear visual communication;
- interpretation of socio-economic patterns;
- translating evidence into actionable recommendations.

## Limitations

- The dataset represents a fictional town rather than an official contemporary census population.
- Some missing or inconsistent values required judgement during preprocessing.
- Demographic patterns support planning decisions but do not establish causal relationships.
- Recommendations are constrained by the options defined for the original planning scenario.

## Future Improvements

Potential extensions include interactive demographic dashboards, household-level analysis, geographic mapping, automated data-quality reporting, scenario scoring and comparison with official census indicators.

## Author

**Abiola Peace Emmanuel**  
MSc Artificial Intelligence & Data Science  
GitHub: **Ape-programmer**
