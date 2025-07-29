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

## Project Overview

A comprehensive market analysis and interactive dashboard identifying strategic expansion opportunities for Lugg by analyzing 321 metropolitan areas across the United States. The project combines competitive intelligence, demographic analysis, and predictive modeling to prioritize market entry strategies.

**[View Demo Video](https://drive.google.com/file/d/1vf7u3VIbbswkIVTHFkTCqZjW8F8B0xRj/view?usp=sharing)** (1 minute)

<br>

## Key Achievements

• **164 untapped markets** with zero competition identified  
• **$1.48M** combined annual revenue potential from top 3 expansion targets  
• **97.5%** data matching accuracy with Census Bureau MSA definitions  
• **45.5%** market penetration by closest competitor (GoShare)  

<br>

## Technical Implementation

### Data Engineering & Processing
- **Collected location data** for 4 competitors across 892 locations
  - TaskRabbit: 103 cities mapped to 52 MSAs
  - Dolly: 44 cities mapped to 42 MSAs  
  - GoShare: 711 cities mapped to 146 MSAs
  - Lugg: 40 cities mapped to 40 MSAs
- **Standardized geographic data** to OMB-compliant Metropolitan Statistical Area format
- **Integrated Census Bureau demographics** including population and median household income
- **Achieved 97.5% matching rate** between competitor locations and official MSA definitions

### Analytical Methodology

#### Market Scoring Algorithm
```python
Market Attractiveness = (Population Percentile × 0.5) + 
                       (Income Percentile × 0.3) + 
                       (Market Size Bonus × 0.2)

Expansion Score = (Market Attractiveness × 0.6) + 
                  (Competition Opportunity × 0.4)
```

#### Market Size Categories
- Mega markets (5M+): 20 bonus points
- Major markets (2-5M): 15 bonus points
- Large markets (1-2M): 12 bonus points
- Medium markets (500K-1M): 8 bonus points
- Small markets (250K-500K): 4 bonus points

#### Revenue Estimation Model
- Average Order Value: $50
- Market Penetration: 0.1%
- Annual Order Frequency: 12 per customer
- Formula: `Population × 0.001 × $50 × 12`

<br>

## Dashboard Features

### Three Interactive Views
1. **Market Overview**
   - Real-time KPI cards showing total addressable markets
   - Geographic distribution visualization
   - Market size distribution analysis

2. **Competitive Intelligence**
   - Competitor presence by MSA
   - Market penetration comparison
   - Competition intensity matrix

3. **Expansion Priorities**
   - Scored market opportunities
   - Revenue projections
   - Top 15 markets table with demographic data

### Technical Features
- **Embedded Tableau visualizations** with dynamic filtering
- **Responsive design** with CSS Grid and Flexbox
- **Custom animations** using CSS keyframes and transitions
- **Glassmorphism UI** for modern visual appeal
- **Mobile-responsive breakpoints** for various screen sizes

<br>

## Market Analysis Results

### Competition Landscape
| Company | Active MSAs | Market Coverage |
|---------|-------------|-----------------|
| GoShare | 146 | 45.5% |
| TaskRabbit | 52 | 16.2% |
| Dolly | 42 | 13.1% |
| Lugg | 40 | 12.5% |

### Top 10 Expansion Opportunities
| Rank | Metro Area | Population | Median Income | Competitors | Score | Est. Annual Revenue |
|------|------------|------------|---------------|-------------|-------|-------------------|
| 1 | Poughkeepsie-Newburgh-Middletown, NY | 697K | $93K | 0 | 83.2 | $419K |
| 2 | Grand Rapids-Kentwood, MI | 1.1M | $77K | 0 | 82.9 | $652K |
| 3 | Madison, WI | 679K | $83K | 0 | 80.6 | $407K |
| 4 | Riverside-San Bernardino-Ontario, CA | 4.6M | $81K | 1 | 80.6 | $2.8M |
| 5 | Portland-South Portland, ME | 553K | $84K | 0 | 79.4 | $332K |
| 6 | Urban Honolulu, HI | 1.0M | $100K | 1 | 79.3 | $606K |
| 7 | Lancaster, PA | 553K | $81K | 0 | 78.2 | $332K |
| 8 | Manchester-Nashua, NH | 423K | $95K | 0 | 77.5 | $254K |
| 9 | Anchorage, AK | 399K | $93K | 0 | 76.7 | $240K |
| 10 | Harrisburg-Carlisle, PA | 593K | $76K | 0 | 75.9 | $356K |

### Market Distribution by Competition
- Zero competition: 164 markets (51.1%)
- One competitor: 96 markets (29.9%)
- Two competitors: 20 markets (6.2%)
- Three competitors: 20 markets (6.2%)
- Four competitors: 21 markets (6.5%)

<br>

## Strategic Recommendations

### Immediate Priorities
Focus on top 3 markets with combined $1.48M revenue potential:
- Strong demographics (high income, large population)
- Zero existing competition
- Established logistics infrastructure

### Market Entry Strategy
1. **Tier 1**: Major metros with ≤2 competitors (6 markets)
2. **Tier 2**: Large metros with ≤2 competitors (13 markets)
3. **Tier 3**: Medium metros with ≤1 competitor (45 markets)

### Expansion Approach
- Target zero-competition markets first (164 available)
- Avoid markets with 3+ competitors initially
- Prioritize markets with median income >$70K

<br>

## Technical Architecture

```
Data Pipeline:
1. Web Scraping → 2. Data Cleaning → 3. MSA Mapping → 4. Census Integration
                                                              ↓
7. Dashboard Integration ← 6. Scoring Algorithm ← 5. Competitive Analysis
```

### Technology Stack
- **Data Processing**: Python (Pandas, NumPy)
- **Visualization**: Tableau Public API, Custom HTML/CSS/JavaScript
- **Analysis Environment**: Google Colab
- **Data Sources**: US Census Bureau, Competitor Websites
- **Version Control**: Git/GitHub

<br>

## Installation & Usage

### Prerequisites
- Python 3.7+
- Modern web browser (Chrome/Edge recommended)
- Internet connection for Tableau visualizations

### Quick Start
```bash
# Clone repository
git clone https://github.com/priyankaraghunathan15/lugg-market-expansion-analysis.git
cd lugg-market-expansion-analysis

# Open dashboard
open index.html  # macOS
start index.html # Windows

# Run analysis notebook (optional)
jupyter notebook Lugg_Market_Expansion_Analysis.ipynb
```

### Browser Compatibility
- Optimized for 1920x1080 resolution
- Best viewed at 100% zoom
- Chrome/Edge recommended for full feature support

<br>

## Project Structure

```
lugg-market-expansion-analysis/
├── index.html                              # Interactive dashboard
├── styles.css                              # Custom styling & animations
├── lugg-logo.jpeg                          # Company branding
├── Lugg_Market_Expansion_Analysis.ipynb   # Complete analysis pipeline
├── data/
│   ├── census_metro_data.csv              # Census demographic data
│   ├── lugg_strategic_market_analysis.csv # Full analysis results
│   ├── lugg_top_15_expansion_opportunities.csv
│   └── lugg_executive_summary.csv
└── README.md
```

<br>

## Data Sources & Methodology

### Data Collection
- **Competitor Locations**: Scraped from official websites
- **Geographic Standards**: OMB Metropolitan Statistical Area definitions
- **Demographics**: US Census Bureau 2020-2024 estimates
- **Market Boundaries**: Core Based Statistical Area (CBSA) codes

### Quality Assurance
- 97.5% successful MSA matching rate
- Manual verification of top 50 markets
- Cross-validation with multiple census sources
- Outlier detection for demographic data

<br>

## Future Enhancements

- Real-time competitor tracking integration
- Machine learning for demand prediction
- API development for dynamic updates
- Additional demographic factors (age, education)
- Route optimization analysis

<br>

---

**Author**: Priyanka Raghunathan  
**Contact**: [GitHub](https://github.com/priyankaraghunathan15) | [LinkedIn](https://www.linkedin.com/in/priyankaraghunathan)  
**License**: MIT