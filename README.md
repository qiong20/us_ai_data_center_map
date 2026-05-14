# US AI Data Center Map

An interactive animated map visualizing the growth of AI data centers across the United States from 2021 to 2030 (including Epoch AI projections). Bubble size represents power capacity in megawatts (MW), and bubbles are colored by company.

## Live Map

[View the interactive map](https://qiong20.github.io/us_ai_data_center_map/ai_datacenters_animated.html)

## Data Source

Data comes from [Epoch AI's Frontier Data Centers dataset](https://epoch.ai/data/data-centers), an open database that tracks AI data centers using satellite imagery, building permits, and public records. It includes construction timelines, power capacity estimates, and operator information.

Projections beyond 2026 are based on Epoch AI's estimates derived from announced plans and permit data — they are informed forecasts, not confirmed facts.

## What's in this repo

- `ai_data_centers_map_usa.ipynb` — Jupyter notebook with all data fetching, geocoding, and visualization code
- `ai_datacenters_animated.html` — Standalone interactive map (no dependencies, open in any browser)

## How to run

1. Clone this repo
2. Install dependencies:
   ```bash
   pip install plotly pandas requests geopy
   ```
3. Open the notebook in JupyterLab:
   ```bash
   jupyter lab ai_data_centers_map_usa.ipynb
   ```
4. Run all cells in order

## Notes

- A small number of data centers with addresses that failed geocoding were assigned coordinates manually
- The dataset covers frontier AI data centers only — general-purpose cloud infrastructure is not included
- Companies represented include Microsoft, Google, Meta, Amazon, Oracle, SpaceXAI, CoreWeave, Fluidstack, and Softbank
