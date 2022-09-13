Pas à pas
=========

.. note::
	Cette page est une ébauche non encore rédigée.


1. Commencer
------------

1.1. Se connecter
^^^^^^^^^^^^^^^^^

La connexion à l'application suppose de disposer d'un compte utilisateur associant un login, une adresse e-mail et un mot de passe. 

On accède au formulaire de connexion en cliquant sur "Login" dans le menu. On entre ensuite soit le login, soit l'adresse mail, ainsi que le mot de passe. On cliquer ensuite sur Login pour se connecter. 

En cas d'oublie de mot de passe, cliquer sur "Lost password?" pour accéder à un formulaire qui génère un email permettant de créer un nouveau mot de passe.

1.2. Créer un projet
^^^^^^^^^^^^^^^^^^^^

Une fois connecté, l'utilisateur arrive sur le tableau de bord des projets. Les projets sont des ensembles de documents, eux-mêmes composés de pages. 

Pour débuter un travail sur eScriptorium, il faut créer son propre projet ou bien être invité dans le projet d'un autre utilisateur. 

Pour créer un projet, il faut cliquer sur le bouton "Create new project" depuis le tableau de bord des projets. 

Le formulaire ne contient qu'un seul champ : le nom du projet. Une fois ce champ rempli, on clique sur "Create". Le nouveau projet apparaît désormais dans le tableau de bord. 

1.3. Créer un document
^^^^^^^^^^^^^^^^^^^^^^

Lorsque l'on cliquer sur un projet depuis le tableau de bord des projet, on accède à la liste des documents qu'il contient. Chacun de ces documents est constitué d'une série d'images formant un ensemble cohérent. 

Pour débuter un travail dans eScriptorium, il faut soit créer un document au sein d'un projet, soit être invité dans le document (ou projet contenant des documents) d'un autre utilisateur.

Pour créer un document, il faut cliquer sur le bouton "Create new Document". 

Dans le formulaire qui s'affiche alors, seul le champ "Name" (nom du document) est obligatoire. Les autres sont facultatifs et peuvent être remplis plus tard. Une fois ce champ rempli, on clique sur "Create". 

Pour retourner au niveau du projet, on clique sur la flèche "⟵", à côté de "Description". Le nouveau document apparaît désormais dans le tableau de bord. 


2. Charger des images
---------------------


2.1. Charger des image depuis le système de fichiers local
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Pour accéder à la fenêtre permettant de charger des images, on clique sur un projet, puis sur un dossier, et enfin sur l'onglet "images". Un rectangle déssiné par les pointillés définit une zone où l'utilisateur peut glisser-déposer des fichiers images, un par un ou en lot. Une fois les fichiers déposés, la progression du chargement de chaque image s'affiche. Il est vivement conseillé de ne pas rafraîchir la page durant cette étape. 

Il est aussi possible de cliquer dans le rectangle pour ouvrir l'explorateur de fichiers et sélectionner les images à charger. Elles sont alors ordonnées selon l'ordre de sélection des fichiers. 

2.2. Charger des images contenues dans un PDF
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Pour accéder à la fenêtre permettant de charger des images, on clique sur un projet, puis sur un dossier, et enfin sur l'onglet "images". Cliquer sur le bouton "Import" puis "Images (PDF)" pour ouvrir l'explorateur de fichier. Cliquer sur le PDF à importer, chaque page en sera extraite sous la forme d'une image.

2.3. Charger des images hébergées sur un serveur IIIF
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Pour accéder à la fenêtre permettant de charger des images, on clique sur un projet, puis sur un dossier, et enfin sur l'onglet "images". Cliquer sur le bouton "Import" puis "Images (IIIF)". Dans la fenêtre qui s'affiche, entrer l'URL du manifeste IIIF référencant les fichiers à importer. Cliquer sur "Start importing". Les images sont importées une par une, ainsi que les métadonnées associées au manifeste. Elles sont consultables dans l'onglet "Description".

3. Segmenter
------------

- expliquer ce que c'est que la segmentation
- expliquer le vocabulaire (baseline/polygone etc)

3.1. Lancer une segmentation automatique
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- dans le volet image
- selectionner les images
- cliquer sur segment
- selectionner le modèle à appliquer
- sélectionner le mode de segmentation

3.2. Réinitialiser le calcul des masques
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- expliquer pourquoi on aurait besoin de le faire
- dans le volet image
- selectionner les images
- cliquer sur segment
- selectionner le modèle à appliquer
- sélectionner le mode de segmentation "only masks"

3.3. Segmenter manuellement ou corriger la segmentation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

3.3.1. Créer ou modifier les lignes de bases
""""""""""""""""""""""""""""""""""""""""""""
- dans edit, activer le volet 2
- tracer une ligne en cliquant à deux endroits sur l'image
- échape pour arreter
- on peut double cliquer pour ajouter des points
- on peut faire un tracé libre en restant appuyé
- on peut fusionner deux lignes
- on peut changer le sens de lecture d'une ligne
- on peut diviser une ligne
- on peut supprimer un point sur une ligne
- on peut selectionner plusieurs lignes en même temps (shift + drag ou ctrl a)

3.3.2. Créer ou modifier les zones
""""""""""""""""""""""""""""""""""
- dans edit , activer le volet 2
- cliquer sur 'toggle region mode'
- les régions sont des rectangles
- on peut ajouter des points
- on peut découper des formes plus complexes en utilisant les ciseaux
- on ne peut pas fusionner deux zones
- on peut selectionner plusieurs zones en même temps (shift + drag ou ctrl a)

3.4. Associer des lignes à un zones
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

3.5. Les racourcis du volet de segmentation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- faire la liste des racourcis
- ajouter que pour naviguer sur l'image quand on a zoomé c'est clic-droit puis on bouge la souris

4. Transcrire
-------------

4.1. Prérequis
^^^^^^^^^^^^^^
- avoir segmenté
- avoir un modèle

4.2. Lancer une transcription automatique
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- sélectionner les images dans le volet images/
- cliquer sur transcrire
- choisir le modèle
- cliquer sur transcrire
- consulter le résultat en allant sur edit puis sélectionner la version de transcription correspondant au modèle appliqué

4.3. Transcrire manuellement ou corriger la transcription
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- aller sur edit
- activer le paneau 3
- cliquer sur une ligne vide ou transcrite
- saisir le texte dans la pop-up
- cliquer sur entré pour valider
- naviguer entre les lignes en cliquant sur les flèches (ou les touches flèches)

4.4. Accéder au clavier virtuel
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- expliquer ce qu'est le clavier virtuel
- activable depuis la pop-up de saisie
- expliquer comment modifier les touches
- expliquer comment exporter ou importer une configuration

4.5. Comparer des transcriptions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- dans l'onglet edit
- en haut, cliquer sur rouages puis cocher les versions à comparer
- activer l'affichage de la version de référence
- afficher le volet 3 puis cliquer sur la ligne à observer
- l'historique s'affiche sous le texte, en rouge les deletions, en vert les additions

5. Contrôler l'ordre de lecture
-------------------------------

- les lignes sont lues zones par zones
- on peut consulter l'ordre de lecture dans le volet 2
- on peut modifier l'ordre de lecture dans le volet 4
- l'ordre de lecture peut être réinitialisé, il faut donc faire ça quand on a fini de modifier la segmentation


6. Typer les zones et les segments
----------------------------------

- noter que ce sont des informations qu'une modèle de segmentation peut apprendre
- par contre si on veut l'appliquer sur un nouveau document, il faut penser à paramétrer correctement l'ontologie

6.1. Paramétrer l'ontologie
^^^^^^^^^^^^^^^^^^^^^^^^^^^

6.2. Associer un type à une ligne ou une zone
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

7. Exporter
-----------

7.1. Exporter des images et des transcriptions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- formats possibles
- paramètres de l'export (images / lignes / zones)
- accéder à l'historique des exports

7.2. Exporter un modèle
^^^^^^^^^^^^^^^^^^^^^^^


8. Importer
-----------

8.1. Importer depuis un fichier XML
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Il est possible d'importer les coordonnées des régions, lignes et masques à appliquer à une image à partir d'un fichier XML. Il en va de même pour les transcriptions, dès lors que le texte est associé, à minima, à des lignes et des masques. 

Les formats supportés sont les mêmes que ceux disponibles à l'export : XML ALTO et XML PAGE. 

L'import de données depuis des fichiers XML se fait à partir de l'onglet "Images" dans un document. Cliquer sur "Import" puis "Transcriptions (XML)". L'explorateur de fichiers s'ouvre, l'utilisateur peut alors sélectionner un seul fichier : soit un fichier XML pour un import unique, soit un fichier ZIP contenant plusieurs fichiers XML pour un import en masse. Si un fichier XML ne correspond à aucune image, il est tout simplement ignoré. 

**Attention :** importer la segmentation contenue dans un fichier XML peut causer l'écrasement de la segmentation existant dans l'application. L'utilisateur doit penser à enregistrer ses données au préalable si ce n'est pas l'effet souhaité. 

> Note : il est possible d'importer des blocs de texte en se servant du 4e volet de visualisation. Après avoir vérifié l'ordre des lignes, on peut copier-coller des blocs de texte dans lesquels on a prélablement ajouté les sauts de ligne correspondants. 

8.2. Importer un modèle
^^^^^^^^^^^^^^^^^^^^^^^

Cliquer sur "My Models" dans le menu pour afficher la liste des modèles disponibles. Cliquer sur le bouton "Upload a Model" pour ouvrir l'explorateur de fichiers et choisir le fichier `.mlmodel` à importer. L'utilisateur peut alors remplir le champ "Name" s'il souhaite modifier le nom affiché dans l'application. Cliquer ensuite sur "Upload", le modèle apparaît désormais dans la liste des modèles de l'utilisateur qui peut y faire appel au sein de n'importe quel projet ou document.

9. Entraîner un modèle
-----------------------
- procédure
- quelques remarques de bons sens
- distinction entre affinage et entraînement from scratch

10. Controler
-------------

10.1. Contrôler les métriques de mon projet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

10.2. Consulter l'état d'exécution des tâches
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
