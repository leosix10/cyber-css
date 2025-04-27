# Cyber CSS - Bibliothèque de composants UI

Cette bibliothèque regroupe plusieurs composants UI réalisés dans un style **Cyberpunk**, pour une interface dystopique, technologique et immersive.

## Explication du style Cyberpunk 

Le style Cyberpunk s’inspire d’un futur dystopique, souvent urbain, technologique et chaotique. Graphiquement, il se caractérise par des couleurs vives (rose flashy, bleu électrique, jaune) sur des fonds sombres ou noirs, ce qui donne un contraste important, donc une bonne lisibilité. Ce style contient aussi des textures numériques, comme des effets glitchs ou des hologrammes, en guise d'animation. Des sites internet ont intégré ce style, comme celui du jeu [Cyberpunk 2077](https://www.cyberpunk.net/us/fr/).

## Présentation des composants et leurs variantes

### 1. Boutons

Les boutons ont été décliné en 4 styles :

- Avec icône
- Sans icône 
- Avec contour
- Bouton désactivé

Des états ont été appliqué à ces éléments. Au survol, un effet glitch apparaît, qui correspond au style Cyberpunk. Lorsqu'on clique, le bouton s'assombrit. Ces états ne s'appliquent pas au bouton désactivé.

### 2. Cartes

Ce composant contient une image, un titre, un paragraphe et un bouton CTA, le tout dans un style Cyberpunk avec ses angles coupés. Au survol, la bordure cyan se déplace. Il existe une variante sans image.

### 3. Galerie

Cette galerie contient des images, accompagné de leurs légendes au survol de l'image. Ce composant s'intègre bien visuellement grâce aux bordures biseautés. 

### 4. Header

L'en-tête du site est composé d'un logo sous forme de texte, ainsi que d'un menu de navigation. Ce menu contient 5 liens et un CTA qui redirige vers le lien pour télécharger le projet. Le header est responsive, il s'adapte à toutes les tailles d'écran, tout en gardant son style rétro-futuriste.

### 5. Formulaires

Pour rendre l'expérience utilisateur plus immersive, plusieurs formulaires ont été réalisés. 

- Newsletter : contient un champ de saisie pour une adresse mail, des cases à cocher (radio et checkbox) et un bouton pour s'inscrire.
- Message : ce formulaire est composé d'une liste d'options, d'un encadré pour écrire du texte et d'un bouton d'envoi.

## Organisation du projet

```
 Projet Cyber CSS
 ┣ 📂 assets
 ┃ ┣ 📂 fonts (police d'écriture)
 ┃ ┗ 📂 images 
 ┣ 📂 styles
 ┃ ┣ 📂 sass
 ┃ ┃ ┣ 📂 abstracts (variables, mixins, fonctions, ...)
 ┃ ┃ ┃ ┣ _variables.scss
 ┃ ┃ ┃ ┗ _mixins.scss
 ┃ ┃ ┣ 📂 base (remise à zéro du CSS, intégration de la typo)
 ┃ ┃ ┃ ┣ _fonts.scss
 ┃ ┃ ┃ ┗ _reset.scss
 ┃ ┃ ┣ 📂 components (boutons, cartes, formulaires, ...)
 ┃ ┃ ┃ ┣ _buttons.scss
 ┃ ┃ ┃ ┣ _cards.scss
 ┃ ┃ ┃ ┣ _forms.scss
 ┃ ┃ ┃ ┣ _gallery.scss
 ┃ ┃ ┃ ┗ _header.scss
 ┃ ┃ ┣ 📂 layout (mise en page)
 ┃ ┃ ┃ ┗ _body.scss
 ┃ ┃ ┗ main.scss (regroupement des propriétés utilisées)
 ┃ ┗ 📂 css (feuille de style compilée)
 ┃   ┣ main.css
 ┃   ┗ main.min.css
 ┣ 🗎 index.html
 ┗ 🗎 README.md
```

## Utilisation de la bibliothèque

Tu peux télécharger le projet en te rendant sur ce dépôt GitHub : [cyber-css](https://github.com/leosix10/cyber-css), puis va sur le bouton Code et choisis l'option que tu souhaites. 

Pour utiliser cette bibliothèque de composants UI basée sur le style **Cyberpunk**, voici les étapes à suivre :

1. **Ajoutez le CSS global :**
Vérifie d'avoir bien compilé le fichier `main.scss` (situé dans `styles/sass/`) vers `styles/css/main.css`.  Ensuite, dans ton fichier HTML, ajoute ce lien dans le `<head>` :

```html
<link rel="stylesheet" href="styles/css/main.css">
```
2. **Structure HTML :**
Chaque composant a été conçu pour être facilement réutilisable. Tu peux copier-coller les classes HTML de chaque composant (boutons, formulaires, cartes, header, galerie) directement dans ton projet. Tu peux retrouver la liste de toutes les classes utilisées en bas du fichier README.

3. **Images**
Les images nécessaires se trouvent dans le dossier images/. Pense à bien conserver la structure des fichiers ou à adapter les chemins si tu modifies l’arborescence.

4. **Sass :**
Si tu souhaites personnaliser les styles ou les intégrer dans un nouveau projet, tu peux travailler directement à partir des fichiers .scss.
Compile-les ensuite à l’aide de l'extension Live Sass Compiler sur VSCode ou tout autre compilateur Sass de ton choix.

### Classes utilisées

| Catégorie               | Classe                             |
|-------------------------|------------------------------------|
| **Header**              | header                             |
|                         | header__logo                       |
|                         | header__toggle                     |
|                         | header__burger                     |
|                         | header__menu                       |
|                         | header__cta                        |
| **Bouton**              | btn                                |
|                         | btn__primary                       |
|                         | btn__secondary                     |
|                         | btn__outline                       |
| **Carte**               | card                               |
|                         | card__image                        |
|                         | card__text                         |
| **Galerie**             | gallery                            |
|                         | gallery__image                     |
| **Formulaire**          | form                               |
|                         | form__text                         |
|                         | form__radio                        |
|                         | form__checkbox                     |
| **Autres**              | cyber__title                       |
|                         | cyber__component                   |


## À propos
Projet universitaire : Cyber CSS - bibliothèque de composants UI (travail noté)

Langages : SCSS, CSS, HTML

Outils : VSCode, [Live Sass Compiler](https://marketplace.visualstudio.com/items/?itemName=glenn2223.live-sass)

Auteur : [Léo Six](https://leosix.fr/), étudiant en Master 1 Design Graphique et d'Interaction

Année : 2025