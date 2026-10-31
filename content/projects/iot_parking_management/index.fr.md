+++
title = "IoT parking management"
description = "Prototype de gestion de parking IoT"
weight = 2
date = 2026-02-18

[extra]
local_image = "/content/projects/iot_parking_management/archi_dark.png"
github = "https://github.com/github.com/iot_parking_management"
demo = "https://iot.lasercata.com/"
tags = ["iot", "python", "flask", "mqtt", "mongoDB"]
+++

Un prototype de système automatique de contrôle du stationnement, dédié aux personnes handicapées.

Chaque place de parking PMR est équipée d'un nœud IoT, qui détecte la présence d'une voiture et lit la carte d'authentification de l'utilisateur.
Il est possible de réserver une place jusqu'à une heure en avance, via une interface web sécurisée.
Le backend, appelé *IoT platform*, relie les nœuds à l'interface utilisateur et met en œuvre la logique de base.

## Architecture
![Architecture du projet](archi_dark.png)

## Interface web
### Utilisateur
Voici la page d'accueil pour un utilisateur :
![User homepage](web_interface/user_home.webp)

L'onglet pour réserver une place se présente comme suit :
![User reservation tab](web_interface/user_reservations.webp)

### Administrateur
Voici la page d'accueil d'un administrateur :
![Admin homepage](web_interface/admin_home.webp)

Les administrateurs peuvent gérer les nœuds :
![Admin nodes tab](web_interface/admin_nodes.webp)
![Admin node creation](web_interface/admin_nodes_creation.webp)

Ils peuvent aussi gérer les utilisateurs :
![Admin users tab](web_interface/admin_users.webp)
![Admin user creation](web_interface/admin_users_creation.webp)

Lorsqu'un administrateur crée un compte, l'utilisateur concerné reçoit un e-mail avec un code temporaire :
![User creation email](web_interface/mail_account_creation.webp)
