# Baghdad Routes Optimizer

not really sure how this project will go, but im ready to go all in.

## Project Structure:

```txt
baghdad-route-optimizer/
├── backend/
│   ├── data/                   # Cached Baghdad road graph & training CSV
│   ├── models/                 # Trained Random Forest / XGBoost model
│   ├── train_risk_model.py     # Step 1: Generates realistic Baghdad delivery data & trains ML model
│   ├── map_engine.py           # Step 2: Downloads Karrada/Mansour OSM road graph & computes real routes
│   ├── vrp_solver.py           # Step 3: Google OR-Tools solver (Naive vs. ML-Risk-Adjusted)
│   ├── main.py                 # Step 4: FastAPI server exposing simulation endpoints
│   └── requirements.txt
├── frontend/
│   ├── src/
│   │   ├── App.jsx             # Interactive Leaflet simulator + KPI comparison
│   │   ├── index.css
│   │   └── main.jsx
│   ├── index.html
│   └── package.json
├── .gitignore
└── README.md
```
