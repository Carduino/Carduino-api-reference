---
title: Carduino Docs

language_tabs:
  - bash
  - ruby
  - python

toc_footers:
  - <a href='http://carduino.dauliac.fr'>Carduino App</a>
  - <a href='http://docs.dauliac.fr'>Carduino Docs</a>
  - <a href='https://github.com/Carduino'>GitHub</a>
  - <a href='http://www.estia.fr'>Site officiel ESTIA</a>

includes:
  - errors

search: true
---

# Introduction

<img src='images/logo-complet.png' alt='Logo Carduino' />



### Carduino - Réseaux de capteurs communiquants

Carduino est le fruit d'un projet d'étudiants ingénieurs de l'[ESTIA](http://www.estia.fr) (École Supérieure des Technologie Industrielles Avancées). Il s'agit d'un démonstrateur, témoin du savoir-faire et des compétences des étudiants et des enseignants de l'ESTIA en matière d'éléctronique, d'informatique et de systèmes embarqués. Au delà de cela, il a été conçu de manière à pouvoir être facilement re-utilisé, et modifié, pour prendre part à de futures activités pédagogiques (TP, cours) et de recherche (capteurs autonomes, énergie, collecte de données).

Le projet se décompose en 3 sous systèmes distincs. Le serveur, les concentrateurs, et les capteurs. Cette documentation détaille le fonctionnement logiciel du serveur et des concentrateurs.



# Installation du serveur
## Debian Jessie
### Téléchargement de l'image de Debian

1. [Télécharger l'image iso de Debian Jessie (8.3)](http://cdimage.debian.org/debian-cd/8.3.0/amd64/iso-cd/debian-8.3.0-amd64-netinst.iso)
2. Lancer l'image iso et suivre le processus d'installation.
3. Mettre le système à jour.
3. Activer la connexion SSH si elle n'est pas déjà activée
4. Installer Vim s'il n'est pas présent

<aside class="warning">Pensez à bien noter le mot de passe root du système !</aside>



## Installation de Git
> mise à jour de la liste des packages puis Installation de Git avec apt-get

```bash
	sudo apt-get update
	sudo apt-get install git-core
```
Installation de Git via apt-get.
Assurez vous que la liste des packages du système est bien à jour, puis installez Git.

<aside class="notice">Git est nécessaire pour l'installation, la gestion de version, et le déploiement des mises à jour du serveur Carduino.</aside>



## Configuration minimale de Git
> Définir le username de Git

```bash
	git config --global user.name "Vôtre nom"
```
>Définir l'email de Git

```bash
	git config --global user.email sammy@example.com
```
Git implémente la gestion de version à partir de deux paramètres pricipaux.

Ces informations se retrouveront dans chaque commit que vous ferez avec Git, qui pourra donc identifier qui a fait quels commits.

<br />

Paramètre | Description
--------- | -----------
user.name | Un nom d'utilisateur
user.email | L'email de l'utilisateur



## Installation de MongoDB
>Ajouter les keys MongoDB pour que le système reconnaisse les packages signés par MongoDB et leur fasse confiance.

```bash
	sudo apt-key adv --keyserver keyserver.ubuntu.com --recv 7F0CEB10  
```

>Ajout de leur dépot aux sources du système.

```bash
	echo "deb http://repo.mongodb.org/apt/debian wheezy/mongodb-org/3.2 main" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.0.list
```

> mise à jour de la liste des packages puis Installation de MongoDB avec apt-get

```bash
	sudo apt-get update
	sudo apt-get install mongodb-org -y
```
Installation en utilisant le dépot apt MongoDB.

Cette méthode permet au système de recevoir la dernière version de MongoDB considérée stable par la team MongoDB.

Si vous voulez supprimer le dépot Mongo DB des sources de votre système par la suite, supprimer simplement le fichier suivant :
`/etc/apt/sources.list.d/mongodb-org-3.0.list`



## Configuration de MongoDB
<aside class="warning">Attention, la configuration de MongoDB est une étape cruciale et très sensible !</aside>




## Node.js
### Installation de Curl
### Installation de Node.js



## Carduino
### Clonage du repository
### Installation
### Lancement

# Installation concentrateur
## Raspbian
## Git
## Node.js
## Carduino



# Configuration



# Authentification



# Interface Web



# API Serveur



# API Concentrateur
