# U.S. Open Venue Difficulty — Statistical Analysis

Supplementary code and data for the research paper *"Measuring Championship Venue Difficulty in U.S. Open Golf: A Cross-Dataset Analysis Using Adjusted Field Scoring Average, Formal Inferential Tests, Women's Open Results, and Amateur Stroke Play Data"* by Junaid Mohiuddin.

This repository reproduces every formal statistical test reported in the manuscript, including the Welch's t-tests, one-way ANOVA, the 2021 U.S. Amateur natural experiment, within-venue variance analysis, and the field-strength regression.

## Contents

| File | Description |
|---|---|
| `statistical_analysis.py` | Main analysis script. Reproduces all statistical tests (Tables 3–6, 9, and 12) when run. |
| `primary_dataset_fsa.csv` | Modern era (2010–2026) U.S. Open field scoring averages, winners, and tier classifications (Table 2). |
| `historical_dataset_fsa.csv` | Pre-modern era (1947–2009) field scoring averages, treated as directional only (Table 10). |
| `womens_open_dataset.csv` | U.S. Women's Open results at venues shared with the Men's Open (Table 7). |
| `amateur_dataset.csv` | U.S. Amateur stroke play data at shared venues, including the 2021 Oakmont natural experiment (Table 8). |
| `us_open_strengths.csv` | Data Golf field-strength index by tournament round, 2010–2026, used for the field-quality confound test (§6.3.2, Table 12). |

## Running the analysis

Requires Python 3.8+, numpy, and scipy.

```bash
pip install numpy scipy
python statistical_analysis.py
```

The script prints descriptive statistics, all five primary statistical tests, and the field-strength regression to stdout, matching the tables and figures reported in the manuscript.

## Data sources

- Modern era field scoring averages: [Data Golf](https://datagolf.com/past-results/majors/26)
- Historical field scoring averages: GOLF Magazine, ESPN Stats & Information, USGA Championship Records
- U.S. Amateur and Women's Open data: USGA Media Center, USGA Championship Records, Wikipedia
- Field strength index: Data Golf

## Citation

If you use this code or data, please cite the accompanying manuscript (preprint, SportRxiv, 2026).

## Contact

Junaid Mohiuddin — JGMohiuddin@gmail.com — [ORCID: 0009-0009-8806-4853](https://orcid.org/0009-0009-8806-4853)
