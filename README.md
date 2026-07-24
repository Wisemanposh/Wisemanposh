# Hi, I'm Trent Stewart 👋

### Applied ML / AI Engineer · Founder, [Elysium Fields AI](https://elysiumfields.ai)

Self-taught ML engineer with 25+ years of creative-technical work behind me. After a career mixing location sound on film and television, I taught myself machine learning and now build and ship deep-learning systems **end-to-end, solo** — with the evaluation discipline to say precisely what each number does and doesn't prove.

📍 Cranbrook, BC, Canada · Open to remote · 📫 **trent@elysiumfields.ai**

---

### 🔭 What I build

A multi-domain environmental-prediction platform: independently trained, per-domain expert models (hydrology, flood, avalanche, drought, wildfire) on a shared **3.3 TB** geospatial data lake, feature store, and reproducible training/evaluation pipeline. I work the whole stack — from scraping government APIs and engineering terabyte-scale data, to training and evaluating models with research-grade rigor, to shipping production apps.

The product thesis is **calibrated operational prediction**, not leaderboard rank: an operator always has yesterday's sensor reading, and a forecast is only useful if its uncertainty is honest.

### 📊 Selected results — public benchmarks

| Task | Result | Published baseline |
|---|---|---|
| **Flood** — pure simulation, 67 gauge-exact GRDC pairs (±20% drainage area, ≤10 km), 2014–2021 | **median NSE 0.61**, ahead on **85%** of gauges | GloFAS operational reanalysis: 0.35 · on par with a published ML benchmark's ungauged random k-fold (0.59) |
| **Streamflow — operational nowcast** (data assimilation), 626 held-out basins, 4 continents | **median NSE 0.83** (log space) / **0.68** (linear); **+0.40 linear over 1-day persistence**; intervals near nominal (50/80/90% → 50.2/77.6/86.0% coverage) | a different task from ungauged simulation — not comparable to the row below |
| **Streamflow — pure simulation, ungauged**, CAMELS-US 531 basins, spatial k-fold | median NSE **0.67** (linear) | Li 2025: 0.79 · Kratzert 2019: 0.69 — **the published baselines still lead here** |
| **Avalanche danger** — 49 zones (live, in production) | **73.2% operational accuracy** (prior-day bulletin as an input); **~52–54%** from weather data alone | approaching the published Swiss SLF operational range (74–78%) |
| **Real-estate price model** — 13.9M+ records | **R² 0.868 · MAPE 9.48%** | — |

*Each row states its task exactly, because the tasks aren't interchangeable: nowcasting **with** observed-discharge assimilation is a fundamentally easier problem than ungauged pure simulation, and NSE computed in log space runs higher than in linear space — so linear is reported wherever a published baseline uses it. Every streamflow, flood, and avalanche number above re-derives bit-identically from its model checkpoints under a fixed verification script. I report the benchmarks I don't beat, too — the ungauged streamflow row is one of them.*

### 🚀 Live products
- **AvalancheWatch** — live avalanche-danger prediction → [avalanche-watch.elysiumfields.ai](https://avalanche-watch.elysiumfields.ai)
- **HydroField** — deep-learning streamflow + offline-first field-data app → [hydrofield.elysiumfields.ai](https://hydrofield.elysiumfields.ai)
- **Elysium Fields AI** → [elysiumfields.ai](https://elysiumfields.ai)

### 🛠️ Stack

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![Lightning](https://img.shields.io/badge/Lightning-792EE5?logo=lightning&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?logo=supabase&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?logo=cloudflare&logoColor=white)
![NVIDIA CUDA](https://img.shields.io/badge/CUDA-76B900?logo=nvidia&logoColor=white)

PyTorch · Lightning · LSTMs · Temporal Fusion Transformers · LightGBM · CatBoost · YOLOv8 · Python · TypeScript · React / React Native · Supabase · Cloudflare · CUDA

### 🧪 How I work
Isolated experiments · reproducible configs · calibrated uncertainty (CRPS) · locked sacred test sets · pre-registered thresholds · honest benchmark reporting. A result isn't a result until it re-derives from its artifacts and survives a check for what else could explain it — including the checks that kill my own claims. Self-taught by building that discipline the hard way; every project is the curriculum.

---

📫 **trent@elysiumfields.ai** · [LinkedIn](https://www.linkedin.com/in/trent-stewart-1522943b3/) · [elysiumfields.ai](https://elysiumfields.ai)
