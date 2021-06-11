# oNews

O'Clock sort son journal d'étudiants :muscle:

Votre mission, si vous l'acceptez (...pfff évidemment qu'on l'accepte ), sera d'intégrer la maquette du site.

![homepage](home.png)

## Infos

- il n'y a qu'une seule page à monter
- il y a une scrollbar à droite, mais on en tient pas compte
- cette fois, on utilise `reboot.css` pour standardiser les styles par défaut des balises HTML
- pour voir les différentes possibilités pour standardiser :
  - https://codepen.io/ncerminara/pen/RLMwmy
  - changez de sélection dans le menu déroulant _None (Browser styles only)_
  - vous verrez les différences en 1 clin d'oeil :wink:
- vous aurez besoin de spécifier une couleur avec de la transparence => `rgba(0, 0, 255, 0.5)` par exemple pour du bleu à 50% d'opacité => https://cssreference.io/property/color/
- vous aurez peut-être besoin de dire à un élément de prendre 100% de la hauteur de la fenêtre => `height: 100vh;`
  - pour comprendre l'unité `vh`, [la doc sur les unités de mesures sur MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/length)

## Charte

### Visuels

Le dossier `images` contient tous les visuels nécessaires pour cette intégration.

_Ne vous préoccupez pas pour l'instant du contraste des textes sur l'image :wink: Ça fera l'objet d'un bonus_ :skull:

### Couleurs

- fond header : #f9f9f9
- bordure d'article : #eaeaea
- WORK : #0766F0;
- TEAM : #DC5E53;
- NEWS : #98DC62;

### Font

Choix libre mais de type sans-serif

## Informations additionnelles

- Les deux parties (portrait et grille d'articles) sont sur une seule et même page
- L'image de la partie de gauche touche les bords supérieur, inférieur et gauche du navigateur, mais n'aura pas la même apparence selon la largeur de chaque écran. Tant qu'elle touche les bords, n'est pas déformée et prend la moitié de la page, c'est que c'est bon ; même si elle se retrouve un peu rognée verticalement.
- n'oubliez pas de mettre un effet lors du survol des liens par la souris :wink:
- un fichier _SVG_ est une image vectorielle, voir [MDN sur SVG](https://developer.mozilla.org/fr/docs/Web/SVG)
- si possible, placer le logo SVG en background :wink:

## Git

- il ne faut pas oublier d'enregistrer ses modifications (versions) avec **git**
- il est préférable de le faire à chaque fonctionnalité terminée (par exemple, une fois la partie de gauche terminée => sauvegarde)
- rappel des commandes **git** :
  - fiche récap : https://kourou.oclock.io/ressources/fiche-recap/git-et-github/#gestion-des-fichiers
  - schéma étapes : https://kourou.oclock.io/content/uploads/2020/09/premiers-pas.png
  - `git add .` pour ajouter tous les fichiers ajoutés/modifiés au prochain commit
  - `git commit -m "message explicite expliquant les modifs effectuées"` pour sauvegarder la version actuelle des fichiers sources

## Bonus "lisibilité" :white_flower:

Si vous avez lu tout l'énoncé, vous savez ce qu'il vous reste à faire ;-)
- Trouvez les propriétés et valeurs CSS idéales pour que le cadre transparent derrière le texte central bouge harmonieusement lorsque vous modifiez la taille de la fenêtre
- Identifiez un moyen de faire ressortir les liens en bas de la page sur le fond clair

## Bonus "défilement" :skull:

- il y a une scrollbar à droite, et désormais on en tient compte :boom:
- la page contient en tout 6 articles, même si seuls 4 sont visibles
- lorsqu'on fait défiler la page pour voir les 2 articles suivants :
  - la partie de gauche ne bouge pas, elle reste figée
  - le scroll fait descendre la partie droite et affiche les 2 articles suivants
