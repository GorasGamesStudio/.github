# Projets du studio

## K4rant : The Arcade Rift

Plateforme VR et PC (Steam, Meta Quest) : lobby multijoueur et jeux d'arcade à seed déterministe, avec classements.

- Moteur : Unity 6, URP, C#
- VR : XR Interaction Toolkit, OpenXR
- Réseau : Netcode for GameObjects, Unity Multiplayer Services
- Chargement : Addressables
- Procédural : seed déterministe via Unity.Mathematics.Random, partageable entre joueurs
- Jeux au lancement : Candypede (défense de tour en vue à la première personne, coop à deux) et The Maze Protocol (labyrinthe procédural, escape game)
- Versionnage : Unity Version Control (Plastic SCM)

Stade : prototypage et game design.

## Commercial Street

Jeu de gestion commerciale multijoueur, dans un monde réunissant plusieurs types de commerces : le joueur loue ou achète un espace et exploite des licences de magasin.

- Moteur : Unity

Stade : game design.

## PartyHospital

Party game coopératif en ligne, à la première personne, jusqu'à 8 joueurs sur PC. Architecture séparant les gestes (six familles de défis écrites une fois) du contenu (maladies, rôles, dialogues), défini en données.

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
