# Appendix D. Supplementary Model Diagnostics and Performance Results

**Table DI. Forecast Accuracy of SARIMAX and ETS Models on Validation and Test Samples**

| Model                                      | Split           |   RMSE |    MAE | MAPE (%) |
| ------------------------------------------ | --------------- | -----: | -----: | -------: |
| ETS(A, N, A), S = 7 + Exog                 | Test 2023–2024  | 15,181 | 10,895 |    14.00 |
| SARIMAX(1, 0, 1) × (0, 1, 1, 7) + Exog     | Test 2023–2024  | 15,476 | 11,095 |    14.22 |
| ETS(A, N, A), S = 7 + Exog (Minus Weather) | Test 2023–2024  | 20,484 | 14,733 |    19.79 |
| ETS(A, N, A), S = 7                        | Test 2023–2024  | 20,598 | 14,623 |    19.77 |
| ETS(A, N, A), S = 7 + Exog                 | Validation 2022 | 12,171 |  9,183 |    16.80 |
| SARIMAX(1, 0, 1) × (0, 1, 1, 7) + Exog     | Validation 2022 | 12,235 |  8,964 |    16.67 |
| ETS(A, N, A), S = 7                        | Validation 2022 | 16,313 | 12,288 |    24.89 |
| ETS(A, N, A), S = 7 + Exog (Minus Weather) | Validation 2022 | 16,363 | 12,454 |    25.18 |

*Author’s computations based on Citi Bike system-level daily demand forecasts.*

**Table DII. Estimated SARIMAX Coefficients with Exogenous Variables**

| Indicator        |    Coef | Std Err | T Value |
| ---------------- | ------: | ------: | ------: |
| is_weekend       |   0.000 |  11,087 |   0.000 |
| is_holiday       | -11,265 |   1,489 |  -7.567 |
| regime_pre_covid |   7,024 |   9,101 |   0.772 |
| regime_covid     |  17,500 |  14,408 |   1.215 |
| regime_recovery  |  21,563 |  18,714 |   1.152 |
| temp_avg_f       |     819 |  57.525 |  14.230 |
| precip_inches    | -20,900 | 275.288 | -75.919 |
| ar.L1            |   0.957 |   0.013 |  74.067 |
| ma.L1            |  -0.675 |   0.026 | -25.523 |
| ma.S.L7          |  -0.904 |   0.014 | -63.182 |

*Author’s computations based on Citi Bike system-level SARIMAX estimates.*

**Table DIII. Estimated Marginal Effects of Prophet Exogenous Regressors**

| Regressor        |   Beta | Approx Trips per Unit |
| ---------------- | -----: | --------------------: |
| is_holiday       | -0.019 |                -3,347 |
| precip_inches    | -0.038 |                -3,154 |
| is_weekend       | -0.032 |                -2,053 |
| regime_covid     | -0.008 |                  -603 |
| temp_avg_f       | -0.051 |                   -87 |
| regime_recovery  |  0.002 |                   144 |
| regime_pre_covid |  0.023 |                 1,791 |

*Author’s computations based on Prophet model estimates for Citi Bike system-level demand.*

![](figures/.png)

*Figure D1 – SARIMAX residual diagnostics.*

![](figures/.png)

*.*
