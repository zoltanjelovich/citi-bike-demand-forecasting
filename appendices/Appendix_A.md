# Appendix A. Station Clustering Diagnostics and Composition

**Table AI. Cluster Composition by Station Count and Proportional Share**

| Cluster Label    | Count | Share |
| ---------------- | ----: | ----: |
| Commercial       | 1,460 | 0.405 |
| Residential      | 1,155 | 0.321 |
| Transit-Adjacent |   987 | 0.274 |

*Author’s computations based on the validated station-to-cluster mapping.*

**Table AII. Cluster Distribution within Each Borough**

| Borough Name  | Commercial | Residential | Transit-Adjacent |
| ------------- | ---------: | ----------: | ---------------: |
| Bronx         |      0.000 |       0.000 |            1.000 |
| Brooklyn      |      0.015 |       0.985 |            0.000 |
| Manhattan     |      0.974 |       0.000 |            0.026 |
| Queens        |      0.012 |       0.000 |            0.988 |
| Staten Island |      1.000 |       0.000 |            0.000 |

*Author’s computations based on station–borough assignments.*

**Table AIII. Distribution of Daily Departures per Cluster**

| Cluster Label    | Min |    25% |    50% |    75% |     Max |   Mean |
| ---------------- | --: | -----: | -----: | -----: | ------: | -----: |
| Commercial       | 131 | 33,255 | 51,433 | 69,736 | 125,592 | 52,811 |
| Residential      |  27 |  7,998 | 13,180 | 22,015 |  55,038 | 15,921 |
| Transit-Adjacent |  14 |  1,252 |  3,833 |  8,052 |  19,569 |  5,283 |

*Author’s computations based on cluster-level daily departures.*

!(figures/fig_A1_kmeans_cluster_validity.png)

*Figure A1 – Cluster validity diagnostics for k-means solutions.*
