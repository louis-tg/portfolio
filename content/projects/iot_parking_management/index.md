+++
title = "IoT parking management"
description = "IoT parking system prototype"
weight = 2
date = 2026-01-01

[extra]
local_image = "iot_parking_management/archi_dark.png"
github = "https://github.com/lasercata/iot_parking_management"
demo = "https://iot.lasercata.com/"
tags = ["iot", "python", "flask", "mqtt", "mongoDB"]
+++

A prototype of an automatic **parking control system** dedicated to people with disabilities.

Each parking spot is equipped with an IoT node, that detects car presence and reads user's authentication card.
The user can reserve a parking sport up to one hour in advance, via a secure web interface.
The backend, called *IoT platform*, links nodes with the user interface and implements the core logic.

## Architecture
![Project architecture](archi_dark.png)

## Showcase
### User
This is the homepage for a regular user:
![User homepage](web_interface/user_home.webp)

And this it the reservation tab:
![User reservation tab](web_interface/user_reservations.webp)

### Administrator
This is the homepage for administrators:
![Admin homepage](web_interface/admin_home.webp)

Administrators can manage nodes:
![Admin nodes tab](web_interface/admin_nodes.webp)
![Admin node creation](web_interface/admin_nodes_creation.webp)

They can also manage users:
![Admin users tab](web_interface/admin_users.webp)
![Admin user creation](web_interface/admin_users_creation.webp)

When an administrator creates an account, the user will receive an email with a temporary code:
![User creation email](web_interface/mail_account_creation.webp)
