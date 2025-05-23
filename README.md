# Face Recognition App with Encoding Cache

## Description

Cette application utilise la reconnaissance faciale en temps réel via la webcam, avec un système d'encodage facial optimisé par cache pour accélérer le processus. Les images des personnes connues sont encodées une fois et sauvegardées dans un fichier cache (`encodings.pickle`) pour éviter le recalcul à chaque démarrage. L’application détecte les visages, les compare avec la base encodée, et affiche le nom associé directement sur la vidéo.

---

## Fonctionnement

1. Chargement des images des personnes à reconnaître depuis le dossier `data/`.
2. Encodage des visages avec la bibliothèque `face_recognition`.
3. Sauvegarde ou chargement des encodages dans un fichier cache pour accélérer les futures exécutions.
4. Capture vidéo en direct via la webcam.
5. Détection et reconnaissance des visages présents dans chaque image.
6. Affichage du cadre et du nom des personnes reconnues dans la fenêtre vidéo.

Pour quitter la vidéo, appuyez sur la touche `q`.

---

## Outils utilisés

- **Python** : langage principal  
- **Jupyter Notebook** : environnement de développement interactif  
- **OpenCV (`cv2`)** : capture vidéo et traitement d’image  
- **face_recognition** : détection et encodage des visages  
- **NumPy** : calculs numériques et manipulation des tableaux  
- **pickle** : gestion du cache des encodages  
- **os** : manipulation des fichiers et chemins  

---
