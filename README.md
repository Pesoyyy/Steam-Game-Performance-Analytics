# Analisis Kinerja dan Trend Game di Platform Steam Tahun 2024

## Repository Outline

* README.md - Penjelasan gambaran umum project
* Notebook for Analysis.ipynb - Notebook berisi eksplorasi data, analisis statistik, visualisasi, dan pemodelan
* dataset.csv - Dataset raw yang akan diolah untuk dianalisa secara mendalam dalam project ini
* dataset_cleaned.csv - Dataset game Steam (2024) yang sudah di bersiihkan dengan variabel: revenue, copiesSold, price, reviewScore, dll.
* dataset_cleaned.xlsx - Dataset game Steam (2024) yang sudah di bersiihkan dengan variabel: revenue, copiesSold, price, reviewScore, dll, dalam bentuk excel untuk di upload ke Tableau
* Dashboard Analysis.twbx - File Dashboard Tableau untuk analisa ini

## Problem Background

Pasar game PC di Steam mengalami pertumbuhan pesat, terutama dari publisher indie. Namun, terdapat ketimpangan kinerja antar game:

* **Mayoritas game** memiliki pendapatan rendah, sedangkan **minoritas outlier** menghasilkan revenue sangat tinggi.
* **Perbedaan model** monetisasi (*free-to-play* vs.  *berbayar* ) memengaruhi pola pendapatan dan volume penjualan.
* **Tujuan Project** : Menganalisis faktor-faktor yang memengaruhi kesuksesan game (revenue, penjualan, rating) dan memberikan rekomendasi strategi monetisasi.

## Data

**Sumber** : Dataset Steam (2024) - simulasi data untuk analisis. (refrensi dataset ada dibawah)

**Karakteristik** :

* **1.500 observasi** (85 game gratis, 1.415 berbayar).
* **Colum** :
* **Variabel kunci** : `revenue`, `copiesSold`, `price`, `reviewScore`, `avgPlaytime`.
* **Missing values** : Tidak ada (*count = 1500 untuk semua variabel*).

## Stacks

* import numpy as np
* import pandas as pd
* import scipy as sp
* import scipy.stats as stats
* import matplotlib.pyplot as plt
* import seaborn as sns
* import pandas as pd
* import statsmodels.api as sm
* import matplotlib.pyplot as plt
* import seaborn as sns
* from sklearn.preprocessing import StandardScaler
* from sklearn.cluster import KMeans
* from sklearn.decomposition import PCA
* from sklearn.metrics import silhouette_score
* from scipy.stats import mannwhitneyu, chi2_contingency, spearmanr

## Reference

[https://www.kaggle.com/code/emanhesham55/top-1500-games-on-steam-by-revenue-analysis](https://www.kaggle.com/code/emanhesham55/top-1500-games-on-steam-by-revenue-analysis)

## Link Tableau

[Tableau Dashboard](https://public.tableau.com/views/DashboardTableau_17478309923130/Page1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
