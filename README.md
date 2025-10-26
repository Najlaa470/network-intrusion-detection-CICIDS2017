# network-intrusion-detection-CICIDS2017

### Présentation du projet

Ce projet vise à **détecter les intrusions réseau** à l’aide du jeu de données **CICIDS2017**, un benchmark reconnu pour l’évaluation de modèles de détection d’attaques réseau.

L’objectif est de construire, entraîner et évaluer un modèle de machine learning ou deep learning capable de **classer le trafic réseau entre normal et malveillant**.

### Jeu de données : CICIDS2017

Le dataset **CICIDS2017** (Canadian Institute for Cybersecurity) contient du trafic réseau simulé incluant des attaques telles que :

- DDoS
- PortScan
- Botnet
- Infiltration
- Brute Force (FTP, SSH)
- Web Attacks (XSS, SQL Injection, etc.)

<aside>
👌🏻

### Étapes du projet

1. **Importation et exploration du dataset**
    - Chargement des données CICIDS2017.
    - Nettoyage, suppression des valeurs manquantes.
    - Analyse exploratoire (distribution des classes, corrélations, visualisations).
2. **Prétraitement des données**
    - Encodage des labels (**Normal vs Attack** ou multiclass).
    - Normalisation/standardisation des variables.
    - Séparation en ensembles d’entraînement et de test.
3. **Modélisation**
    - Implémentation de plusieurs modèles de classification :
        - Logistic **Regression, Random Forest, XGBoost**
        - **Réseau de neurones** (Keras/TensorFlow)
    - Optimisation des hyperparamètres.
4. **Évaluation**
    - Utilisation de métriques telles que :
        - **Accuracy, Precision, Recall, F1-Score**
        - **Confusion Matrix, ROC Curve**
    - Comparaison entre modèles.
5. **Visualisation et interprétation**
    - Graphiques d’importance des features.
    - Analyse des erreurs et suggestions d’amélioration.
</aside>

### Technologies utilisées

- **Langage** : Python 3.x
- **Bibliothèques principales** :
    - `pandas`, `numpy`, `matplotlib`, `seaborn`
    - `scikit-learn`
    - `tensorflow` / `keras` (si réseau de neurones)
    - `xgboost` ou `lightgbm` (si applicable)

### Résultats attendus

- Détection efficace des attaques avec un score F1 supérieur à 95 % sur le test set.
- Comparaison claire des performances entre différents algorithmes.
- Visualisations et interprétations pour améliorer la robustesse du modèle.
