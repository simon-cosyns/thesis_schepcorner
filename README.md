# Masterproef – Data-driven onderzoek naar nichesport: de schepcorner in het minivoetbal

Deze repository bevat de code en analyses ontwikkeld in het kader van mijn masterproef aan de Universiteit Gent. De focus ligt op het onderzoeken van de schepcorner in minivoetbal via zowel beschrijvende statistiek als predictieve modellering.

> **Titel**: *Data-driven onderzoek naar nichesport: de schepcorner in het minivoetbal*  
> **Auteur**: Simon Cosyns  
> **Opleiding**: Master in Handelsingenieur – Data Analytics  
> **Universiteit**: Universiteit Gent  
> **Academiejaar**: 2024–2025

---

## Structuur van de repository

### `Data/`

- **Bronze/**: Ruwe data uit observaties en enquêtes (`.xlsx`)
- **Silver/**: cleaned data en gecontroleerde data, aangepast uit directe observaties (`_cleaned`)
- **Gold/**: Finale train/test-sets voor het predictieve model (`.csv`)

### `Notebooks/`

#### `data_cleaning/`
- `data_check.ipynb`: Controle en verbetering van datakwaliteit (missende waarden, validatie)
- `controle.ipynb`: Vergelijking tussen observaties en zelfgerapporteerde enquêtes

#### `descriptive/`
- `impact.ipynb`: Analyse van de impact van schepcorners en momentum, inclusief simulatie van een regelwijziging
- `statistiek.ipynb`: Exploratieve statistiek en variabelebeschrijving

#### `predictive/`
- `feature_engineering.ipynb`: Feature creatie, imputatie, en datasplitsing
- `model.ipynb`: Predictieve modellen (Logistic Regression, Random Forest, XGBoost), inclusief feature selection met permutation importance en Boruta
