# Lugg Market Expansion Analysis

<br>

<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white" alt="Tableau" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
</div>

<br>

## Overview

A data-driven analysis identifying strategic expansion opportunities for Lugg across 321 U.S. metropolitan areas through competitive intelligence and demographic insights.

**[View Demo Video](https://drive.google.com/file/d/1vf7u3VIbbswkIVTHFkTCqZjW8F8B0xRj/view?usp=sharing)** (1 minute)

<br>

## Impact

• Identified **164 untapped markets** with zero competition  
• Projected **$1.48M annual revenue** from top 3 markets  
• Achieved **97.5% accuracy** in geographic data matching  
• Analyzed **892 locations** across 4 major competitors  

<br>

## Approach

### Data Engineering
- Collected and standardized location data from TaskRabbit, Dolly, GoShare, and Lugg
- Mapped 892 locations to Census Bureau Metropolitan Statistical Areas
- Integrated population and income demographics for 321 metro areas

### Analysis
- Developed scoring algorithm: Population (50%) + Income (30%) + Market Size (20%)
- Calculated competitive density and market opportunity scores
- Built revenue projections based on penetration modeling

### Visualization
- Created interactive dashboard with market overview, competitive analysis, and expansion priorities
- Embedded Tableau visualizations for dynamic data exploration
- Implemented responsive design optimized for 1920x1080 displays

<br>

## Key Findings

### Top 5 Expansion Markets

| Metro Area | Population | Income | Competition | Score |
|------------|------------|--------|-------------|-------|
| Poughkeepsie-Newburgh-Middletown, NY | 697K | $93K | None | 83.2 |
| Grand Rapids-Kentwood, MI | 1.1M | $77K | None | 82.9 |
| Madison, WI | 679K | $83K | None | 80.6 |
| Riverside-San Bernardino-Ontario, CA | 4.6M | $81K | Low | 80.6 |
| Portland-South Portland, ME | 553K | $84K | None | 79.4 |

<br>

## Technical Implementation

```
Data Pipeline:
1. Web Scraping → 2. Data Cleaning → 3. Geographic Mapping → 4. Analysis → 5. Visualization
```

**Technologies**: Python (Pandas, NumPy) • Tableau Public API • HTML/CSS/JavaScript

<br>

## Repository Structure

```
lugg-market-expansion-analysis/
├── index.html                              # Interactive dashboard
├── styles.css                              # Custom styling
├── Lugg_Market_Expansion_Analysis.ipynb   # Analysis notebook
└── data/
    ├── lugg_strategic_market_analysis.csv  # Complete results
    └── census_metro_data.csv               # Source data
```

<br>

## Usage

```bash
git clone https://github.com/priyankaraghunathan15/lugg-market-expansion-analysis.git
cd lugg-market-expansion-analysis
open index.html
```

<br>

---

**Author**: Priyanka Raghunathan  
**Contact**: [GitHub](https://github.com/priyankaraghunathan15) | [LinkedIn](https://www.linkedin.com/in/priyankaraghunathan)