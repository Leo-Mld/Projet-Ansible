Exam Ansible

Elaboration d'un Playbook Ansible pour construire un environnement LAMP.

Prérequis:
 - Construire deux containers avec le port 80 et 3306
 - S'assurer de la bonne connexion avec Ansible
 - Vous allez créer un playbook qui fait appel à 3 roles Apache, Php et Mysql distincts.
 - Ces rôles devront installés le service avec un compte de service.

Elements globaux:
 - Il devra effectuer l'installation de chaque brique si l'OS est un Ubuntu 18.04
 - Les services Apache, Php et Mysql seront Up et fonctionnel
 - Faire un check via Ansible

Apache:
 - Assurer vous qu'apache est bien installer
 - Copier le fichier de configuration apache2.conf
 - Lorsque le fichier change, redémarrer à l'aide d'un handlers le service Apache

PHP:
 - Modifier le fichier index.php avec une variable contenant votre prénom


MySQL:
 - Créer une base de donnée, en variabilisant le nom de cette base dans vos fichiers de variables
 - Créer un utilisateur root avec un password ( encrypté dans un fichier )
 - Créer deux utilisateurs ayant les droits sur la base de donnée