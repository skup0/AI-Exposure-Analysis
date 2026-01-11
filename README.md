MATH 1130 — AI Exposure & Wage Inequality Analysis (Canada)

OVERVIEW
This project was completed as part of MATH 1130 and analyzes how wages in Canada have evolved
from 2012 to 2024, with a focus on occupational differences, regional patterns, AI exposure,
skill gaps, and inequality.

The analysis integrates multiple publicly available datasets to examine wage levels, wage
dispersion, workforce representation, and employer responses to skill gaps. The project
emphasizes data cleaning, exploratory data analysis (EDA), statistical reasoning, and careful
interpretation of limitations.

All analysis is conducted in a Jupyter Notebook for transparency and reproducibility.

--------------------------------------------------------------------

COURSE CONTEXT
MATH 1130 focuses on applied data analysis and statistical reasoning, including:
- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Visualization and interpretation
- Regression analysis
- Communicating evidence-based conclusions

This project applies these concepts to a real-world labour market dataset.

--------------------------------------------------------------------

DATA SOURCES
The project combines multiple Canadian datasets, including:
- Occupational wage data (2012, 2018, 2024)
- Skill gap and employer training responses
- Workforce gender representation data

All datasets are aggregated at the occupation–region–year level.

--------------------------------------------------------------------

TOOLS & LIBRARIES
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy (linregress)
- Jupyter Notebook

--------------------------------------------------------------------

PROJECT STRUCTURE
.
├── final.ipynb        # Main analysis notebook
├── raw-data/          # Raw input datasets (not included here)
└── README.txt         # Project documentation

--------------------------------------------------------------------

METHODOLOGY

1. DATA CLEANING
- Standardized column names across wage datasets
- Normalized NOC identifiers across years
- Standardized province and region labels
- Removed rows with missing wage values
- Combined wage data into a single long-format dataset
- Cleaned and filtered gender and skill gap datasets to Canada-only records

2. DATA TRANSFORMATION
- Separated hourly and annual wages
- Created an AI exposure proxy using NOC major groups
- Constructed a wage inequality measure (wage gap ratio)
- Applied log transformations to address skewness and extreme values
- Aggregated skill gap responses to identify employer strategies

3. EXPLORATORY DATA ANALYSIS
- Compared wage trends across provinces and occupations over time
- Examined wage differences between AI-exposed and non-exposed occupations
- Analyzed wage distributions and dispersion
- Investigated workforce representation by gender
- Evaluated employer responses to skill gaps

4. STATISTICAL ANALYSIS
- Estimated linear regressions between median wages and wage dispersion
- Quantified the relationship between AI exposure, wage levels, and inequality
- Interpreted results with attention to aggregation and data limitations

--------------------------------------------------------------------

RESEARCH QUESTIONS

RQ1: Industry & Region
How have wages changed across industries and regions from 2012 to 2024, and what patterns
may be linked to AI adoption?

RQ2: Demographics
How do demographic factors influence access to AI-related opportunities?

RQ3: Diversity, Equity & Skill Gaps
What trends are observed in workforce diversity, wage equity, and skill gaps?

RQ4: Benefits & Barriers
Which groups are most likely to benefit from AI adoption, and which face barriers?

--------------------------------------------------------------------

KEY FINDINGS
- Wages increased across provinces and occupations from 2012 to 2024, but unevenly
- AI-exposed occupations consistently earn higher wages
- Wage gains in AI-exposed occupations are more dispersed, indicating higher inequality
- Wage benefits are concentrated rather than evenly shared
- Direct demographic wage analysis is not possible with wage data alone
- Occupational and regional sorting likely reflects structural demographic access
- Employers primarily rely on internal training rather than large-scale reskilling

Regression analysis of AI-exposed occupations shows a strong relationship between median wage
and wage dispersion (R² ≈ 0.60), indicating benefit concentration.

--------------------------------------------------------------------

LIMITATIONS
- AI exposure is measured using an occupational proxy
- Data is aggregated, not individual-level
- Direct demographic wage gaps cannot be measured
- Causal inference is not possible

All demographic interpretations are therefore indirect and structural, not empirical.

--------------------------------------------------------------------

CONCLUSION
AI adoption in Canada is associated with higher wages for skilled occupations but also increased
inequality. Without targeted policy, training, and reskilling interventions, AI-driven growth
may disproportionately benefit already advantaged groups and reinforce existing labour market
stratification.

--------------------------------------------------------------------

HOW TO RUN
1. Clone the repository
2. Install required Python dependencies
3. Open the notebook:
   jupyter notebook final.ipynb
4. Run cells sequentially from top to bottom

--------------------------------------------------------------------

NOTES
This project was completed as part of MATH 1130 coursework and is intended to demonstrate
applied statistical analysis, data cleaning, and interpretation skills.
