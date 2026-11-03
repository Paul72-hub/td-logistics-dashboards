# Logistics dashboards — three roles, three KPIs

One French logistics network (warehouses in Paris, Lyon and Lille serving 20 cities),
three dashboards built for three different decisions:

- `co2.html` — sustainability manager: which routes to prioritize for CO2 reduction
- `cost.html` — operations manager: is each warehouse's cost problem transport or storage
- `network.html` — strategy manager: open Bordeaux or Marseille, or close Lille

`scripts/compute_kpis.py` computes all three from `data/cities.csv`. The GitHub Action
(`compute.yml`, manual trigger only) runs it and commits `docs/data/*.json`, served by
GitHub Pages from `docs/`.

Assumptions (all shown on the dashboards): demand estimated from population (50 t/year
per 1,000 residents, illustrative), 0.10 kg CO2e per tonne-km (within the published
ADEME/Ministry range), 0.12 EUR per tonne-km transport and 40 EUR per tonne per year
storage (illustrative, not sourced).
