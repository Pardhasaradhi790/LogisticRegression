```mermaid
flowchart TD
    A[Data Sources<br/>• Claims CSV<br/>• Reporting Table CSV<br/>• Rework Status Logs]

    B[Data Ingestion Layer<br/>• Pandas CSV Readers<br/>• Schema Validation<br/>• Data Quality Checks<br/>• Define Success Metrics (MAE, R²)]

    C[Data Processing & Cleaning<br/>• Column Normalization<br/>• Missing Value Handling<br/>• String Standardization<br/>• Datetime Conversion<br/>• Outlier Detection]

    D[Feature Engineering<br/>• TAT Duration Calculation (Target y)<br/>• ClaimID-Based Merge<br/>• Request-Level Aggregation<br/>• Status Count Pivoting<br/>• Rework Frequency Features<br/>• Priority Encoding]

    E[Feature Transformation<br/>• Categorical Encoding<br/>• Numerical Scaling (StandardScaler)<br/>• Feature Readiness Validation]

    F[ML Training Pipeline<br/>• Train/Test Split<br/>• Supervised Regression Models<br/>• RandomForest<br/>• GradientBoosting<br/>• ExtraTrees<br/>• HistGradientBoost<br/>• XGBoost<br/>• LightGBM<br/>• CatBoost<br/>• MLP Baseline]

    G[Hyperparameter Optimization<br/>• GridSearchCV<br/>• Cross Validation (CV=3)<br/>• Bias–Variance Tradeoff<br/>• Overfitting Prevention]

    H[Model Evaluation & Selection<br/>• MAE<br/>• RMSE<br/>• R²<br/>• Best Model Selection (XGBoost)]

    I[Prediction & Interpretation<br/>• Predict TAT (Seconds)<br/>• Convert to HH:MM:SS<br/>• Attach Predictions to Claims]

    J[Output & Consumption<br/>• CSV Reports<br/>• Performance Charts<br/>• Dashboards / APIs<br/>• SLA & Ops Insights]

    K[Monitoring & Continuous Improvement<br/>• Data Drift Detection<br/>• Model Performance Monitoring<br/>• Periodic Retraining<br/>• Feedback Loop]

    A --> B --> C --> D --> E --> F --> G --> H --> I --> J --> K
