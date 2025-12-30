# Maintenance Prédictive Aéronautique par IA

Ce projet exploite des données de capteurs de moteurs afin de prédire le Remaining Useful Life (RUL), c’est-à-dire la durée de vie restante avant qu’une panne ne survienne. Pour ce faire, différents modèles de régression, tels que la régression linéaire et le Random Forest Regressor, sont utilisés.

## Librairies utilisées


- **pandas** 
- **numpy** 
- **matplotlib** 
- **seaborn** 
- **scikit-learn** 


### Étapes du projet

1. **Chargement des données** : Les données des moteurs (`train_FD001.txt`) sont chargées et prétraitées.
2. **Calcul du RUL** : $RUL = \text{cycle maximal du moteur} - \text{cycle courant}$.
3. **Analyse exploratoire des données (EDA)** :
    - Évolution des capteurs pour un moteur.
    - Matrice de corrélation des capteurs.
4. **Prétraitement** :
    - Suppression des capteurs constants.
    - Normalisation des valeurs des capteurs.
5. **Modélisation** :
    - Régression Linéaire.
    - Random Forest Regressor.
6. **Évaluation** : RMSE (Root Mean Square Error) sur l'ensemble de validation pour comparer les modèles.

#### Résultats 

- **RMSE Régression Linéaire :** 30.96
-  **RMSE Random Forest :** 26.24
 
