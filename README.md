# Taiwan and the Philippines: growth accounting

**Lauren Nichols · MIT 14.05**

Why did Taiwan and the Philippines follow different productivity paths? This project uses Penn World Table data to compare output per worker, capital accumulation, labor inputs, and a residual measure of productivity.

[Read the paper](reports/growth-accounting-paper.pdf) · [Explore the analysis](notebooks/growth_accounting.ipynb)

## Approach

- Construct country-level time series and log growth rates.
- Decompose output growth into capital, labor, and a residual using observed labor shares.
- Compare five-year periods and examine trade and investment alongside growth.

The exercise is descriptive. Associations with trade and investment do not identify causal effects. Human capital appears in diagnostics but is not a separate contribution in the implemented decomposition; the residual therefore includes human-capital changes as well as other omitted factors and measurement error.

## Run the analysis

Use Python 3, install `requirements.txt`, and place the original workbook in `data/macro_data.xlsx` as described in [data instructions](data/README.md). Open `notebooks/growth_accounting.ipynb` in Jupyter and run its cells in order from the notebooks directory. The five-year table is written to `results/`.

## Files and provenance

The notebook is adapted from the original course analysis: outputs and personal notebook metadata were removed, the installation command was moved to the dependency file, and file paths were made relative. The submitted paper is preserved unchanged. See [validation](VALIDATION.md) for checks and limits.
