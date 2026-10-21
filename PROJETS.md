# Projets du studio

## K4rant : The Arcade Rift

Salle d'arcade sociale sur PC et VR (Steam, Meta Quest). Un lobby en forme de grand dôme où chaque borne géante ouvre sur un jeu, avec salons et mini-jeux de kermesse pour gagner des jetons.

Deux jeux au lancement :

- Candypede, inspiré de Centipede : vue 3D à la première personne sur une tour centrale. Il faut défendre un terrain circulaire contre un mille-pattes qui se divise à chaque impact. Obstacles (chamallow, caramel) et bonus tous les X vagues. Solo ou coop à deux sur un rail partagé.
- The Maze Protocol, inspiré de Cube : labyrinthe procédural qui se réorganise en permanence, escape game avec timer dégressif, secrets qui rapportent du temps ou du score. Une IA narratrice accompagne le joueur. Niveaux infinis enchaînés avec multiplicateur. Solo ou coop à deux.

Systèmes transversaux : seed déterministe partageable entre joueurs, progression intra-partie sans amélioration permanente (skill pur), classements quotidien, mensuel et All-Time.

- Moteur : Unity 6, URP, C#
- VR : XR Interaction Toolkit, OpenXR
- Réseau : Netcode for GameObjects, Unity Multiplayer Services
- Chargement : Addressables
- Procédural : seed déterministe via Unity.Mathematics.Random, partageable entre joueurs
- Versionnage : Unity Version Control (Plastic SCM)

Stade : prototypage et game design.

## Commercial Street

Jeu de gestion commerciale multijoueur qui réunit dans un même monde les simulateurs de gestion existants : supermarché, restaurant, casino, et bien d'autres.

Le joueur arrive avec un budget, loue ou achète un espace, et l'exploite comme il le souhaite grâce à des licences de magasin : il choisit le type de commerce, ce qu'il vend et comment il le gère. Les joueurs se fournissent et se rendent service entre eux (nourriture, boissons, courses, immobilier, jeux). Chacun doit aussi se nourrir, se reposer et s'habiller.

Le monde se partage entre amis, avec une mécanique sociale en plus de la gestion. On peut devenir riche ou faire faillite.

- Moteur : Unity

Stade : game design.

## PartyHospital

Party game coopératif en ligne, à la première personne, jusqu'à 8 joueurs sur PC. Chacun tient un poste (accueil, consultation, analyses, traitement, chirurgie) et enchaîne des défis courts sous pression : enregistrer un patient, l'examiner, passer une radio, analyser un prélèvement, doser un médicament, opérer, faire payer.

Principe central : un patient bien soigné part et ne revient pas ; mal soigné, il revient et repaie. Rater n'est pas perdre, c'est un modèle d'affaires.

À la fin de chaque journée, l'hôpital reste ouvert s'il franchit l'un des deux seuils, qualité des soins ou rentabilité. Le milieu est la seule zone mortelle, et les seuils montent chaque jour, annoncés par le ministère.

Quatre événements perturbent la journée : coupure de courant, panne du réseau pneumatique, inspection surprise, afflux de patients.

Architecture : six familles de défis écrites une fois. Maladies, rôles et patients sont des données, ce qui permet d'ajouter du contenu sans réécrire le code.

- Moteur : Unity 6, URP
- Réseau : Netcode for GameObjects
- Prototype d'équilibrage : simulation C# déterministe d'une journée de jeu, sans moteur, avec replay HTML (.NET 8), dans un dépôt séparé

Stade : pré-production, design avancé ; prototype jouable non commencé.

## GGS-Core

Package Unity commun à tous les projets du studio (`com.ggs.core`) : mise en place du projet, chargement avec écran de masque, navigation par clés de scène.

- Moteur : Unity, C#

## Unasso (anciennement AssoPilot)

Gestion d'association (loi 1901) : événements, membres, finances, matériel et boutique. Une base de données par association, avec des modules qui alimentent les autres (achat reçu créant l'objet d'inventaire et la dépense).

- Backend : .NET 8, Blazor Server, Entity Framework Core
- Base : PostgreSQL, une base par association

Stade : en développement, site de présentation en relecture.

## Pockyt

Gestion de budget personnel multi-comptes, avec prévisionnel du solde jour après jour (3 mois en gratuit, 12 mois en Pockyt+) et budgets par catégorie.

- Monorepo : Turborepo
- Backend : NestJS, TypeScript, PostgreSQL
- Front : Next.js (web), React Native / Expo (mobile)
- Hébergement : OVH, Union européenne

Stade : bêta sur invitation.
