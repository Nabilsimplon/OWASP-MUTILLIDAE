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

* 1 Installer une VM Ubuntu dans Virtualbox.

>https://www.ubuntu-fr.org/download/< 

Mettre à jour Ubuntu une fois la VM démarrée, pour cela lancer le terminal pour passer en mode console une fois l'installation de Ubuntu terminée et entrée les commandes suivantes:

sudo -s pour la fonction Administrateur jusqu'a la prochaine fermeture du terminal!

 apt-get update pour rechercher les mises à jours
 
 apt-get upgrade pour les installées.

* 2  Installer les ajouts d'invité VirtualBox
sur Ubuntu.

Installer pour ceux faire via le terminal [gcc,make,perl] avec la commande:

 apt install gcc make perl, ensuite sélectionné l'onglet périphérique l'image du cd des ajouts d'invité et lancer l'installation en automatique. 

* 3  Installer le serveur Web Apache

apt install apache2

* 4 Installer PHP

apt install php

apt install php libapache2-mod-php php-mysql

* 5 Installer MariaDB

apt install mariadb-server

mysql_secure_installation pour changer le mot de passe 

* 6 Installer Mutillidae

On va aller dans le dossier ou déposer le fichier avant en tapant via le terminal:

cd /var/www/html/ et taper la ligne suivante pour installer Mutillidae:

*git clone https://git.code.sf.net/p/mutillidae/git mutillidae*

Vous pouvez à présent aller sur le navigateur web et lancer dans la barre de recherche le site en tapant:

**localhost/mutillidae**

Penser a restart les services mysql apache2 en tapant via le terminal service (....) restart

Pour vérifier l'etat de fonctionnement des services la commande **services --status** le + indique que un service et actif et - le service et inactif.

Merci d'avoir suivi cette doc redigée en MARKDOWN toutes remarques ou appreciations et la Bienvenue.

! (C:\Users\utilisateur\Pictures\download.jpg)
'''
p
{
    color:blue;
}
'''
