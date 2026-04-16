## Annexe 2025

> Projets et réalisations significatives de 2024-2025, incluant des développements logiciels internes pour High Tee, ainsi que des projets clients majeurs dans les secteurs de l’industrie, de la logistique et de l’énergie.

### Sommaire
+ [Développement logiciel interne](#développement-logiciel-interne)
+ [ElectroSofie](#electrosofie)
+ [MyActEnergy](#myactenergy)
+ [Starfresh Planning](#starfresh-planning)
+ [TMSI Intradel](#tmsi-intradel)
+ [NGE Wialon Module](#nge-wialon-module)
+ [NGE Integration Hiboo-Flespi](#nge-integration-hiboo-flespi)
+ [Connectic Integrations](#connectic-integrations)
+ [Odin](#odin)
+ [RFID Zebra](#rfid-zebra)
+ [Jost](#jost)
+ [High Tee Data Management](#high-tee-data-management)

### Développement logiciel interne

**Client :**
High Tee

**Réalisations :**
* Migration et harmonisation des applications existantes : passage des environnements, librairies et templates Angular 9 => 14 et Flutter 3.16 => 3.22, avec adaptation du SDK cible Android (API 35) pour assurer la compatibilité et la publication continue sur le Play Store.
* Mise en place d’un processus de maintenance annuelle obligatoire pour chaque projet : planification des mises à jour des librairies internes, maintien de la conformité technique et garantie de la pérennité du code pour les futurs développements.
* Refonte complète des librairies internes TypeScript servant de base à l’ensemble des autres librairies du groupe, sur la base de mes propres développements personnels afin d’uniformiser la structure et le typage des projets.
* Enrichissement et maintenance continue des librairies internes TypeScript et Flutter : ajout de fonctionnalités transversales, amélioration du design system, gestion de l’état et de l’asynchrone.
* Développement d’une librairie Angular de composants UI commune pour faciliter et standardiser le design, les services et la logique applicative sur l’ensemble des projets.

**Environnement technique :**
TypeScript, Angular, Flutter (Dart/Kotlin), Node.js, AWS (Lambda, API Gateway, DynamoDB, S3, Route53, ACM, CloudFront, CloudWatch), PostgreSQL, Odoo, GitHub Actions

***

### ElectroSofie

**Client :**
ElectroSofie, société active dans la collecte, le tri, le reconditionnement et la réparation d’électroménagers

**Rôle :**
Chef de projet, concepteur, développeur full-stack et interlocuteur client

**Contexte :**
Réalisation complète d’un écosystème applicatif web et mobile pour la gestion des réparations, productions et clients.

**Réalisations :**
* Conception et développement de l’application web interne pour la gestion des clients, appareils, réparations et productions, avec suivi des statuts, coûts, garanties et génération automatique des bons de commande.
* Développement de l’application mobile Flutter destinée aux techniciens et responsables : attribution des réparations, suivi des statuts, saisie des prestations, matériel, commentaires et formulaires.
* Intégration matérielle : Intégration d'imprimantes Brother et du SDK dédié pour impression d’étiquettes (modèles avec QR code) et ajout d’un module de scan QR dans l’application.
* Conception et développement d’une librairie TypeScript et Flutter permettant de générer des formulaires dynamiques, multi-version et rétrocompatibles, configurables depuis l’application web.
* Mise en place d’une interface d’administration pour le contrôle qualité et la gestion des formulaires de vérification hebdomadaires.
* Gestion complète du projet : analyse du besoin, conception, développement, déploiement web et mobile (Play Store), maintenance et communication directe avec le client.

**Environnement technique :**
TypeScript, Angular, Flutter (Dart/Kotlin), Node.js, AWS (Lambda, API Gateway, DynamoDB, S3, Route53, ACM, CloudFront, CloudWatch), GitHub Actions

***