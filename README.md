
<h1 align='center'>Lugg Market Expansion Analysis</h1>

<p align="center">
  <img src="images/lugg-image.jpeg" alt="Lugg Moving Truck" width="500"/>
</p>
"""

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
</p>

---

## Overview

This project provides a comprehensive market analysis and dashboard to support Lugg’s strategic expansion into new metropolitan areas across the United States. It integrates competitive landscape assessment, demographic profiling, and a scoring algorithm to prioritize market entry opportunities.

**[Demo Video (1 minute)](https://drive.google.com/file/d/1vf7u3VIbbswkIVTHFkTCqZjW8F8B0xRj/view?usp=sharing)**

---

## Key Outcomes

- **164** metro areas with zero competition identified
- **$1.48M** projected annual revenue from the top three expansion targets
- **97.5%** geographic matching accuracy with U.S. Census MSA definitions
- **45.5%** market share held by top competitor GoShare

---

## Technical Approach

### Data Engineering

- Extracted competitor location data from official sources
- Mapped 892 city-level entries into 321 Metropolitan Statistical Areas (MSAs)
- Integrated U.S. Census Bureau data for population and income metrics
- Standardized locations using OMB-compliant MSA naming

### Analytical Framework

#### Expansion Scoring Algorithm

```python
Market Attractiveness = (Population Percentile × 0.5) + 
                        (Income Percentile × 0.3) + 
                        (Market Size Bonus × 0.2)

Expansion Score = (Market Attractiveness × 0.6) + 
                  (Competition Opportunity × 0.4)
```

#### Revenue Projection Model

- Assumptions:
  - $50 average order value
  - 0.1% market penetration
  - 12 orders per customer per year
- Formula: `Population × 0.001 × $50 × 12`

---

## Dashboard Highlights

- **Overview**: KPI cards, market distribution charts
- **Competitive Intelligence**: Competitor presence, intensity matrix
- **Expansion Priorities**: Ranked expansion targets, demographic insights

---

## Market Insights

### Top 5 Recommended Markets

| Metro Area | Population | Median Income | Score | Est. Revenue |
|------------|------------|---------------|-------|---------------|
| Poughkeepsie, NY | 697K | $93K | 83.2 | $419K |
| Grand Rapids, MI | 1.1M | $77K | 82.9 | $652K |
| Madison, WI | 679K | $83K | 80.6 | $407K |
| Riverside, CA | 4.6M | $81K | 80.6 | $2.8M |
| Portland, ME | 553K | $84K | 79.4 | $332K |

---

## Technical Stack

- **Languages**: Python, HTML5, CSS3, JavaScript
- **Libraries**: Pandas, NumPy
- **Visualization**: Tableau Public (embedded), CSS animations
- **Data Sources**: U.S. Census Bureau, Competitor websites
- **Environment**: Google Colab, GitHub

---

## Setup Instructions

### Prerequisites

- Python 3.7+
- Web browser (Chrome/Edge recommended)

### Quick Start

```bash
# Clone repository
git clone https://github.com/priyankaraghunathan15/lugg-market-expansion-analysis.git
cd lugg-market-expansion-analysis

# Open dashboard
open index.html  # macOS
start index.html # Windows
```

---

## Repository Structure

```
lugg-market-expansion-analysis/
├── index.html                        # Dashboard
├── styles.css                        # Styling
├── Lugg_Market_Expansion_Analysis.ipynb  # Jupyter analysis notebook
├── data/
│   ├── census_metro_data.csv
│   ├── lugg_strategic_market_analysis.csv
│   ├── lugg_top_15_expansion_opportunities.csv
│   └── lugg_executive_summary.csv
└── README.md
```

---

## Future Enhancements

- Competitor data automation via APIs
- Demand forecasting using machine learning
- Inclusion of advanced demographics (e.g., age, education)
- Real-time Tableau dashboard via server integration

---

**Author**: Priyanka Raghunathan  
**License**: MIT  
**Contact**: [GitHub](https://github.com/priyankaraghunathan15) | [LinkedIn](https://www.linkedin.com/in/priyankaraghunathan)
