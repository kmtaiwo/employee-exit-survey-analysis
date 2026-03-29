# Employee exit survey analysis

Standalone analysis of two Queensland (Australia) public-sector employee exit surveys: **DETE** (Department of Education, Training and Employment) and **TAFE** (Technical and Further Education). The work cleans and combines the sources, then explores whether **length of service** and **age group** relate to **resignation** and **dissatisfaction-related** reasons.

## Project layout

| Path | Purpose |
|------|---------|
| `data/` | Raw CSV inputs (`dete_survey.csv`, `tafe_survey.csv`) |
| `notebooks/employee_exit_survey_analysis.ipynb` | End-to-end cleaning, transformation, and analysis |

## Setup

```bash
cd employee-exit-survey-analysis
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

Open the notebook (from the repo root or from `notebooks/`):

```bash
jupyter lab
```

The first code cell resolves `data/` automatically whether your working directory is the repository root or the `notebooks/` folder.

## Data sources

- [TAFE exit survey (data.gov.au)](https://data.gov.au/dataset/ds-qld-89970a3b-182b-41ea-aea2-6f9f17b5907e/details?q=exit%20survey)
- [DETE exit survey (data.gov.au)](https://data.gov.au/dataset/ds-qld-fe96ff30-d157-4a81-851d-215f2a0fe26d/details?q=exit%20survey)

Hosted copies may change over time; the CSVs in `data/` match the versions used for this analysis.

## New GitHub repository

To publish under the name `employee-exit-survey-analysis`:

```bash
cd employee-exit-survey-analysis
git init
git add .
git commit -m "Initial commit: employee exit survey analysis"
git branch -M main
git remote add origin https://github.com/<your-username>/employee-exit-survey-analysis.git
git push -u origin main
```

## Origin

This repository was extracted from a course-level group project so the analysis notebook and data live in a focused, reproducible layout. The original project folder was **not** removed or altered.
