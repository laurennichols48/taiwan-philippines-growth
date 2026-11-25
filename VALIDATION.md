# Validation and preparation notes

The notebook ran successfully from first to last cell on the original workbook during portfolio preparation on November 25, 2026. It produced the five-year CSV and LaTeX tables in `results/`. This verifies execution, not every statement in the submitted paper.

Changes from the original notebook:

- Replaced the inline package installation with `requirements.txt`; made input and output paths relative.
- Fixed the residual-productivity plot to use the calculated growth-accounting frames, plot the signed residual directly rather than take its logarithm, and label the axis correctly.
- Set the aggregation interval to five years to match the exported filenames (the original setting was ten).
- Removed an empty human-capital contribution column from the exported table; human capital remains outside the implemented decomposition.
- Removed saved outputs and personal notebook metadata. The submitted paper was not edited.

The notebook reproduces the growth-accounting component. The paper’s discussion of trade and investment is not a separate regression implementation in this notebook. Country-year coverage can differ after dropping missing inputs, and boundary bins can contain fewer than five observations. The plotted residual is not a pure measure of technology.
