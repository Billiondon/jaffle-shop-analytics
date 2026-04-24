# Rapport d'Intégration : Pipeline Jaffle Shop Analytics

**Statut du système :** Opérationnel / Stable
**Environnement :** Snowflake (DB) + dbt Cloud (IDE)
**Auteur :** Billiondon

## 1. Synthèse du Projet
Mise en œuvre d'une infrastructure de transformation de données (ELT). L'objectif était de sécuriser le flux entre l'entrepôt Snowflake et les modèles de sortie via dbt, en assurant une intégrité totale des droits d'accès et de la structure des schémas.

## 2. Protocole Technique (Interventions)
Le déploiement a suivi le protocole de rigueur suivant :
* **Accès Data Warehouse :** Configuration et isolation du rôle `ACCOUNTADMIN`. Ciblage exclusif de la base `DEMO_DB`.
* **Architecture dbt :** Initialisation des répertoires et purge des modèles d'exemple non conformes.
* **Modélisation :** Création du modèle `customers.sql` (test de charge positif).
* **Versionnage :** Workflow Git validé via Pull Request documentée et fusion (Merge) sur branche principale.

## 3. Validation (Test d'effort)
Le dernier `dbt run` confirme une exécution sans erreur. La donnée est correctement traitée et disponible dans le schéma cible.

## 4. Spécifications
* **Stack :** Snowflake, dbt Cloud, GitHub.
* **Langage :** SQL (DML/DDL).
