# Machine Learning: CART (3-11-2026)

CART (Classification And Regression Trees) built from scratch and with scikit-learn, for both classification and regression.

## Data
- **Classic Play Tennis (14 rows):** classification only.
- **Synthetic tennis data (1,000 rows):** generated in the notebook, with `PlayTennis` for classification and `HoursPlayed` for regression.

## Results

| Dataset | Situation | Metric | Baseline | CART |
|---|---|---|---|---|
| Classic tennis | Classification | Leave-one-out accuracy | 0.643 | 0.596 |
| Synthetic | Classification | Test accuracy | 0.695 | 0.895 |
| Synthetic | Regression | Test RMSE (hours) | 1.053 | 0.468 |
| Synthetic | Regression | Test R² | -0.005 | 0.801 |

The synthetic results show that CART can recover known rules. They do not describe real tennis behaviour.

## Run
```bash
pip install -r requirements.txt
jupyter notebook CART_Tennis_Classification_Regression.ipynb
```

## Author
Mohammed Mutee ([MohammedMutee](https://github.com/MohammedMutee))
