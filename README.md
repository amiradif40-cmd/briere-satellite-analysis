# 🛰️ Analyse Spatiale Multi-Indice : Sécheresse & Stress Hydrique à Saint-Malo-de-Guersac (Brière)

Ce projet propose une analyse comparative de la végétation, du stress hydrique et des niveaux d'eau superficielle sur la commune de **Saint-Malo-de-Guersac** (Marais de Brière, Loire-Atlantique) entre **août 2025** et **août 2026**, à partir d'imagerie satellite **Sentinel-2**.

---

## 📌 Présentation du Projet

L'objectif est d'évaluer l'évolution du couvert végétal et de l'humidité des sols à l'échelle locale en croisant plusieurs indices spectraux issus des bandes optiques et infrarouges de Sentinel-2.

L'étude met en évidence :
* Une baisse globale de la vigueur de la végétation (**NDVI**, **EVI**, **SAVI**).
* Un stress hydrique accru dans la masse foliaire (**NDMI**).
* **Le piège de l'indice NDWI** : une hausse apparente du signal d'eau (**+9,4 %**) expliquée par la fauche et les moissons précoces mettant les sols à nu (faible réflectance dans le proche infrarouge).

---

## 📊 Indices Analysés

| Indice | Nom complet | Rôle & Analyse |
| :--- | :--- | :--- |
| **NDVI** | *Normalized Difference Vegetation Index* | Santé et densité globale de la végétation. |
| **EVI** | *Enhanced Vegetation Index* | Correction des effets atmosphériques et de la saturation de la canopée. |
| **SAVI** | *Soil-Adjusted Vegetation Index* | Ajustement pour les zones à faible couvert végétal / sol nu. |
| **NDMI** | *Normalized Difference Moisture Index* | Teneur en eau à l'intérieur des feuilles (déshydratation végétative). |
| **NDWI** | *Normalized Difference Water Index* | Présence d'eau superficielle et humidité des sols. |
| **NBR** | *Normalized Burn Ratio* | Sensibilité aux zones asséchées et à la biomasse sèche. |

---

## 🛠️ Stack Technique

* **Langage :** Python 3
* **Environnement :** Google Colab / Jupyter Notebook
* **Bibliothèques utilisées :**
  * `rasterio` / `rioxarray` : Manipulation des données spatiales raster (TIFF).
  * `geopandas` / `shapely` : Découpage et gestion des zones d'intérêt (AOI).
  * `matplotlib` / `seaborn` : Visualisation cartographique et tracés des deltas.
  * `numpy` : Calculs matriciels des indices spectraux.

---

## 🚀 Utiliser et Exécuter le Notebook

Vous pouvez exécuter directement le code interactif sur Google Colab sans rien installer en cliquant sur le badge ci-dessous : (https://colab.research.google.com/drive/1FSXOmjY8w67TPoh-4pcF9aZKQT2ApPZ5?usp=sharing)

---

## 📝 Auteur

**Amira DIF** — *Data Science / Computer Vision / Geodata*  
* N'hésite pas à me contacter ou à me suivre sur [www.linkedin.com/in/amira-dif-605574191) !
