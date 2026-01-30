# Appendix C. Time Series Diagnostics and Model Specification Support

**Table CI. Unit Root and Stationarity Test Results for System-Level Demand**

| Test      | Series               |    Stat |     P | Lags |
| --------- | -------------------- | ------: | ----: | ---: |
| Adf       | Y                    |  -2.497 | 0.116 |   26 |
| Kpss (C)  | Y                    |   2.411 | 0.010 |   28 |
| Kpss (Ct) | Y                    |   0.151 | 0.046 |   27 |
| Adf       | Y Diff (1)           | -12.031 | 0.000 |   26 |
| Kpss (C)  | Y Diff (1)           |   0.064 | 0.100 |  121 |
| Adf       | Y Diff (7)           |  -9.936 | 0.000 |   23 |
| Kpss (C)  | Y Diff (7)           |   0.076 | 0.100 |   15 |
| Adf       | Y Diff (1), Diff (7) | -14.893 | 0.000 |   26 |
| Kpss (C)  | Y Diff (1), Diff (7) |   0.007 | 0.100 |   23 |

*Author’s computations based on the cleaned Citi Bike system-level daily demand series.*

**Table CII. Information Criteria and Ljung–Box Residual Diagnostics for Candidate ARIMA and SARIMA Models**

| Model                          |    AIC |    BIC |  LB_p (7) |  LB_p (14) |  LB_p (21) |
| ------------------------------ | -----: | -----: | --------: | ---------: | ---------: |
| SARIMA(1, 0, 1) × (0, 1, 1, 7) | 47,860 | 47,883 | 1.478e-14 |  1.093e-12 |  1.021e-10 |
| SARIMA(1, 0, 1) × (1, 1, 1, 7) | 47,859 | 47,888 | 2.660e-14 |  3.800e-12 |  4.107e-10 |
| ARIMA(1, 1, 1)                 | 47,959 | 47,976 | 9.801e-07 |  8.762e-17 |  1.408e-25 |
| SARIMA(1, 0, 0) × (0, 1, 1, 7) | 48,037 | 48,054 | 6.050e-24 |  8.741e-44 |  1.175e-54 |
| ARIMA(0, 1, 1)                 | 48,096 | 48,107 | 2.149e-37 |  1.492e-56 |  5.748e-73 |
| SARIMA(0, 0, 1) × (1, 1, 1, 7) | 48,137 | 48,160 | 3.683e-71 |  6.087e-96 | 7.288e-105 |
| SARIMA(0, 0, 1) × (0, 1, 1, 7) | 48,143 | 48,160 | 7.636e-73 | 1.676e-100 | 3.152e-113 |
| ARIMA(1, 1, 0)                 | 48,442 | 48,453 | 2.530e-54 |  6.449e-68 |  8.934e-82 |

*Author’s computations based on the cleaned Citi Bike system-level daily demand series.*

**Table CIII. Information Criteria and Ljung–Box Residual Diagnostics for Candidate ETS Models**

| Model         |    AIC |    BIC |  LB_p (7) | LB_p (14) | LB_p (21) |
| ------------- | -----: | -----: | --------: | --------: | --------: |
| ETS(A, N, A)  | 41,724 | 41,776 | 1.072e-17 | 8.109e-16 | 9.496e-14 |
| ETS(M, N, A)  | 41,724 | 41,776 | 1.072e-17 | 8.109e-16 | 9.496e-14 |
| ETS(A, Ad, A) | 41,736 | 41,805 | 2.263e-18 | 9.691e-16 | 2.431e-13 |
| ETS(M, Ad, A) | 41,736 | 41,805 | 2.263e-18 | 9.691e-16 | 2.431e-13 |
| ETS(A, A, A)  | 41,758 | 41,821 | 1.887e-20 | 4.651e-18 | 1.285e-15 |
| ETS(M, A, A)  | 41,758 | 41,821 | 1.887e-20 | 4.651e-18 | 1.285e-15 |

*Author’s computations based on the cleaned Citi Bike system-level daily demand series.*
