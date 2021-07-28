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

**DEFINITION**

*Présentation d'OWASP*

[OWASP](image/téléchargement.htm)

>https://www.owasp.org/

1 La communauté OWASP (Open Web Application Security project) est une communauté travaillant sur la sécurité des
applications web. Elle a pour but de publier des recommandations de sécurisation des sites web et
propose des outils permettant de tester la sécurité des applications web.

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

[Apache](image/téléchargement2.png)

Apache est conçu pour prendre en charge de nombreux modules lui donnant des fonctionnalités supplémentaires : interprétation du langage Perl, PHP, Python et Ruby, serveur proxy, Common Gateway Interface, Server Side Includes, réécriture d'URL, négociation de contenu, protocoles de communication additionnels, etc. Néanmoins, il est à noter que l'existence de nombreux modules Apache complexifie la configuration du serveur web. En effet, les bonnes pratiques recommandent de ne charger que les modules utiles : de nombreuses failles de sécurité affectant uniquement les modules d'Apache sont régulièrement découvertes.

Lancer le terminal et taper: apt install apache2

On doit retrouver via le navigateur en tapant (localhost)

[Résultat](téléchargement2.png)

* 4 Installer PHP

[PHP](image/téléchargement3.jpg)

PHP: Hypertext Preprocessor19, plus connu sous son sigle PHP (sigle auto-référentiel), est un langage de programmation libre20, principalement utilisé pour produire des pages Web dynamiques via un serveur HTTP19, mais pouvant également fonctionner comme n'importe quel langage interprété de façon locale. PHP est un langage impératif orienté objet.

PHP a permis de créer un grand nombre de sites web célèbres, comme Facebook et Wikipédia21. Il est considéré comme une des bases de la création de sites web dits dynamiques mais également des applications web.

ouvrir le terminal et taper: apt install php

apt install php libapache2-mod-php php-mysql

* 5 Installer MariaDB

[MARIADB](image/téléchargement.jpg)

En 2009, à la suite du rachat de MySQL par Sun Microsystems et des annonces du rachat de Sun Microsystems par Oracle Corporation, Michael Widenius, fondateur de MySQL, quitte cette société6 pour lancer le projet MariaDB, dans une démarche visant à remplacer MySQL tout en assurant l’interopérabilité. Le nom vient de la 2e fille de Michael Widenius, Maria (la première s'appelant My).

Lancer le terminal et taper: apt install mariadb-server.

taper: (mysql_secure_installation) pour changer le mot de passe. 

* 6 Installer Mutillidae

[Mutillidae](image/06.jpg)

On va aller dans le dossier ou déposer le fichier avant en tapant via le terminal:

cd /var/www/html/ et taper la ligne suivante pour installer Mutillidae:

*git clone https://git.code.sf.net/p/mutillidae/git mutillidae*

Vous pouvez à présent aller sur le navigateur web et lancer dans la barre de recherche le site en tapant:

**localhost/mutillidae**

Penser a restart les services mysql apache2 en tapant via le terminal service (....) restart
 
Pour vérifier l'etat de fonctionnement des services la commande **services --status** le + indique que un service et actif et - le service et inactif.

* 7 GITHUB
  
[GITHUB](image/téléchargement4.png)

  Utiliser une plateforme de projet collaboratif pour déposer la documentation technique.  

Git et un language,une techno.

Merci d'avoir suivi cette doc redigée en **MARKDOWN** toutes remarques ou appreciations et la Bienvenue.

