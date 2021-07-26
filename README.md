# CYBERLAB OWASP-MUTILLIDAE
23.07.2021

Nabil Kerour

Simplon.CO
__________
Mise en place de l'environnement de **pentest**

**OBJECTIF**

Préparer une démo d’un POC MUTILLIDAE OWASP.

Sur un LAPTOP sous Windows 10 avec un VM fonctionnelle sous Linux (Ubuntu), le POC devra être réalisé est validé devant les collègues du CERT.

Site Mutillidae sous LAMP.

Créer une documentation technique en Markdown sur le dépôt GitHub. 

**Etapes détailler a suivre**

1 Installer une VM Ubuntu dans Virtualbox.

>https://www.ubuntu-fr.org/download/< 

Mettre à jour Ubuntu une fois la VM démarrée, pour cela lancer le terminal pour passer en mode console une fois l'installation de Ubuntu terminée et entrée les commandes suivantes:

 sudo apt-get update pour rechercher les mises à jours
 
 sudo apt install pour les installées.

2  Installer les ajouts d'invité VirtualBox
sur Ubuntu.

Installer pour ceux faire via le terminal [gcc,make,perl] avec la commande:

 sudo apt install gcc make perl, ensuite sélection dans périphérique l'image du cd des ajout invité et lancer l'installation en automatique. 

3  Installer le serveur Web Apache

Lancer le terminal et faite la commande suivante:

sudo apt install apache2

4 Installer PHP

Lancer le terminal et faite la commande suivante:

sudo apt install php

5 Installer MariaDB

Lancer le terminal et faite la commande suivante:

sudo apt install mariadb

6 Installer Mutillidae

Lancer le terminal et faite la commande suivante:

cd /var/www/html/ qui vous permet d'etre sur le dossier ou sera déposé le fichier et taper la ligne suivante:

*git clone https://git.code.sf.net/p/mutillidae/git mutillidae*

Vous pouvez à présent aller sur le navigateur web et lancer dans la barre de recherche le site en tapant:

**localhost/mutillidae**

![mutillidae]
(Screenshot 2021-07-26 at 07-54-57 Screenshot.png)