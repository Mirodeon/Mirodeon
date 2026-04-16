### Odin

**Client :**
Connectic, intégrateur IT & IoT belge spécialisé dans le développement sur-mesure, la gestion de flottes (fleet & asset tracking) et les intégrations ERP / plateformes connectées.

**Rôle :**
Chef de projet, concepteur, développeur full-stack et interlocuteur client

**Contexte :**
Initialement nommé Connectic Hub puis Natacha, le projet a été rebaptisé Odin à mon initiative, en référence à la figure mythologique du dieu nordique du savoir et de la vigilance.  
À l’image d’Odin, dont les corbeaux parcourent le monde pour lui rapporter les nouvelles de tous les royaumes, la plateforme a pour vocation de collecter, synchroniser et centraliser les données issues de multiples sources (Odoo, Flespi, Sensolus, Wialon, FOTA) afin d’offrir une vision unifiée et cohérente du parc IoT de Connectic, soit plus de
60 000 équipements connectés (balises, cartes SIM, véhicules, capteurs, etc.).

**Réalisations :**
* Reprise complète du projet : correction des dysfonctionnements critiques, stabilisation du backend et mise à niveau de l’infrastructure technique.
* Migration architecturale vers les standards internes (Angular + microservices AWS), refonte du modèle de données et ajout d’un système complet de gestion des utilisateurs.
* Refonte des synchronisations automatiques multi-sources (Odoo, Flespi, Sensolus, Wialon, FOTA) :
    + Traitement différentiel pour éviter les réécritures inutiles,
    + Priorisation et hiérarchisation des sources pour consolider les clients et équipements,
    + Fiabilisation des correspondances inter-plateformes et de la gestion des “enfants” (balise + SIM).
* Ajout d’un système de synchronisation manuelle avec suivi d’état persistant (pending, success, error) et mise à jour en temps réel côté client.
* Refonte et unification des commandes distantes (Flespi, Wialon, SMS, etc.) :
    + Exécution groupée ou ciblée par IMEI,
    + Uniformisation du traitement et des retours pour les plateformes distinctes.
* Refonte complète de la gestion des fournisseurs et types de hardware :
    + Ajout de la hiérarchie de mapping multi-plateforme (Odoo, Wialon, Flespi, Sensolus, FOTA),
    + Association de logos, métadonnées et priorisation des identifiants pour assurer la cohérence.
* Uniformisation des interfaces et indicateurs visuels (icônes de plateformes, statuts, alertes, avertissements).
* Collaboration directe avec les équipes internes (System Engineers & Support Engineers) pour résoudre les incohérences d’échanges et fiabiliser la synchronisation globale.

**Environnement technique :**
Angular, TypeScript, Node.js, AWS (Lambda, API Gateway, DynamoDB, S3, Route53, ACM, CloudFront, CloudWatch), Odoo API, Flespi API, Wialon API, Sensolus API, FOTA, GitHub Actions

***

### RFID Zebra

**Partenaires :**
High Tee, Connectic et Etilux.

**Rôle :**
Chef de projet, concepteur et développeur full-stack

**Contexte :**
Projet de recherche et développement subventionné dans le cadre d’un programme d’innovation technologique, réunissant High Tee, Connectic et Etilux autour de la conception d’une application mobile d’inventaire RFID.  
L’objectif était de démontrer la faisabilité technique et logicielle d’une solution mobile interopérable capable de lire, gérer et transmettre des données RFID issues de terminaux Zebra (RFD40 / RFD90 + TC27 / TC53) vers des plateformes métiers telles qu’Odoo ou des applications connectées internes.

**Réalisations :**
* Développement complet de l’application mobile Flutter, assurant l’interface utilisateur, la gestion d’état et la logique d’inventaire RFID.
* Intégration du SDK Zebra RFID via Kotlin natif (Android) pour la communication directe avec les lecteurs RFD40 / RFD90 et les terminaux TC27 / TC53.
* Utilisation du mécanisme d’interfaçage Flutter <=> Kotlin (plugin Flutter natif), enrichi par des services personnalisés des deux côtés :
    + Côté Kotlin : gestion bas-niveau du matériel, lecture continue ou par gâchette, modes d’activation et communication ascendante,
    + Côté Flutter : orchestration des états, réception des données, interaction utilisateur, et synchronisation des requêtes/réponses.
* Conception d’un mécanisme asynchrone de file interne (requêtes <=> réponses) assurant une communication persistante et fiable entre les deux couches malgré les contraintes d’isolation.
* Fonctionnalités principales :
    + Lecture et affichage en temps réel des balises RFID,
    + Création, mise à jour et suppression d’inventaires,
    + Consultation détaillée des balises,
    + Gestion multi-modes (manuel, automatique, déclenchement via zapette).
* Préparation du socle d’intégration avec les systèmes ERP (Odoo) et plateformes internes de Connectic.

**Environnement technique :**
Flutter, Kotlin (Android natif), Zebra SDK (RFD40 / RFD90, TC27 / TC53)

***

### Jost

**Client :**
Jost Group, acteur majeur européen du transport et de la logistique

**Rôle :**
Développeur full-stack, Support R&D

**Contexte :**
Développement d’une application tablette Flutter destinée aux conducteurs de stackers (chariots élévateurs à conteneurs) dans les parcs logistiques du groupe Jost.  
L’application permet de suivre, identifier et gérer les mouvements de conteneurs entre différents sites et zones, en assurant la traçabilité complète des flux.  
Elle s’appuie sur le backend propriétaire de Jost et sur les librairies et modèles Flutter développés en interne par High Tee.

**Réalisations :**
* Contribution à la structure technique et aux librairies Flutter servant de base à l’application (architecture, composants, services, thèmes, gestion d’état).
* Développement de plusieurs écrans fonctionnels pour la gestion des flux, la visualisation des conteneurs et la navigation multi-parcs.
* Fonctionnalités principales :
    + Affichage et suivi des conteneurs (statut, destination, type, température, etc.),
    + Suivi des activités de déplacement et de transport (stackers, quais, parcs),
    + Gestion multi-sites et attribution par stacker.
* Recherche et développement (R&D) sur la lecture automatique des identifiants de conteneurs :
    + Étude des solutions OCR (dont Amazon Textract) et identification de leurs limites pour des environnements visuels non structurés,
    + Expérimentation et validation de la solution Amazon Rekognition, plus adaptée à la détection de texte en contexte libre (angles, luminosité, supports variés),
    + Conception d’un microservice AWS dédié, basé sur les librairies internes AWS, pour traiter et restituer les identifiants reconnus vers l’application Flutter.
* Solution Rekognition validée techniquement avant intégration finale dans la version production.

**Environnement technique :**
Flutter (Dart), TypeScript, Node.js, AWS (Lambda, API Gateway, Rekognition, CloudWatch)

***