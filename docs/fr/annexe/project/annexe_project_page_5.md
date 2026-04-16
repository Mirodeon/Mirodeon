### High Tee Data Management

**Client :**
High Tee

**Rôle :**
Chef de projet, concepteur et développeur full-stack

**Contexte :**
Développement et maintenance d’une plateforme SaaS d’analyse télématique connectée à Flespi, permettant de collecter, agréger et visualiser les données issues de balises et équipements connectés.  
Elle permet aux System Engineers d’administrer les espaces clients, d’activer les calculateurs et compteurs à suivre, et de fournir aux utilisateurs finaux une visualisation claire de leurs activités (trajets, allumages moteur, arrêts, etc.).

**Réalisations :**
* Reprise complète du projet et stabilisation d’un code complexe, incluant diagnostic, correction et refactorisation.
* Refonte intégrale du système de compteurs et calculateurs :
    + Passage d’une architecture rigide (énums codées en dur) à un système modulaire et extensible,
    + Ajout du support pour de nouveaux types de compteurs (trajets, durée moteur, consommation, événements, etc.),
    + Simplification de la maintenance et de l’évolution fonctionnelle sans modification du code source.
* Mappage et intégration des calculateurs Flespi :
    + Détection automatique des calculateurs disponibles lors d’une synchronisation manuelle,
    + Intégration semi-automatisée : remplissage obligatoire des métadonnées (labels, unités, champs requis) avant activation,
    + Activation et gestion réalisées par les System Engineers via l’interface d’administration.
* Optimisation de la visualisation : affichage clair et performant des données télématiques (trajets, arrêts, temps moteur, indicateurs historiques).
* Responsabilité technique complète : supervision, refactorisation, standardisation et amélioration continue dans une optique multi-clients et SaaS.

**Environnement technique :**
Angular, TypeScript, Node.js, AWS (Lambda, API Gateway, DynamoDB, S3, Route53, ACM, CloudFront, CloudWatch), Flespi API, GitHub Actions

***