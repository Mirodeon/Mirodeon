### MyActEnergy

**Client :**
ActEnergy, société de gestion de contrats et de consommation énergétique pour professionnels

**Rôle :**
Chef de projet, concepteur, développeur full-stack et interlocuteur client

**Contexte :**
Reprise et maintenance évolutive d’une application web complexe de gestion énergétique, utilisée pour le suivi complet des contrats, consommations et coûts liés à l’énergie (électricité, gaz, injection).

**Réalisations :**
* Reprise complète du code legacy de la plateforme, analyse et cartographie des interconnexions entre entités clients, sociétés, compagnies et points de fourniture.
* Stabilisation, correction et évolution du système pour garantir la fiabilité des calculs (coûts GRD/GRT, taxes, tarifs fournisseurs, consommations et estimations).
* Développement de nouveaux modules fonctionnels (ajout de pages et entités métier, calculs complémentaires, extensions de reporting et intégrations Excel) pour enrichir la plateforme et répondre aux nouveaux besoins clients.
* Amélioration de la structure de données et des requêtes pour fiabiliser les calculs temporels (mensuels/annuels) et les agrégations budgétaires.
* Génération de rapports, budgets et estimations personnalisés au format Excel et PDF, avec calculs précis.
* Accompagnement du client et maintenance corrective/évolutive continue.

**Environnement technique :**
TypeScript, Angular, Node.js, AWS (Lambda, API Gateway, DynamoDB, S3, Route53, ACM, CloudFront, CloudWatch), GitHub Actions

***

### Starfresh Planning

**Client :**
Starfresh, grossiste en fruits, légumes et produits frais

**Rôle :**
Chef de projet, concepteur, développeur full-stack et interlocuteur client

**Contexte :**
Reprise et maintenance évolutive d’une application Flutter Web destinée à la planification des tournées, à la gestion logistique et au suivi des chauffeurs.

**Réalisations :**
* Reprise du projet et mise à niveau technique, conception et développement de nouvelles fonctionnalités complexes.
* Amélioration de la planification automatisée : génération de tournées standard à partir de modèles, attribution automatique des chauffeurs, camions et quais, avec possibilité d’ajustement manuel.
* Développement d’un module complet de gestion des retours marchandise et vidanges :
    + Encodage des retours directement par les chauffeurs via l’application mobile (photos, quantités, commentaires)
    + Traitement, validation et suivi des retours par les responsables via la plateforme web
    + Intégration d’un flux de validation multi-niveaux connecté à l’API Starfresh, garantissant la synchronisation et la traçabilité des validations entre les acteurs internes et le système central du client.
* Conception et développement d’une application mobile chauffeurs : consultation du planning hebdomadaire, suivi des tournées, retours, congés et informations clients enrichies (photos, vidéos, codes d’accès).
* Génération automatisée de PDF de reporting et de contrôle pour vérification manuelle et correction d’écarts.
* Gestion complète du projet : développement, maintenance, support et communication client directe.

**Environnement technique :**
Flutter (Web & Mobile), Dart, Node.js, AWS (Lambda, API Gateway, DynamoDB, S3, Route53, ACM, CloudFront, CloudWatch), GitHub Actions

***

### TMSI Intradel

**Client :**
Intradel, intercommunale wallonne de gestion des déchets et recyclage

**Rôle :**
Responsable technique, concepteur, développeur full-stack et formateur technique

**Contexte :**
Conception et développement du TMSI (Transport Management System – Intradel), une plateforme web et mobile destinée à la planification, au suivi et à l’optimisation des flux logistiques (tournées, missions, chauffeurs, véhicules, conteneurs, matériaux, sites).

**Réalisations :**
* Conception et développement de l’application web Angular assurant la gestion complète des utilisateurs, chauffeurs, véhicules, conteneurs, matériaux, recyparcs, sites de destination et entrepôts.
* Intégration de l’API Intradel pour la synchronisation automatique des données (création, mise à jour et archivage des missions, recyparcs, matériaux et conteneurs).
* Mise en place d’un planning logistique interactif avec gestion des tournées, filtres dynamiques, codes couleur, actions multiples (création, duplication, déplacement, reports, interruptions, suppressions) et système de versioning évitant les conflits d’édition.
* Développement d’un module d’optimisation de tournées via l’API Google, prenant en compte les contraintes liées aux types de missions, véhicules et séquences d’étapes.
* Développement d’un outil complet de reporting automatisé exportant les activités (missions, tournées, chauffeurs, conteneurs, etc.) vers des fichiers Excel détaillés sur une période donnée.
* Intégration Azure AD (via le tenant Intradel) pour l’authentification unique sur l’application web et mobile, après R&D et externalisation des logiques communes dans les librairies internes.
* Résolution d’un blocage majeur côté client lié à la configuration d’Azure AD : identification immédiate du problème lors d’une réunion technique et mise en œuvre de la solution en moins de 15 minutes après plusieurs semaines d’échanges infructueux entre équipes.
* Participation à la conception technique et fonctionnelle de l’application mobile Flutter, définition des structures de données, des flux et de la cohérence UX/UI avec la plateforme web.
* Supervision et accompagnement d’un collègue Software Engineer sans expérience préalable en développement mobile sur la mise en œuvre Flutter, la structuration du code et les bonnes pratiques, afin d’assurer la cohérence technique entre les volets web et mobile du projet.

**Environnement technique :**
Angular, TypeScript, Flutter (Dart), Node.js, AWS (Lambda, API Gateway, DynamoDB, S3, Route53, ACM, CloudFront, CloudWatch), Azure AD, Google Maps & Routes API, GitHub Actions

***