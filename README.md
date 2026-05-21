# Loblaw Companies DCF Valuation

A 3-statement discounted cash flow model of Loblaw Companies Limited (TSX: L), with comparable companies cross-check, scenario analysis, and Monte Carlo simulation on WACC and terminal growth.

**Status:** In progress. Building model in LibreOffice Calc; sensitivity, football-field, and Monte Carlo analysis in Python.

## Scope

- **Subject:** Loblaw Companies Limited (TSX: L)
- **Currency:** CAD
- **Historical window:** FY2021–FY2025 (audited annual reports)
- **Forecast window:** FY2026–FY2030
- **Valuation methods:** DCF (primary), trading comparables, bull/base/bear scenarios, Monte Carlo

## Repo structure

```
loblaw-dcf-valuation/
├── model.xlsx                  # 3-statement DCF model (LibreOffice Calc)
├── memo.pdf                    # 1-page investment memo
├── notebook/
│   └── analysis.ipynb          # sensitivity, football field, Monte Carlo
├── data/
│   └── source-financials/      # Loblaw annual reports FY2021–FY2025
├── screenshots/                # PNG renders of key model tabs
├── docs/
│   └── assumptions.md          # written justification for each assumption
├── environment.yml             # conda environment spec
└── README.md
```

## Reproduction

```bash
git clone git@github.com:tangentjet-33/loblaw-dcf-valuation.git
cd loblaw-dcf-valuation
conda env create -f environment.yml
conda activate loblaw-dcf
jupyter lab notebook/analysis.ipynb
```

Open `model.xlsx` in LibreOffice Calc or Excel.

## Methodology

To be documented as the model is built. See `docs/assumptions.md` for detailed assumption justification.

## Author

Ilya Sharif — Master of Engineering, University of Toronto (Data Analytics & ML). Toronto, ON.

## Disclaimer

This is a personal portfolio project for educational and demonstration purposes. Not investment advice.