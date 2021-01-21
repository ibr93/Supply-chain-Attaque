# INTRODUCTION

En début décembre 2020, IBM fait une étrange découverte : les supply chain mises en place pour distribuer les vaccins contre le COVID-19 font l’objet de cyber-attaques. 

# Qu’est ce que l’attaque par Supply chain ?

La supply chain est une cyber-attaque qui se déroule en 02 phases. La première phase vise les prestataires de services et bureaux d’études informatique. La seconde phase, quant à elle, consiste à intégrer le système d'information des clients consommateurs de ses services. Les approches diffèrent selon les groupes d’attaquants qui sont entre autres le groupe CLOUD HOPPER et Shadow Hammer. 

# Les Stratégies d’attaque par Supply Chain

**1. Les approches du groupe Cloud Hopper**

Le groupe Cloud Hopper cible les grands fournisseurs de services pour les grandes entreprises. La finalité de leurs attaques (cible réel) ne sont pas les tiers fournisseurs de service informatique mais plutôt les entreprises consommatrices de ces services. Pour mener à bien leur programme malveillant, Cloud Hopper s’introduit dans le système du fournisseur via : 

- Credential stuffing qui est une pratique visant à utiliser les identifiants volés d’un compte pour accéder de manière automatique à plusieurs comptes sur divers sites (ex : serveur Web mal sécurisé, bourrage d’identifiant , scan du réseau via des outils comme **Acunetix**…) ;

- Escalade de privilèges à l’aide d’outils légitimes tels que **ProcDump** ou **Certmig** qui facilite la prise en main du système le réseau du fournisseur ;

- Création d’une persistance via la réutilisation d’un ou plusieurs comptes VPNs légitimes de l’entreprises ou des réseaux d’anonymisation TOR afin de faciliter un retour aux systèmes ;

-  Découverte réseau ou recherche des cibles via des outils comme **Netscan**, **WMI Exec**. Ces exemples d’outils permettent d’énumérer les attaques qui peuvent réussir sur le système et donne une idée du système d’exploitation utilisé sur la machine distante.

- Accès et vol des donnés sensible via des déplacements entre le système du fournisseur et la cible réelle ;
-  Transfert légitime des données volées du système du client vers le système du fournisseur ou dans le pire des cas une exfiltration directe des données.

**2. Les approches du groupe Shadow Hammer**

L’approche du groupe Shadow Hammer est une approche plus opportuniste. Le groupe crée des attaques diffuses pour une infime machine ciblée. Ce qui s’est révélé en particulier en mars 2019 avec l’attaque qui a touché le fabricant de matérielle informatique ASUS. En particulier le logiciel **Asus Live Updater.**  Ce groupe a réussi à accéder aux certificats d’Asus et injecter du code malveillant dans le logiciel d’ASUS. Cette attaque à touché des milliers de machines toutefois, environ 600 adresses MAC étaient ciblé. Asus n’est pas la seule firme victime de leur attaque malicieuse. Asus n’est pas la seule firme victime de l’approche Shadow Hammer. Nous pouvons citer entre autres le logiciel CCleaner (40 machines infectées pour 700 000 machines touchées) en 2017 et les éditeurs de jeux vidéo asiatiques Electronic Extreme et Zepetto (compromission de la chaîne de développement et installation de backdoors sans plusieurs jeux vidéo) en 2019.

# Conclusion
Nous pouvons constaté qu'un point commun entre les types d'attaque par Supply chain est l'utilisation des fournisseurs de services informatiques afin de nuire aux systèmes consommateurs de ces services. Ce qui nous emmène à nous demander si on peut réellement faire confiance aux fournisseurs de services ?