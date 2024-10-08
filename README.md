# LITReview

LITReview est une application web Django qui permet aux utilisateurs de demander et de publier des critiques de livres ou d'articles. Elle offre une plateforme sociale où les utilisateurs peuvent interagir en créant des billets, en écrivant des critiques et en suivant d'autres utilisateurs pour voir leur contenu dans leur flux personnalisé.

## Table des matières

- [Fonctionnalités](#fonctionnalités)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Utilisation](#utilisation)
  - [1. Créer un compte](#1-créer-un-compte)
  - [2. Se connecter](#2-se-connecter)
  - [3. Naviguer dans l'application](#3-naviguer-dans-lapplication)
- [Conformité à l'accessibilité](#conformité-à-laccessibilité)
- [Auteurs](#auteurs)

## Fonctionnalités

- **Gestion des utilisateurs :**
  - Inscription, connexion et déconnexion sécurisées.
- **Billets (Tickets) :**
  - Création de billets pour demander des critiques sur un livre ou un article.
  - Modification et suppression de ses propres billets.
- **Critiques (Reviews) :**
  - Réponse aux billets en écrivant des critiques.
  - Création de critiques simultanément avec un nouveau billet.
  - Modification et suppression de ses propres critiques.
- **Flux personnalisé :**
  - Affichage des billets et critiques des utilisateurs suivis et de ses propres publications.
  - Tri des publications par ordre chronologique.
- **Suivi des utilisateurs :**
  - Possibilité de suivre d'autres utilisateurs pour voir leur contenu dans le flux.
  - Affichage de la liste des utilisateurs suivis et des abonnés.
- **Accessibilité :**
  - Conformité aux directives du Référentiel Général d'Amélioration de l'Accessibilité (RGAA) pour garantir une expérience utilisateur optimale pour tous.

## Prérequis

- **Python 3.8 ou supérieur**
- **Django 3.2 ou supérieur**
- **pip**
- **Virtualenv** (recommandé)
- **Git** (pour cloner le dépôt, si nécessaire)



## Installation

   **Cloner le dépôt :**

   ```bash
   git clone https://github.com/myrteza-labi/P8.git
   cd P8
   ```


## Créer et activer un environnement virtuel

   **Sous Windows**

    ```bash
    python -m venv env
    env\Scripts\activate
    ```

   **Sous macOS/Linux**

    ```bash
    python3 -m venv env
    source env/bin/activate
    ```

## Installer les dépendances :

    ```bash
    pip install -r requirements.txt
    ```
Note : Si vous n'avez pas de fichier requirements.txt, vous pouvez installer Django directement :

    ```bash
    pip install django
    ```

## Appliquer les migrations :

    ```bash
    python manage.py migrate
    ```

## Lancer le serveur de développement :

    ```bash
    python manage.py runserver
    ```
Le serveur est disponible à l'adresse **http://127.0.0.1:8000/.**


# Utilisation


## Créer un compte :

Accédez à **http://127.0.0.1:8000/signup/** pour créer un nouveau compte utilisateur.
Remplissez le formulaire d'inscription avec un nom d'utilisateur, une adresse e-mail (optionnelle) et un mot de passe.


## Se connecter :

Accédez à **http://127.0.0.1:8000/login/** pour vous connecter avec vos identifiants.
Après la connexion, vous serez redirigé vers votre flux personnalisé.

## Naviguer dans l'application :

**Flux** : Affiche les billets et critiques des utilisateurs que vous suivez ainsi que vos propres publications.

**Créer un billet** : Accédez à "Créer un billet" dans le menu pour demander une nouvelle critique.

**Créer une critique** : Vous pouvez créer une critique en réponse à un billet existant ou créer un billet et une critique simultanément.

**Suivre des utilisateurs** : Utilisez la fonctionnalité "Suivre un utilisateur" pour suivre d'autres membres de la communauté.

**Mes publications** : Consultez et gérez vos propres billets et critiques.

**Déconnexion** : Cliquez sur "Déconnexion" pour vous déconnecter de votre compte.

## Conformité à l'accessibilité

L'application LITReview a été développée en respectant les directives du RGAA pour assurer une accessibilité maximale :

**Structure sémantique** : Utilisation appropriée des balises HTML5.

**Contraste des couleurs** : Choix de couleurs avec un contraste suffisant.

**Textes alternatifs** : Fourniture de textes alternatifs pour les images.

**Navigation clavier** : L'interface est entièrement navigable au clavier.

**Labels associés** : Les champs de formulaires sont correctement associés à leurs labels.

## Auteurs

LABI Myrteza : https://github.com/myrteza-labi
(et dans Myrteza, Il y a : AZERTY)



<!--
///((/((((((((((((((#############################%#%%%%%%%%%%%%%%%%%%%%%%%%%%%%%###%%%%#############################((((
//(((((((((((((((#(#########################%#%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#%%%%#######################((
(((((((((((((((########################%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#%#######################
((((((((((((#######################%%%%%%%%%%%%%%%%%%%%%%%%%%%#(%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#%###################
((((((((((####################%#%%%%%%%%%%%%%%%%%%%%*,.......    ..../#%&%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#################
((((((((#################%##%%%%%%%%%%%%%%%%%%%%#  ..     .,,.  .......,..*&%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#############
(((((((#################%#%%%%%%%%%%%%%%%%%%%%%,         .,.,,,....,,.......(%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#%############
((((################%%%%%%%%%%%%%%%%%%%%%%%%%% .            ....,...,,.,....*&&&&&%%%%%%%%%%%%%%%%%%%%%%%%%%%%##########
((###############%%%%%%%%%%%%%%%%%%%%%%%&%%%,  .   ...                 .... ..#&&&&&&&&&&&%%%%%%%%%%%%%%%%%%%%%#########
((#############%%%%%%%%%%%%%%%%%%%%&&&&&&&%    ...,*//(***/(/,,,,**,..........,&&&&&&&&&&&&%%%%%%%%%%%%%%%%%%%%%########
############%%%%%%%%%%%%%%%%%%%%%&&&&&&&&&....,/(##%%%%&&&&&&&&&&&&&&&%%%##*...&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%%%%%#######
##########%%%%%%%%%%%%%%%%%%%%&&&&&&&&&&&%....*(###%%%%&&&&&&@@@&&&&&&&&&%%%(..#&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%%%%%%#####
#########%%%%#%%%%%%%%%%%%%&&&&&&&&&&&&&&#.,,,*(###%%%%&&&&&&&@@@@&&&&&&&&%%#*,/&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%%%%%%####
#######%%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&(,***(((##%%%&&&&&&&&&&@&&&&&&&%%%%#(/*&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%%%####
######%%%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&(**//((((*/***/#%&&&&@@@@&&&&&&&%%%##//&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%%%%#
#####%%%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&(**////(##%%&%#(((##%%%%%%(//**/((/*/(/&&&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%%%
####%#%%%%%%%%%%%%%&&&%&&&&&&&&&&&&&&&&&&/***/((((*/*,**((/((#%%%#(//(%&%((#(((/&&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%%%%
##%%%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&%((/*/(###(/(#####%##(#%&%##%%#%#(((/##(/%%&&&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%
%#%%%%%%%%%%%%%%%&%&&&&&&&&&&&&&&&&&&&%((//*/(###%%%%%%%%%#(##%%%##%%%%%%%&%%%#(#/&&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%%
###%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&(%#/**/(####%%%%&&%((#%&&&%##%%%&&%%%%%##&#&@&&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%
%#%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&(((/**/((###%%&&&%#//,,((( .##&&&&%%%%#((##&&@@@&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%
#%%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&%#(/,**/((##%%%%%%%%####%##%%%%%%%%%##(/(#&@@@@@&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%
#%%%%%%%%%%%%%%%&%&&&&&&&&&&&&&&&&&&&&&&&&/.,*//((###(//(((##%%&%%#(((((#####(*%&&&&&@&&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%
%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&&&&&&&,.,,*/(#%##(/***//(////(/*/(##%%#/**@&&@@@@@@@@&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%
%%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&&&&&&%.,,****(##################%%%%(**,%&&@@@&@@@@&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%
#%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&&&&&&&&,.,,,***/(((###%%%%%#%%%%###(/**,(&@@@@@@&&&&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%
%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&&&&&&&&%...,,,,,*/*/(##%%%%%%%###(/**,,%&&@@@@@&&&@&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%
##%%%%%%%%%%%%%%%&%&&&&&&&&&&&&&&&&&&&&&&&&&&*,,.,,,.,,****/((((#((//*,,,.,#&&&&@@@@@&&&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%
####%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&&&&&&&&@(/***,,.,,,,.,,,*****,...,,,/(#&@&&@@@@&&&&&&&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%
##%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&&&&&@@@&////**,,,...,,,,,,,..,,**/(#/@&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&%&&%%%%%%%%
###%%%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&&&&&&@@@@@@@@&((((//****//////////(((###&@@@&&&&@&&&&&&&&&&&&&&&&&&&&&&&&&%&%%%%%%%%
#####%%%%%%%%%%%%%%%&&&&&&&&&&&&&&&&@@&@@@@&@@@@@@@@@####(((((((((########/%&@@@@@@@@@&&&&&&&&&&&&&&&&&&&&&&%%%%%%%%%%%%
######%#%%%%%%%%%%%%%%&&&&&&&&&&@@@@@@@@@@&&@@@@@@@@@@@@%###%%%%%%###%%##(*&&@@@@@@@@@@@@@@@&&&&&&&&&&&&&&&&%%%%%%%%%%%%
######%%%%%%%%%%%%%%%%%&%&%&@@@@@@@@@@@@@@@@&@@@@@@@@@@@@@@&%#%####%%%##(/&&@@@@@@@@@@@@@@@@@@@@@@&&&&&&&%&%%%%%%%%%%%%%
#########%%%%%%%%%%%%%%&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&@%%%%%%%%#(/&&@&&&&&@@@@@@@@@@@@@@@@@@@@@&%&%%%%%%%%%%%%%%%
##########%%%%%%%%%&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@%%%%%%#((&@&@@&@&&@@@@@@@@@@@@@@@@@@@@@@@@@&%%%%%%%%%%%%%
############%%%%&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@%%%%%##@@&@&&@@@@@&@@@@@@@@@@@@@@@@@@@@@@@&@&@%%%%%%%%%%%
((##########%&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&@@@@@%%#&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&&%%%%%####
(((######%%&&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@%@@@@@@@@@@@@@@@&@@@@@@@@@@@@@@@@@@@@@@@@@@@@&&%%%####
((((((#&&&&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&@%#####
((((#&&&&@&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&@@@@@@@@&@@#####
(((%%&&&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&@@&####
(#%&&&&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&@@@@@@@@&@@&&###
%%&&&&&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&@&@@@&@@&@@&&###
%%&&&&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&@&@&@@@&@@&&@#(#
&&&&&&&@&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&&@&&@@@@@@&&&@(((
%&&&&&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&&&%@@&@@@@@&@@(((
%&@&&&@@@@@@@@@@@@@@@@@@@@@&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&&&&%&@@@@@@%@@@((
-->