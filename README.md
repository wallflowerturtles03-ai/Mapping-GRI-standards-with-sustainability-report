# Mapping GRI Standards with Sustainability Report

This project performs a thematic analysis of sustainability reports to map narrative content to relevant climate and reporting themes. The workflow reads PDF sustainability disclosures, extracts paragraph-level text, applies theme-based keyword coding, and organizes the output in a structured dataset for longitudinal analysis.

The notebook is designed around SLB CDP climate reporting and can be adapted to other disclosure documents or sustainability reports.

## Project Goal

The main objective is to:

- extract text from PDF-based sustainability reports
- segment the content into paragraphs
- classify each paragraph against a set of predefined themes
- summarize theme prevalence over time
- generate output files suitable for reporting and analysis

This supports ESG analysis, sustainability disclosure review, and thematic trend monitoring across reporting years.

## Repository Contents

- `slb_cdp_thematic_analysis.ipynb`  
  Main notebook performing PDF extraction, theme coding, and visualization.

- `slb_cdp_thematic_coding.csv`  
  Structured dataset containing coded report paragraphs and assigned themes.

- `SLB_CDP_Thematic_Analysis_Report.pdf`  
  Exported report or summary document generated from the analysis workflow.

## Methodology

The notebook uses Python libraries including:

- `PyMuPDF` for PDF text extraction
- `pandas` for data handling
- `matplotlib` for thematic charts
- `numpy` for numerical support
- `wordcloud` for keyword visualization

The workflow includes:

1. locating PDF reports in the working directory
2. extracting raw text from each PDF
3. splitting the text into paragraphs
4. cleaning and normalizing the text
5. assigning relevant themes using keyword matching
6. generating a coded output table
7. creating theme frequency summaries and visualizations

## Theme Categories

The coding framework includes themes such as:

- Climate Governance
- Climate Strategy
- Physical Climate Risks
- Transition Risks
- GHG Emissions
- Energy Management
- Technology & Innovation
- Operational Efficiency
- Supply Chain
- Climate Opportunities
- Risk Management
- Targets & Performance
- Sustainable Finance
- Stakeholder Engagement
- Reporting & Transparency

## Usage

Place the relevant PDF reports in the same directory as the notebook, then run the notebook in Jupyter.

Example:

```bash
jupyter notebook slb_cdp_thematic_analysis.ipynb
