# Rapport d'Intégration : Pipeline Jaffle Shop Analytics

**Statut du système :** Opérationnel 
**Environnement :** Snowflake et dbt Cloud 

## Résumé de l'intervention
Mise en place de l'infrastructure de données, qui permet d'établir une connexion stable entre l'entrepôt (Snowflake) et l'unité de traitement (dbt), puis de valider la circulation des informations sans perte ni erreur.

## Protocole suivi
* **Ouverture des accès :** Configuration des droits d'administration pour débloquer le circuit de données (Rôle ACCOUNTADMIN).
* **Nettoyage du foyer :** Suppression des fichiers d'exemples inutiles pour garantir un environnement de travail sain.
* **Test de flux :** Création d'un premier modèle (`customers.sql`) pour vérifier la réponse du système.
* **Validation Git :** Sauvegarde et archivage de l'intervention sur le dépôt principal.

## Résultat du test d'effort
Le dernier contrôle (dbt run) montre un succès total. La donnée circule normalement, le pipeline est stable.

![Preuve du succès dbt](<img width="660" height="213" alt="image" src="https://github.com/user-attachments/assets/e90b5d4c-9454-4bd5-9fc0-b2fb487d5bb1" />
)

## Équipement utilisé
* Entrepôt : Snowflake
* Traitement : dbt Cloud
* Archivage : GitHub
