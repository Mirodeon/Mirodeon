### NGE Wialon Module

**Client :**
NGE, groupe français spécialisé dans les travaux publics, les infrastructures et les services aux entreprises industrielles.

**Rôle :**
Chef de projet, concepteur, développeur full-stack et interlocuteur client

**Contexte :**
Développement d’une application web intégrée à la plateforme Wialon pour permettre au client de générer des rapports Excel complets et unifiés sur ses flottes de véhicules et équipements, en contournant les limitations de traitement natives du système Wialon.

**Réalisations :**
* Développement d’une application client-side embarquée dans Wialon, accessible via le SSID de l’utilisateur connecté, assurant une intégration et une authentification transparentes.
* Conception d’un mécanisme de contournement des limites de traitement Wialon (temps serveur maximal de 10 minutes) : génération séquentielle et contrôlée des rapports individuels pour chaque élément de flotte, avec gestion intelligente des pauses et reprise automatique du processus.
* Agrégation en temps réel des résultats hétérogènes renvoyés par l’API Wialon, puis fusion et mise en forme cohérente dans un rapport Excel unique et structuré.
* Interface web permettant la sélection intuitive du type de rapport, des flottes, des véhicules, des équipements et de la période d’analyse, adaptée aux besoins spécifiques du client.
* Optimisation du pipeline de génération pour garantir la fiabilité, la cohérence et la complétude des rapports, même sur de grands volumes de données.

**Environnement technique :**
Angular, TypeScript, Wialon API (JSON-RPC), ExcelJS,  AWS (S3, Route53, ACM, CloudFront), GitHub Actions

***

### NGE Integration Hiboo-Flespi

**Client :**
NGE, groupe français spécialisé dans les travaux publics, les infrastructures et les services aux entreprises industrielles.

**Rôle :**
Responsable technique, concepteur, développeur full-stack

**Contexte :**
Développement d’un service backend d’intégration assurant la synchronisation périodique des données télématiques entre les plateformes Hiboo (collecte et analyse des données d’engins de chantier) et Flespi (agrégation et diffusion de données IoT), afin de centraliser, uniformiser et fiabiliser les informations issues du suivi de flotte.

**Réalisations :**
* Conception et développement d’un service automatisé côté serveur, exécuté à intervalles réguliers (≈ 5 minutes), configurables selon la fréquence de mise à jour requise.
* Récupération des éléments suivis dans Hiboo à partir des identifiants fournis par NGE (ID Flespi, équipements, véhicules, etc.), puis mise à jour et enrichissement des données correspondantes.
* Reformattage et transformation des données télématiques (compteurs, valeurs instantanées, métriques de fonctionnement, etc.) pour les adapter au format attendu par Flespi.
* Publication des données transformées vers Flespi via un broker MQTT, assurant la continuité des informations dans la plateforme cible.
* Collaboration avec un System Engineer en charge de la plateforme Flespi et prise d’autonomie progressive sur le pilotage technique et la relation client, afin d’assurer la cohérence et la continuité du projet.

**Environnement technique :**
Node.js, TypeScript, API Hiboo, Flespi MQTT Broker, AWS (Lambda, API Gateway, DynamoDB, CloudWatch)

***

### Connectic Integrations

**Client :**
Connectic, intégrateur IT & IoT belge spécialisé dans le développement sur-mesure, la gestion de flottes (fleet & asset tracking) et les intégrations ERP / plateformes connectées.

**Rôle :**
Concepteur, développeur full-stack et formateur technique

**Contexte :**
Développement d’une plateforme web interne permettant de centraliser, superviser et déclencher les différents services d’intégration (Hiboo-Flespi, Wialon, Odoo, etc.), initialement développés comme services isolés. L’objectif était de mutualiser et orchestrer ces intégrations dans un environnement unifié, plus maintenable et plus observable.

**Réalisations :**
* Conception d’une architecture microservices pour regrouper les intégrations existantes sous un même portail.
* Refactorisation de l’application web pour lui permettre de monitorer les intégrations : exécuter manuellement, afficher l’historique, surveiller succès / échec, consulter logs, etc.
* Correction et remise en fonctionnement de l’application, puis déploiement en test et production.
* Intégration de l’intégration Hiboo-Flespi dans ce nouveau cadre centralisé.
* Formation et accompagnement d’un collègue Software Engineer spécialisé Odoo pour le faire monter sur stack web (Angular, AWS, librairies internes).
* Supervision continue du projet : architecture, structure de code, déploiement, alignement technique.

**Environnement technique :**
Angular, TypeScript, Node.js, AWS (Lambda, API Gateway, DynamoDB, S3, Route53, ACM, CloudFront, CloudWatch), GitHub Actions

***