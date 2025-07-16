# 📈 Ethereum Price Forecasting

Ce projet propose une **analyse complète** et des **modèles de prévision** du prix de l’Ethereum à partir de données historiques. Il combine des approches classiques (**ARIMA**) et des modèles de **Deep Learning** tels que **ANN**, **RNN**, **LSTM**, et **GRU**.

---

## 📊 Description des données

- **Source** : [CoinMarketCap - Ethereum Historical Data](https://coinmarketcap.com/currencies/ethereum/historical-data/)
- **Période** : du 8 août 2015 au 11 décembre 2024
- **Colonnes principales** :
  - `Open` : Prix d’ouverture
  - `High` : Prix le plus haut
  - `Low` : Prix le plus bas
  - `Close` : Prix de clôture
  - `Volume` : Volume échangé

---

## ⚙️ Prétraitement

- Suppression des colonnes inutiles
- Conversion des dates et création de variables temporelles (`month`, `day`, `day_of_week`)
- Vérification et traitement des valeurs manquantes

---

## 📈 Visualisation

- Graphique de l’évolution du **prix de clôture**
- Calcul et affichage des **moyennes mobiles exponentielles** :
  - EMA20, EMA50, EMA100, EMA200

---

## 📉 Modélisation ARIMA

- **Test de stationnarité** avec ADF (Augmented Dickey-Fuller)
- Différenciation des séries si nécessaire
- **Séparation train/test**
- **Sélection des meilleurs paramètres** via Grid Search
- **Validation glissante** (Walk Forward Validation)
- **Évaluation des performances** :
  - MAE
  - MSE
  - RMSE
  - R²

---

## 🤖 Modélisation Deep Learning

- **Normalisation** des données
- Création de **séquences temporelles** pour les modèles
- Modèles testés :
  - **ANN** – Réseau de Neurones Artificiel
  - **RNN** – Réseau Récurrent Simple
  - **LSTM** – Long Short-Term Memory
  - **GRU** – Gated Recurrent Unit
- Visualisation des **prédictions vs valeurs réelles**
- Évaluation avec les mêmes métriques (MAE, MSE, RMSE, R²)


## 🧪 Utilisation

1. Cloner le dépôt :
   ```bash
   git clone https://github.com/<votre-nom-utilisateur>/<nom-du-depot>.git
   cd <nom-du-depot>
