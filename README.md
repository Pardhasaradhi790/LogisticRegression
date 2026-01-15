┌──────────────────────────────┐
│        Data Sources          │
│──────────────────────────────│
│ • Claims CSV                 │
│ • Reporting Table CSV        │
│ • Rework Status Logs         │
└───────────────┬──────────────┘
                │
                ▼
┌──────────────────────────────┐
│     Data Ingestion Layer     │
│──────────────────────────────│
│ • Pandas CSV Readers         │
│ • Schema Validation          │
│ • Data Quality Checks        │
└───────────────┬──────────────┘
                │
                ▼
┌──────────────────────────────┐
│  Data Processing & Cleaning  │
│──────────────────────────────│
│ • Column Normalization       │
│ • Missing Value Handling     │
│ • String Standardization     │
│ • Datetime Conversion        │
└───────────────┬──────────────┘
                │
                ▼
┌──────────────────────────────┐
│   Feature Engineering Layer  │
│──────────────────────────────│
│ • TAT Duration Calculation   │
│ • ClaimID-Based Merge        │
│ • Request-Level Aggregation  │
│ • Status Count Pivoting      │
│ • Priority Encoding          │
└───────────────┬──────────────┘
                │
                ▼
┌──────────────────────────────┐
│   ML Training Pipeline       │
│──────────────────────────────│
│ • Train/Test Split           │
│ • Feature Scaling            │
│ • Multi-Model Training       │
│   - RandomForest             │
│   - GradientBoosting         │
│   - ExtraTrees               │
│   - HistGradientBoost        │
│   - XGBoost                  │
│   - LightGBM                 │
│   - CatBoost                 │
└───────────────┬──────────────┘
                │
                ▼
┌──────────────────────────────┐
│ Hyperparameter Optimization  │
│──────────────────────────────│
│ • GridSearchCV               │
│ • Cross Validation (CV=3)    │
│ • R²-Based Model Selection   │
└───────────────┬──────────────┘
                │
                ▼
┌──────────────────────────────┐
│  Prediction & Evaluation     │
│──────────────────────────────│
│ • TAT Prediction (Seconds)   │
│ • HH:MM:SS Conversion        │
│ • MAE / RMSE / R² Metrics    │
└───────────────┬──────────────┘
                │
                ▼
┌──────────────────────────────┐
│ Output & Consumption Layer   │
│──────────────────────────────│
│ • CSV Reports                │
│ • Performance Charts         │
│ • Dashboards / APIs          │
│ • SLA & Ops Insights         │
└──────────────────────────────┘
