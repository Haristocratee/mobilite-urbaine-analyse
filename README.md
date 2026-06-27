# 🗺️ Analyse de la Mobilité Urbaine — Île-de-France

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![GeoPandas](https://img.shields.io/badge/GeoPandas-139C5A?style=flat)
![Folium](https://img.shields.io/badge/Folium-77B829?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

> **Aide à la décision publique** : analyse des flux de mobilité multimodaux pour identifier les zones sous-équipées et orienter les investissements d'infrastructure.

---

## 🎯 Problématique

Comment identifier les communes qui cumulent un fort besoin de déplacements et un déficit d'offre de transports en commun, afin de prioriser les investissements en mobilité douce ?

---

## 📊 Données utilisées

| Source | Données | Lien |
|--------|---------|------|
| IDFM Open Data | Validations réseau ferré | [data.iledefrance-mobilites.fr](https://data.iledefrance-mobilites.fr) |
| INSEE | Population par commune | [data.gouv.fr](https://data.gouv.fr) |
| data.gouv.fr | Aménagements cyclables | [data.gouv.fr](https://transport.data.gouv.fr) |
| OpenStreetMap | Réseau viaire & POI | [overpass-api.de](https://overpass-api.de) |

---

## 🗂️ Structure du projet

```
mobilite-urbaine-analyse/
├── notebooks/
│   ├── 01_exploration_donnees.ipynb       # Chargement, nettoyage, EDA
│   ├── 02_analyse_flux_mobilite.ipynb     # Analyse modale et temporelle
│   └── 03_cartographie_interactive.ipynb  # Cartes Folium & choroplèthes
├── data/
│   └── sources.md                         # Instructions de téléchargement
├── outputs/
│   └── (cartes HTML générées)
└── requirements.txt
```

---

## 🔍 Méthodologie (Framework PACE)

1. **Plan** — Cadrage du besoin décisionnel avec les élus
2. **Analyze** — EDA sur les validations IDFM + données démographiques INSEE
3. **Construct** — Cartographie SIG, segmentation des communes
4. **Execute** — Dashboard décisionnel + recommandations actionnables

---

## 📈 Résultats clés

- Identification de **12 communes** combinant forte densité et faible desserte TC
- Corrélation **r=0.73** entre taux d'équipement vélo et part modale douce
- Carte interactive des flux domicile-travail par mode de transport

---

## ⚙️ Installation

```bash
pip install -r requirements.txt
jupyter notebook notebooks/01_exploration_donnees.ipynb
```

---

## 👤 Auteur

**Harry TEGUE** — Data Analyst | Génie Urbain | Paris
🎓 IMT-BS · EIVP · Ex-Mairie de Noisy-le-Grand
📧 harrytegue@gmail.com
