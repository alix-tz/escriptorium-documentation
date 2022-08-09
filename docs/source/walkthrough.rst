Pas à pas
=========

.. note::
	Cette page est une ébauche non encore rédigée.


1. Se connecter
---------------

2. Créer un projet
------------------

3. Créer un document
--------------------

4. Charger des images
---------------------


4.1. Charger des image depuis le système de fichiers local
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

4.2. Charger des images contenues dans un PDF
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


4.3. Charger des images hébergées sur un serveur IIIF
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

5. Segmenter une image
----------------------

- expliquer ce que c'est que la segmentation
- expliquer le vocabulaire (baseline/polygone etc)

5.1. Lancer une segmentation automatique
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- dans le volet image
- selectionner les images
- cliquer sur segment
- selectionner le modèle à appliquer
- sélectionner le mode de segmentation

5.2. Réinitialiser le calcul des masques
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- expliquer pourquoi on aurait besoin de le faire
- dans le volet image
- selectionner les images
- cliquer sur segment
- selectionner le modèle à appliquer
- sélectionner le mode de segmentation "only masks"

5.3. Segmenter manuellement ou corriger la segmentation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

5.3.1. Créer ou modifier les lignes de bases
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

5.3.2. Créer ou modifier les zones
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- dans edit , activer le volet 2
- cliquer sur 'toggle region mode'
- les régions sont des rectangles
- on peut ajouter des points
- on peut découper des formes plus complexes en utilisant les ciseaux
- on ne peut pas fusionner deux zones
- on peut selectionner plusieurs zones en même temps (shift + drag ou ctrl a)

5.5. Les racourcis du volet de segmentation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- faire la liste des racourcis
- ajouter que pour naviguer sur l'image quand on a zoomé c'est clic-droit puis on bouge la souris

6. Transcrire un document
-------------------------

6.1. Prérequis
^^^^^^^^^^^^^^
- avoir segmenté
- avoir un modèle

6.2. Lancer une transcription automatique
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- sélectionner les images dans le volet images/
- cliquer sur transcrire
- choisir le modèle
- cliquer sur transcrire
- consulter le résultat en allant sur edit puis sélectionner la version de transcription correspondant au modèle appliqué

6.3. Transcrire manuellement ou corriger la transcription
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- aller sur edit
- activer le paneau 3
- cliquer sur une ligne vide ou transcrite
- saisir le texte dans la pop-up
- cliquer sur entré pour valider
- naviguer entre les lignes en cliquant sur les flèches (ou les touches flèches)

6.4. Accéder au clavier virtuel
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- expliquer ce qu'est le clavier virtuel
- activable depuis la pop-up de saisie
- expliquer comment modifier les touches
- expliquer comment exporter ou importer une configuration

6.5. Comparer des transcriptions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
- dans l'onglet edit
- en haut, cliquer sur rouages puis cocher les versions à comparer
- activer l'affichage de la version de référence
- afficher le volet 3 puis cliquer sur la ligne à observer
- l'historique s'affiche sous le texte, en rouge les deletions, en vert les additions

7. Contrôler l'ordre de lecture des lignes
------------------------------------------

- les lignes sont lues zones par zones
- on peut consulter l'ordre de lecture dans le volet 2
- on peut modifier l'ordre de lecture dans le volet 4
- l'ordre de lecture peut être réinitialisé, il faut donc faire ça quand on a fini de modifier la segmentation


8. Typer les zones et les segments
----------------------------------

- noter que ce sont des informations qu'une modèle de segmentation peut apprendre
- par contre si on veut l'appliquer sur un nouveau document, il faut penser à paramétrer correctement l'ontologie

8.1. Paramétrer l'ontologie
^^^^^^^^^^^^^^^^^^^^^^^^^^^

8.2. Associer un type à une ligne ou une zone
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

9. Exporter les données
-----------------------
- formats possibles
- paramètres de l'export (images / lignes / zones)
- accéder à l'historique des exports

10. Importer des données
------------------------
- importer la segmentation ou la transcription à partir des fichiers XML
- hack pour importer un texte à plat

11. Importer un modèle
----------------------

12. Entraîner un modèle
-----------------------
- procédure
- quelques remarques de bons sens
- distinction entre affinage et entraînement from scratch

13. Consulter les métriques de mon projet
-----------------------------------------

14. Consulter l'état d'exécution des tâches
-------------------------------------------
