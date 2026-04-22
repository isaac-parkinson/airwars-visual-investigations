# Measurable Truth: Quantitative Coding of Airwars Visual Investigations
**Dataset v1.0 · Isaac Parkinson · King's College London · 2026**  
**DOI:** https://zenodo.org/records/18761762  
**Licence:** CC0

---

## What this is

The Measurable Truth dataset provides systematic quantitative coding of 13 visual investigations produced by [Airwars](https://airwars.org) between 2021 and 2025. Each investigation is coded across 39 variables covering the types of visual techniques used, how transparently the investigation explains its methods, how it is presented, and how it circulates.

This is an initial corpus designed for expansion. It forms part of *Digital Verite*, a broader research project examining the changing conditions of knowledge production in computational visual documentation across OSINT, journalism, and human rights practice. The coding schema is designed to remain stable as the dataset grows to cover additional institutions and time periods.

---

## Files

| File | Description |
|------|-------------|
| `Airwars_Visual_Investigations_Corpus.xlsx` | Primary dataset. One spreadsheet, two interleaved tables: investigation rows (`INV###`) and technique-instance rows (`INV###_T##`). |
| `airwars_investigations.json` | Investigation-level table as JSON. 13 records, 39 fields. |
| `airwars_techniques.json` | Technique-instance table as JSON. 89 records. |
| `airwars_investigations.csv` | Investigation-level table as CSV. |
| `airwars_techniques.csv` | Technique-instance table as CSV. |
| `airwars_visualisations.html` | Interactive dashboard with 28 charts across 8 thematic sections. Self-contained — open in any browser, no internet required. |
| `Measurable_Truth_Data_Paper.docx` | Full data paper with methodology, variable definitions, and reuse guidance. |
| `README.md` | This file. |

---

## How the data is structured

The dataset has two levels. For each investigation there is one **investigation-level row** (ID: `INV###`) recording overall metrics — technique ratios, reflexivity score, format, collaboration, dates — and a variable number of **technique-instance rows** (ID: `INV###_T##`) recording each individual visual technique observed, its duration, and its properties.

These two tables are interleaved in the Excel file and distinguished by their ID pattern. **If working computationally, start with the JSON or CSV files**, which already separate the two tables. Working directly from the Excel file requires a pre-processing step to filter rows by ID format.

The four technique ratio columns (Observational, Computational, Hybrid, Synthetic) record the proportion of each investigation's total technique duration accounted for by each category. They sum to 1.0 per investigation.

---

## Key variables

| Variable | What it measures |
|----------|-----------------|
| `Reflexivity 0–4` | How explicitly an investigation accounts for its own methods: 0 = none; 2 = dedicated methodology section; 4 = pedagogical |
| `Methodology Y/N` | Whether an explicit methodology statement is present |
| `Computational Ratio` | Proportion of technique duration that is computational (e.g. 3D reconstruction, geolocation mapping) |
| `Observational Ratio` | Proportion of technique duration that is observational (e.g. witness video, photographic stills) |
| `Primary Presentational Format` | 1.1 = Linear video · 1.2 = Interactive database · 1.3 = Scrolling narrative |
| `Interactivity` | Passive / Limited / User-directed / Collaborative |
| `Collaboration` | Whether the investigation had a news media partner |

The full 39-variable schema with all values and definitions is in Appendix A of the data paper.

---

## Coverage and limitations

- **n = 13 investigations · single institution (Airwars) · 2021–2025**
- All statistics should be treated as directional
- No investigations from 2015–2020 are included, as no Airwars investigations from that period carry the Visual category tag used to define the corpus
- All coding was conducted by one researcher; no inter-rater reliability statistics are available for this release

---

## Suggested citation

Parkinson, I. (2026). *Measurable Truth: Quantitative Coding of Airwars Visual Investigations* [Dataset]. Zenodo. https://zenodo.org/records/18761762
