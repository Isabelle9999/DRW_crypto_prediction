# DRW_crypto_prediction

Objective: Predict cryptocurrency price movements using 780 anonymized market features
Result: 0.0313 RMSE with Pearson R=0.76
Data Scale: 525K+ minute-level observations across 12 months

Feature Engineering
Hull Moving Averages: Multi-timeframe trend detection with reduced lag
Market Regime Detection: UP/DOWN/HIGH_VOL/STABLE classification for adaptive modeling
Rolling Statistics: Temporal pattern capture across multiple windows
Feature Interactions: Cross-asset relationships and momentum indicators
Microstructure Features: Bid-ask spreads, order flow dynamics

Model Architecture
Algorithm: LightGBM with optimized hyperparameters
Validation: 5-fold walk-forward time series cross-validation
Feature Selection: Stability-based selection reducing 5000+ to 400 optimal features


Project Structure
| Notebook | Description |
|----------|-------------|
| explore_data.ipynb | Initial data exploration and statistical analysis |
| feature_analysis.ipynb | Deep feature analysis and correlation studies |
| target&time_structure.ipynb | Time series properties and target variable analysis |
| HMA_FW_RegimeDetection.ipynb | Hull Moving Averages and market regime implementation |
| Additional notebooks | Cross-validation, model training, and submission pipeline |
