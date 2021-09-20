[:arrow_left: Retour vers le portfolio](https://github.com/ThibaultLanthiez/Portfolio)

<img src="https://github.com/ThibaultLanthiez/Detection-port-masque/blob/main/image-mask.PNG" width="140%" and height="120%"/>

# Détection du port de masque

L'objectif de ce projet est de créer un modèle identifiant si les personnes présentes sur une photo portent correctement le masque ou non.

Pour cela, j'ai téléchargé sur la plateforme Kaggle un jeu de données de plus de 800 images. Ces images représentent une ou plusieurs personnes. J'ai également la position de chaque visage via un cadre (quatre coordonnées formant un rectangle autour du visage). De plus, pour chaque personne je sais si elle porte ou non un masque et même si elle le porte correctement.

En "découpant" chaque visage des personnes sur les photos, j'ai obtenu un nouveau jeu de données. Ainsi, j'ai pu créer un modèle qui détermine la manière dont la personne porte le masque.

Enfin, le modèle [CascadeClassifier](https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html) de la bibliothèque OpenCV de Python permet d'identifier les personnes sur une photo. Ainsi, en passant une photo dans CascadeClassifier puis dans mon modèle de classification de masque, je peux déterminer si les personnes portent correctement leur masque ou non.

# Code

Voici le code du projet : [notebook](https://github.com/ThibaultLanthiez/Detection-port-masque/blob/main/Mask%20detection.ipynb)
