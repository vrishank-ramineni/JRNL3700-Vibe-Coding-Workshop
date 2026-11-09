# Claude.ai use by US state

A one-page map of the Anthropic Economic Index **usage per capita index** for the 50 US states and D.C., May 2026. An index of 1.0 means a state's share of US Claude.ai use equals its share of US working-age (15–64) people.

- `index.html` — the page (D3 + TopoJSON from jsDelivr)
- `data.json` — the 51 values the page uses
- `states-albers-10m.json` — state shapes from [us-atlas](https://github.com/topojson/us-atlas) 3.0.1

## Data

Source: [Anthropic Economic Index](https://www.anthropic.com/economic-index), release of 2026-06-26, file `aei_claude_ai_2026-06-26.csv` from the [Anthropic/EconomicIndex](https://huggingface.co/datasets/Anthropic/EconomicIndex) dataset (CC-BY). The full CSV (~220 MB) is not in this repository. `data.json` keeps rows where `geo_level = subregion`, `geo_id` starts with `US-`, `category_name = overall`, `metric_id = usage_per_capita_index` and `date_start = 2026-05-01`.
