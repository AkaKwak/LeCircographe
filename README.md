### Projet de site web pour le Circographe

#### 1. Présentation

Ce projet vise à créer une plateforme web pour l’association Circographe, un espace artistique à Toulouse dédié aux arts du cirque et aux arts urbains.<br><br>Le site répondra à deux besoins principaux :<br>- **Frontend public** : destiné au grand public pour informer et attirer vers les activités de l'association. <br>- **Dashboard administrateur** : pour aider le bureau de l’association à gérer les membres(inscriptions, présences), les événements, la gestion de la salle et les finances

L'objectif est d'offrir une solution intuitive et complète qui optimise la gestion associative tout en valorisant la visibilité du Circographe auprès de la communauté.

### 2. User Stories

#### Visiteur (Grand Public)
1. En tant que **visiteur**, je veux consulter la liste des événements et activités disponibles afin de savoir quelles activités sont proposées par le Circographe.
2. En tant que **visiteur**, je veux accéder aux informations sur l'équipe pour mieux comprendre qui anime les activités et le fonctionnement du Circographe.
3. En tant que **visiteur**, je veux pouvoir vérifier les horaires d'ouverture mis à jour pour planifier ma visite en fonction des disponibilités du lieu.
4. En tant que **visiteur**, je veux utiliser un formulaire de contact pour faire une demande de résidence artistique ou de location de salle.

#### Membres de l’Association (Administrateurs)
1. En tant qu'**administrateur**, je veux créer et mettre à jour les événements afin de maintenir un calendrier précis et à jour pour les participants.
2. En tant qu'**administrateur**, je veux consulter, ajouter et mettre à jour la liste des membres, incluant leurs noms, prénoms et état d'adhésion, pour m'assurer que tous les participants sont en règle.
3. En tant qu'**administrateur**, je veux pouvoir modifier les horaires en fonction des disponibilités des bénévoles pour garantir une bonne gestion du lieu.
4. En tant qu'**administrateur**, je veux suivre la présence des pratiquants de cirque pour pouvoir gérer les entrées et les présences de manière organisée.
5. En tant qu'**administrateur**, je veux administrer les paiements des séances de cirque via l'API SumUp pour gérer facilement les transactions financières.
6. En tant qu'**administrateur**, je veux consulter les statistiques de fréquentation afin d'analyser l'engagement et ajuster les activités en conséquence.


## 3. Concrètement et techniquement

### 3.1. Base de données
- **Tables principales** : Utilisateurs, événements, adhérents, inscriptions, résidences, présences, abonnements, tâches.
- **Relations clés** : Les utilisateurs (rôles : visiteur, administrateur) sont liés aux événements (inscriptions), aux adhérents (suivi de l'abonnement), et aux tâches (tableau de tâches pour l'équipe administrative).

### 3.2. Frontend
- **Composants UI** : 
   - **Accueil** : Présentation du Circographe avec sections pour les événements, les activités (entraînements libres, résidences, stages) sous forme d'agenda ?  Les informations pratiques.
   - **Page Équipe** : Affiche les membres et partenaires principaux de l’association.
   - **Page Contact/Location de salle** : Formulaire de contact pour les demandes de location de salle.
- **Javascript + rails 8** : Utilisation pour les notifications push et la gestion dynamique des réservations et horaires.

### 3.3. Backend
- **Framework** : Ruby on Rails 8
- **API** : Intégration de SumUp pour les paiements, SumUp pour la gestion des paiements ponctuels, et Active Storage (selon rails 8) pour le stockage d'images et de documents.
- **Notifications** : Configuration d’un système de mail pour les nouveaux inscrits et notifications push pour les horaires d'ouverture.

### 3.4. Mes besoins techniques
Je me charge de la configuration du backend en Rails et de la structure de base de données. Pour compléter l’équipe, j’aurai besoin de 3-4 personnes avec des compétences en :
   - **Frontend** (CSS avec Tailwind, JS pour les notifications push)
   - **Design** (UI/UX pour une bonne expérience utilisateur)
   - **Gestion des bases de données** et analyse
   - **API et intégration de paiements**

## 4. La version minimaliste mais fonctionnelle qu'il faut avoir livrée la première semaine

Pour le MVP, l’objectif est d’avoir une version fonctionnelle avec les fonctionnalités de base :
- **Accueil public** : Affichage des événements et informations de contact.
- **Dashboard basique pour les administrateurs** : Gestion simplifiée des événements et de la liste des membres.
- **Système de réservation** : Fonction de réservation sans paiement pour un événement.
- **Notifications** : Envoi d’emails aux nouveaux inscrits.

## 5. La version que l'on présentera aux jury

Pour la version finale, des fonctionnalités avancées seront ajoutées pour une expérience utilisateur complète :
- **Gestion des abonnements et des présences** : Système de suivi des inscriptions et des abonnements (annuels, carnets de 10).
- **Possibilité de nourrir la base de données depuis des formulaires pour effectuer la migration de papier vers numérique.
- **Analyses et statistiques** : Dashboard analytique pour la fréquentation des événements.
- **Interactivité** : Notifications push pour les horaires d'ouverture et newsletters automatiques.

## 6. Notre mentor

**Mentor** : Hadrien Samouillan

######################################################################################################################################

Rejoindre ce projet, c'est bien plus que coder ; c'est faire partie d'une aventure artistique et sociale unique ! En collaborant avec nous, vous allez contribuer à créer une plateforme web pour **le Circographe**, un lieu de création et de pratique artistique au cœur de Toulouse. Voici pourquoi ce projet mérite toute votre attention :

#### Impact réel et utilité sociale
Ce projet va **réellement aider une communauté artistique** : le Circographe est un espace de création et de diffusion des arts du cirque et des arts urbains. Votre code permettra aux artistes, aux bénévoles et au public de mieux interagir, de suivre les événements et de s’inscrire plus facilement. Vous allez pouvoir voir concrètement l’impact de votre travail et contribuer à faire rayonner un espace culturel !

#### Une expérience technique riche et complète
Ce projet offre une occasion unique de toucher à **tous les aspects du développement fullstack** :
- **Backend Ruby on Rails 8** : Pour ceux qui veulent approfondir leurs compétences backend.
- **Gestion de base de données avancée** : Un système avec des tables relationnelles pour les adhérents, événements, abonnements, etc., parfait pour ceux qui souhaitent se plonger dans une logique de gestion complexe.
- **Frontend et design UX/UI** : Ce projet nécessite un design attrayant et fonctionnel, optimisé pour mobile et desktop.
- **API et paiements** : En intégrant des solutions comme **Stripe** et **SumUp**, vous aurez une expérience pratique d’intégration de paiements en ligne, indispensable pour tout développeur moderne.

#### Un produit fini et présentable
Nous allons livrer un **site complet, fonctionnel et présentable**. C’est un projet que vous pourrez montrer fièrement à des employeurs ou utiliser comme référence sur votre portfolio. Ce n’est pas juste un exercice de code : c’est un produit avec des utilisateurs réels et des retours immédiats.

#### Une expérience collaborative et formatrice
Travailler en équipe sur un projet complet est une des meilleures façons de progresser. Que vous soyez plutôt orienté backend, frontend ou devOps, il y a une place pour vous et vos compétences ici ! De plus, le projet implique des rôles définis et une organisation structurée, idéale pour expérimenter la collaboration en développement fullstack.
