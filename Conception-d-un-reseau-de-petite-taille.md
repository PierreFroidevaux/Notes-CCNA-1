# Chapitre 11 : Conception d'un réseau de petite taille

Pour faire évoluer un réseau, plusieurs éléments sont nécessaires :

Documentation réseau : topologie physique et logique
Inventaire des équipements : liste des terminaux qui utilisent ou constituent le réseau 
Budget : budget IT détaillé comprenant le budget annuel alloué à l'achat du matériel
Analyse du trafic : les protocoles, les applications et les services, ainsi que leurs besoins respectifs en termes de trafic doivent être documentés





Bloquer les tentatives de connexion sur RouterA pendant 30 secondes si 2 tentatives de connexion sont infructueuses en 10 secondes
  RouterA(config)# login block-for 30 attempts 2 within 10





Les indicateurs les plus courants d'une requête ping envoyée par Cisco IOS sont « ! », « . » et « U ». 
Le point d'exclamation (!) indique que la requête ping a réussi et vérifié la connectivité au niveau de la couche 3. 
Le point (.) peut indiquer un problème de connectivité, un problème de routage ou un problème de sécurité du périphérique sur le chemin et qu'un message ICMP d'inaccessibilité de la destination n'a pas été envoyé. 
La lettre « U » indique qu'un routeur situé sur le chemin ne possède vraisemblablement pas de route vers l'adresse de destination et a envoyé un message ICMP d'inaccessibilité de la destination.



Les délais d'attente d'exécution permettent au périphérique Cisco de déconnecter automatiquement les utilisateurs lorsqu'ils sont inactifs pendant la période indiquée. Des délais d'attente d'exécution peuvent être configurés pour la console, l'interface VTY et les ports auxiliaires.








Chapitre 11 : Conception d'un réseau de petite taille
Pour répondre aux besoins des utilisateurs, même les réseaux de petite taille doivent faire l'objet d'une planification et d'une conception. La planification garantit que tous les besoins, les facteurs de coûts et les options de déploiement sont pris en compte. La fiabilité, l'évolutivité et la disponibilité sont des aspects essentiels de la conception d'un réseau.

La prise en charge et le développement d'un petit réseau requièrent une bonne connaissance des protocoles et des applications de réseau exécutés sur le réseau concerné. Les analyseurs de protocoles permettent à un professionnel des réseaux de compiler rapidement des données statistiques à propos des flux de trafic sur un réseau. Les informations collectées par l'analyseur de protocole sont évaluées en fonction de la source et de la destination du trafic, ainsi que du type de trafic envoyé. L'analyse peut ensuite être utilisée par un technicien réseau pour déterminer comment améliorer la gestion du trafic. Les protocoles réseau les plus courants sont les suivants : DNS, Telnet, SMTP, POP, DHCP, HTTP et FTP.

Lors de la planification de la mise en œuvre d'un réseau, il est indispensable de tenir compte des menaces et des failles de sécurité potentielles. Tous les périphériques du réseau doivent être sécurisés. Cela inclut les routeurs, les commutateurs, les périphériques des utilisateurs finaux et même les dispositifs de sécurité. Les réseaux doivent être protégés contre les logiciels malveillants tels que les virus, les chevaux de Troie et les vers. Les logiciels antivirus peuvent détecter la plupart des virus et des chevaux de Troie et les empêcher de se propager dans le réseau. La meilleure façon de limiter les risques d'attaque de ver est de télécharger les mises à jour de sécurité du fournisseur du système d'exploitation et d'appliquer des correctifs sur tous les systèmes vulnérables.

Les réseaux doivent également être protégés contre les attaques de réseau. Celles-ci peuvent être classées en trois catégories principales : les attaques de reconnaissance, les attaques par accès et les attaques par déni de service. Plusieurs méthodes permettent de protéger un réseau contre les attaques.

Les services de sécurité réseau d'authentification, d'autorisation et de gestion des comptes fournissent la structure principale permettant de mettre en place un contrôle d'accès sur un périphérique réseau. Ces services permettent de contrôler les utilisateurs autorisés à accéder à un réseau (authentification), ce que ces derniers peuvent faire lorsqu'ils sont connectés (autorisation) et les actions qu'ils exécutent lors de l'accès au réseau (gestion des comptes).
Un pare-feu est l'un des outils de sécurité les plus efficaces pour protéger les utilisateurs internes du réseau contre les menaces externes. Un pare-feu se trouve entre deux réseaux, ou plus, et contrôle le trafic entre eux tout en contribuant à interdire les accès non autorisés.
Pour protéger les périphériques réseau, il est important d'utiliser des mots de passe forts. En outre, si des périphériques réseau font l'objet d'un accès à distance, il est vivement recommandé d'activer SSH à la place du protocole Telnet non sécurisé.
Après la mise en œuvre du réseau, l'administrateur doit être en mesure de le contrôler et d'assurer sa connectivité. Plusieurs commandes permettent d'y parvenir. Pour tester la connectivité réseau à des destinations locales et distantes, on utilise généralement des commandes telles que ping, telnet et traceroute.

Sur les périphériques Cisco IOS, la commande show version peut être utilisée pour vérifier et dépanner certains composants matériels et logiciels de base utilisés lors du processus de démarrage. Pour afficher des informations relatives à toutes les interfaces réseau d'un routeur, on utilise la commande show ip interface. La commande show ip interface brief permet d'afficher un résultat plus abrégé que la commande show ip interface. CDP (Cisco Discovery Protocol) est un protocole propriétaire de Cisco qui s'exécute au niveau de la couche liaison de données. Puisque le protocole CDP fonctionne au niveau de la couche liaison de données, deux périphériques réseau Cisco ou plus, tels que des routeurs prenant en charge différents protocoles de couche réseau, peuvent échanger des informations même si la connectivité de couche 3 n'existe pas.

Les fichiers de configuration Cisco IOS tels que startup-config (configuration de démarrage) et running-config (configuration en cours) doivent être archivés. Ils peuvent être enregistrés dans un fichier texte ou être stockés sur un serveur TFTP. Certains modèles de routeur possèdent également un port USB et permettent ainsi de sauvegarder les fichiers sur un périphérique de stockage USB. Si nécessaire, ces fichiers peuvent être copiés vers le routeur ou le commutateur à partir du serveur TFTP ou du périphérique USB.

The figure is a standard graphic for the introduction and conclusion pages.
