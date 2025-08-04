# 🏦 Segmentation de Clients Bancaires 

## 📌 Objectif du Projet

Ce projet vise à segmenter les clients d'une institution bancaire à partir de leurs caractéristiques démographiques et comportementales, afin de :

* Identifier les clients à forte valeur ajoutée
* Détecter les profils à risque (emprunt, défaut)
* Adapter les campagnes marketing selon les segments
* Optimiser la fidélisation et les offres personnalisées

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
* `scikit-learn` : clustering (KMeans, DBSCAN, Agglomératif), PCA (réduction de dimension)
* `umap-learn` : réduction de dimension non linéaire (très utile pour visualiser des clusters)
