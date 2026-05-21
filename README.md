# 🕹️ Jouer aux anciens jeux Flash (Road of Fury & autres)

Ce dépôt vous guide pour faire revivre vos jeux Flash préférés sur votre ordinateur, sans navigateur ni plugin obsolète, grâce à l'émulateur **[Ruffle](https://ruffle.rs/)**.

---

## 📥 Prérequis : installer Ruffle

Ruffle est un lecteur Flash moderne, sécurisé et gratuit. Téléchargez la version **Desktop** correspondant à votre système :

- [Windows](https://ruffle.rs/downloads#windows)
- [macOS](https://ruffle.rs/downloads#macos)
- [Linux](https://ruffle.rs/downloads#linux)

Une fois téléchargé, décompressez l'archive et placez l'exécutable `ruffle` (ou `ruffle.exe`) dans un dossier dédié, par exemple `C:\Ruffle\`. Aucune installation n'est nécessaire.

---

## ▶️ Lancer un fichier `.swf`

1. Lancez Ruffle (double-cliquez sur l'exécutable).
2. Glissez-déposez un fichier `.swf` dans la fenêtre de Ruffle.
3. Le jeu démarre immédiatement. Vous pouvez également utiliser le menu **File > Open** pour parcourir vos dossiers.

---

## 🗂️ Structure de dossier recommandée (sur votre ordinateur)

Pour éviter de vous perdre parmi des fichiers aux noms parfois cryptiques, organisez vos jeux ainsi :

Mes_Jeux_Flash/<br>
├── Road_of_Fury/<br>
│ ├── Road_of_Fury.swf<br>
│ ├── RoF2_23Dec.swf<br>
│ ├── RoadZ.swf<br>
│ └── infos.txt<br>
├── Autre_Jeu/<br>
│ ├── jeu_principal.swf<br>
│ └── ...<br>
└── Raccourci_Ruffle.lnk (optionnel)<br>

**Astuce** : renommez les fichiers `.swf` avec des noms clairs (ex. `Road_of_Fury_1.swf`) tout en conservant l’extension `.swf`. Si un fichier porte un nom comme `551cfce133e26222247814.swf`, identifiez-le d’abord avec Ruffle, puis renommez-le.

---

## 🌐 Où trouver des jeux Flash ?

Plusieurs sources fiables existent pour récupérer des `.swf` :

| Source | Description |
|--------|-------------|
| [Internet Archive](https://archive.org/) | Des millions de fichiers `.swf` dans des collections comme « Flash Game Archive ». Recherchez par titre ou explorez les collections dédiées. Utilisez le torrent pour tout télécharger d’un coup. |
| [Flashpoint Archive](https://bluemaxima.org/flashpoint/) | Un projet de préservation colossal avec un launcher tout-en-un. Téléchargez la version Infinity pour accéder à des milliers de jeux prêts à jouer. |
| [Newgrounds](https://www.newgrounds.com/) | De nombreux jeux Flash restent jouables directement sur le site grâce à Ruffle intégré. Possibilité de récupérer les `.swf` pour un usage local. |
| [Dépôts GitHub](https://github.com/topics/swf-games) | Cherchez des collections via le tag `swf-games` ou des projets comme [FlashStorage](https://github.com/FlashStorage/FlashStorage.github.io). |

---

## 🔍 Identifier le bon fichier `.swf`

Les archives contiennent parfois des noms cryptiques (`551cfce133e26222247814.swf`). Pour les reconnaître :

1. Ouvrez le fichier avec Ruffle. Si le jeu démarre, c’est le bon.
2. Aidez-vous des captures d’écran souvent présentes sur la page de l’archive (fichiers `.png` ou `.jpg`).
3. Notez la taille : le jeu principal est généralement le plus volumineux (plusieurs Mo).
4. Renommez-le avec un nom clair (`Road_of_Fury.swf`) **sans supprimer l’extension `.swf`**.

---

## ❓ Problèmes fréquents

### Le jeu ne se lance pas (écran noir)
- Vérifiez que le fichier est bien un `.swf` valide (pas corrompu).
- Essayez un autre fichier de la même archive (parfois une version alternative fonctionne).

### La souris ne répond pas dans le menu
- Un clic droit dans Ruffle permet d’activer le verrouillage de la souris (indispensable pour certains jeux).

### Pas de son
- Ruffle gère la plupart des sons Flash. Si le son manque, le jeu utilisait peut-être un format audio externe non inclus dans le `.swf`.

### Le jeu est en anglais ?
- Modifiez les options dans le menu du jeu quand c’est possible. Ruffle ne traduit pas automatiquement.

---

## 🧩 Exemple concret : jouer à Road of Fury

1. Téléchargez les fichiers `.swf` depuis [cette page](https://archive.org/download/road-of-fury-flash-game-series) (le plus simple : prenez le torrent).
2. Placez-les dans un dossier `Mes_Jeux_Flash/Road_of_Fury/`.
3. Lancez Ruffle et ouvrez `Road_of_Fury.swf` (ou `RoF2_23Dec.swf` pour la suite).
4. Profitez ! 🎉

---

## 📦 Structure du dépôt (pour ranger vos jeux)

Si vous utilisez ce dépôt pour partager une collection, voici l’organisation conseillée :<br>
.<br>
├── README.md # Ce guide<br>
├── ruffle/ # (optionnel) Exécutable Ruffle portable<br>
├── games/<br>
│ ├── Un_Jeu/ (Exemple)<br>
│ └── Votre_Jeu/ (Exemple)<br>
├── screenshots/ # Captures d’écran ou jaquettes<br>
└── ...<br>

---

## 🤝 Contribuer

Si vous possédez des jeux Flash inédits ou souhaitez améliorer ce guide, ouvrez une **issue** ou une **pull request**. Ensemble, préservons ce patrimoine vidéoludique.

---

## 📄 Licence

Ce guide est sous licence [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/). Vous êtes libre de l’utiliser, de le modifier et de le partager sans restriction.

**Bon jeu !** 🚗💨
