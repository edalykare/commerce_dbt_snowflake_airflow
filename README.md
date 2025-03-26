3W2XXSJ92V7YB7XVSY33EN5V
A. Collecte et ingestion des données
  Source de données : Générer des données de logs clients (fréquence de connexion, nombre d’achats, support client...)  
  Stockage : Sauvegarder ces logs dans PostgreSQL / Snowflake
  Automatisation : Utiliser Airflow pour exécuter une ingestion journalière
B. Préparation et Feature Engineering
  Nettoyer les données avec Pandas
  Créer des nouvelles features (ex: taux d’utilisation sur 7 jours, interactions avec le support...)
  Stocker les données transformées dans une table "feature store"
C. Entraînement du modèle ML (Hebdomadaire)
  Récupérer les données pré-traitées
  Séparer en train/test et entraîner un modèle XGBoost
  Suivre les métriques avec MLflow
  Sauvegarder le modèle versionné
