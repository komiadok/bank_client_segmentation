<h1 align="center">Configuration de Miniconda </h1>

1. Créer un nouvel environnement
   ```
   conda create -n bsenv python=3.10
   ```
   > `python=3.10` : version de Python souhaitée <br>
   > `bsenv` : nom de l'environnement bank_segmentation_env
2. Activer l'environnement
   ```
   conda activate bsenv
   ```
3. Installer les bibliothèques nécessaires au projet
   ```
   conda install anaconda::pandas
   conda install anaconda::numpy
   conda install anaconda::matplotlib
   conda install anaconda::seaborn
   conda install anaconda::scipy
   conda install anaconda::scikit-learn
   conda install anaconda::xgboost
   conda install anaconda::category_encoders
   ```
4. Installer le notebook jupyter
   ```
   conda install notebook
   ```
