# 🏦 Prédiction de la souscription d'un dépôt à terme 

## 📌 Objectif du Projet

Ce projet vise à prédire si les prospects d'une institution bancaire souscriront (oui/non) un dépôt à terme. Il s'agit d'un problème de classification binaire. 
Pour y arriver, il faudra : 

* Analyser l'efficacité des campagnes marketing téléphonique
  * Quels facteurs influencent le plus la souscription ?
  * Quels segments de clients sont les plus réceptifs ?
  * Quel est le meilleur moment (mois, jour) pour contacter un client ?
  * Combien de contacts sont nécessaires en moyenne pour obtenir une souscription ?   
* Tester et évaluer plusieurs modèles de machine learning 
  * Comparer la performance de différents algorithmes de classification (logistic regression, decision tree, random forest, SVM, etc.)
  * Evaluer les performances selon plusieurs métriques : accuracy, precision, recall, F1-score, AUC-ROC
* Optimiser les campagnes marketing
  * Identifier des profils types de clients susceptibles de souscrire
  * Aider à réduire le coût des campagnes (éviter d'appeler plusieurs fois les clients peu susceptibles de répondre positivement)
  * Fournir des recommandations ciblées pour les campagnes futures 

---

## 📊 Données Utilisées

* **Source** : [Bank Marketing Dataset — UCI](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)
* **Volume** : ~41 000 lignes et 21 colonnes

| Champs         | Description                                       | Type      |
|----------------|---------------------------------------------------|-----------|
| age            | âge du client                                     | Numérique |
| job            | emploi du client                                  | Texte     |
| marital        | statut marital                                    | Texte     |
| education      | niveau scolaire                                   | Texte     |
| default        | a-t-il un crédit en défaut ?                      | Texte     |
| housing        | possède-t-il un prêt immobilier ?                 | Texte     |
| loan           | possède-t-il un prêt personnel ?                  | Texte     |
| contact        | type de communication                             | Texte     |
| month          | mois du dernier contact                           | Texte     |
| day_of_week    | jour du dernier contact                           | Texte     |
| duration       | durée du dernier contact                          | Numérique |
| campaign       | nombre de contacts effectués durant la campagne   | Numérique |
| pdays          | nombre de jours écoulés depuis le dernier contact | Numérique |
| previous       | nombre de contacts effectués avant cette campagne | Numérique |
| poutcome       | résultat de la précédente campagne marketing      | Texte     |
| emp.var.rate   | taux de variation de l'emploi                     | Numérique |
| cons.price.idx | indice des prix à la consommation                 | Numérique |
| cons.conf.idx  | indice de confiance des consommateurs             | Numérique |
| euribor3m      | taux Euribor 3 mois                               | Numérique |
| nr.employed    | nombre d'employés                                 | Numérique |
| y              | le client a-t-il souscrit un dépôt à terme ?      | Binaire   |  

---

## 🧰 Environnement technique

### 🔧 Prérequis

* Installer [Miniconda](https://www.anaconda.com/download/) 
> Entrer son email et choisir la distribution de Miniconda adaptée.<br>
> S'assurer que `(base)` apparaît devant le chemin du disque dur après installation.

### 💻 Technologies utilisées

* Python
* Jupyter Notebook via Miniconda

### 📦 Librairies Python utilisées

* `pandas` : manipulation de données
* `matplotlib` et `seaborn` : visualisations
* `numpy` : traitement numérique
* `scikit-learn` : algorithmes d'apprentissage automatique
* `xgboost` : algorithme d'apprentissage automatique
* `category_encoders` : encodage 
