[:arrow_left: Retour vers le portfolio](https://github.com/ThibaultLanthiez/Portfolio)

<img src="https://github.com/ThibaultLanthiez/Detection-port-masque/blob/main/image-mask.PNG" width="140%" and height="120%"/>

# Détection du port de masque

L'objectif de ce projet de créer un modèle identifiant si les personnes présentes sur une photo portent correctement le masque ou non.

Pour cela, j'ai téléchargé sur la plateforme Kaggle un jeu de données de 800 images. Ces images représentent une ou plusieurs personnes. J'ai aussi la position de chaque personne grâce à quatre points formant un rectangle autour de leur tête. De plus, pour chaque personne je sais si elle porte ou non un masque et même si elle le porte mal.

En "découpant" chaque tête des personnes sur les photos, j'ai pu créer un nouveau jeu de données. Ainsi, j'ai pu créer un modèle qui détermine la manière dont la personne porte le masque.

Enfin, le modèle CascadeClassifier de la bibliothèque CV2 de python permet d'identifier les personnes sur une photo. Ainsi, en passant une photo dans CascadeClassifier puis mon modèle de classification de masque, je peux déterminer si les personnes portent correctement leur masque ou non.

# Code

Voici le code du projet : [notebook](https://github.com/ThibaultLanthiez/Detection-port-masque/blob/main/Mask%20detection.ipynb)
