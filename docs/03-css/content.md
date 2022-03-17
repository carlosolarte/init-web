
## Initiation Web (G1INWEB)
## CSS (CM3)
---
## Déjà vu ...
---
### HTML (HyperText Markup Language) 

- Langage de _balisage d'hypertexte_
- Langage _standardisé_ utilisé pour la description des __pages Web__
- _Hyperlien_:  permet de passer d’un document à un autre
---
### Balises 
<img src="https://developer.mozilla.org/fr/docs/Learn/HTML/Introduction_to_HTML/Getting_started/chat-grincheuxl.png">

Source : [Commencer avec le HTML](https://developer.mozilla.org/fr/docs/Learn/HTML/Introduction_to_HTML/Getting_started)
---
### Balises 

Exemples : 
```html
<title> Le titre de mon  document </title>

<p> Un  paragraphe  dans  mon  document. </p>
```
- Les balises _structurent le contenu_ de la page (texte, images, etc.).
- Chaque balise a un __rôle__ et donne du __sens__ au contenu présenté.
- Chaque balise commence par le caractère __"<"__ et se termine par le caractère __">"__
- Ces balises _ne sont pas affichées_ par le navigateur car elles ne
  correspondent pas à du texte

---
### Structuration d'un document HTML

Deux grandes parties :
1. _En-tête_ : définition du titre, du codage, des mots-clés, etc.
- Information destinée aux machines (navigateur, robots, etc.)
2. _Corps_ : contenu de la page Web
- Information destinée à l'humain (et aux machines)

---
##  Aujourd'hui 

<img src="https://www.interviewbit.com/blog/wp-content/uploads/2021/10/HTML-and-CSS.png" width="700">

Source : [interviewbit](https://www.interviewbit.com/)

---
### Mettre en forme une page Web

- Balise `<span>` : conteneur générique _en ligne_
- Attribut `style` : Par exemple, `color=COULEUR`

Changer la couleur :

```html
Le texte en <span style="color:blue">blue</span> 
et le texte en <span style="color:red">rouge</span> 
```
---
### Mettre en forme une page Web
- Et si je veux changer la couleur de tous les titres ?
- Et si je veux tous les mots importants en rouge ?

En général, le formatage du texte est géré non par HTML mais par une
feuille  de style _CSS_ 

---
### CSS

- _Cascading_ Style Sheets
- Feuilles de style en cascade
- Standard développé par le W3C.

---
### CSS

Principe de séparation :    
 - Fond : _HTML_
 - Forme :  _CSS_

> Un site HTML bien conçu devrait ne contenir aucune information de style
---
### HTML 
Structure / Fond 

<img src="css0.png" width=700>
---
### HTML + CSS
Mis en forme 

<img src="css3.png" width=300>

---
### HTML + CSS
Mis en forme 

<img src="css1.png" width=800>
---
### CSS : Syntaxe générale 

<img src="./structure.png">

---
### CSS : Syntaxe générale 

<img src="./structure.png" width=400>

- _Sélecteur_ : Désigne les éléments d'un document concernés par la règle
- _Déclarations_ : propriété et valeur 

---
### Fichier CSS
<img src="./files.png" width=300>

- Comment inclure la feuille de style dans la page HTML ?
---
### Fichier CSS
__À éviter !!!__

```html
<h1 style="color : white ; 
        background-color : black ; 
        font-weight : bold"> 
        Titre No 1</h1>

```
> Un site HTML bien conçu devrait _ne contenir aucune_ information de style

---
### Fichier CSS
Style dans l'en-tête (`<head>`)

<img src="./entete.png" width="500">

Vaguement mieux ... Mais si mon site a plusieurs pages HTML ?

---
### Fichier CSS
- Fichier ayant l'extension _.css_
- Syntaxe insensible aux espaces et retours à la ligne 
- L'_indentation_ est __fortement recommandée__
---
### Fichier CSS
<img src="./entete2.png">

- `rel` (__obligatoire__) : indique la nature de la relation établie entre deux ressources 
- `feuille.css` est un fichier de code CSS qui va permettre de _styliser le document actuel_

---
### Fichier CSS
feuille.css
```css
h1{
    color : white;
    font-weight : bold;
    background-color: black;
}
```
- Définition des propriétés de `<h1>`
- Voir [Exemple](./exemples/ex1)
---
### Fichier CSS

Les avantages de cette méthode :
- _Séparation totale_ de la structure et de la présentation 
- Possibilité d’avoir des présentations __alternatives__
- Possibilité d’appliquer la même feuille de style sur plusieurs pages 
- _Cohérence_ de la présentation sur tout le site et les pages futures.
---
### Commentaires 
Code CSS qui __n’est pas exécuté__, donc non pris en compte par le navigateur
```css
h1{
    /* Titre h1 */
    color : white;
    /* font-weight : bold; */
    background-color: black;
}
```

- Les commentaires restent _visibles_ dans la source de la feuille de style
- Attention à ne pas y laisser d’informations confidentielles !

---
## Les principales propriétés et leurs valeurs
---
### Modification de la police
#### font-size :  taille de la police 
_Valeurs absolues_ 

- xx-small
- x-small
- small
- medium (_par défaut_) 
- large
- x-large
- xx-large

Voir [exemple](./exemples/ex2/page.html)

---
### Modification de la police
#### font-size :  taille de la police 
_Valeurs relatives_ 
- larger (plus grande que celle de l'élément _parent_)
- smaller 

Voir [exemple](./exemples/ex2/page.html)

---
### Modification de la police
#### font-size :  taille de la police 
_Valeurs numériques_
- `font-size : 12px;` : taille en pixels (déconseillée)
- `font-size : 0.5em;` : la taille est la moitié de celle utilisée pour l'élément parent

Voir [exemple](./exemples/ex2/page.html)
---
### Modification de la police
#### font-weight :  graisse de la police

- lighter
- normal
- bold
- bolder
- Valeurs numériques entre 0 et 1000 

> Les niveaux de graisse disponibles _dépendent de la police_. 
> Certaines fontes n'existent qu'avec les niveaux de graisses `normal` et `bold`.

Voir [exemple](./exemples/ex2/page2.html)
---
### Modification de la police
#### font-style :  inclinaison de la police 
- normal
- italic 

Voir [exemple](./exemples/ex2/page2.html)
---
### Modification de la police
#### text-decoration :  décoration (soulignage, surlignage)
- underline
- overline
- line-through
- none
- color : couleur de la ligne 
- dotted 
- wavy

Voir [exemple](./exemples/ex2/page2.html)

---
### Modification de la police
#### font-family : famille de la police de caractères 
-  Grandes familles : serif, sans-serif, mono, monospace
-  Nom de police : Arial, Courier New, Courier, Helvetica, Times ...

- `font-family` permet de définir une liste _ordonnée par priorité_. 
-  Le navigateur choisira la première police installée sur l'ordinateur 
- `@font-face` : polices chargées depuis un fichier 

Voir [exemple](./exemples/ex2/page3.html)

---
### Modification de la police
#### Capitales 
`font-transform` : police en capitales / minuscules 

- capitalize (première lettre)
- uppercase (capitales)
- lowercase (minuscules) 
- none (normal)

Voir [exemple](./exemples/ex2/page3.html)
---
### Modification du texte
`text-align` :  permet de spécifier l'alignement horizontal du texte
- left : alignement à gauche 
- right : alignement à droite 
- center : centré
- justify : texte justifié 

Voir [exemple](./exemples/ex2/page4.html)

---
### Couleurs 
`color` : couleur de la police 

- Couleurs _prédéfinies_ : red, blue, green ... (~ 140 couleurs)
- Code _hexadécimal_ : composé de trois chiffres hexadécimaux représentant les
  tons de __rouge__, de __vert__ et de __bleu__. Il permet de définir plus de 16 millions
  de couleurs (ex. `#4B0082`).

---
### Couleurs 
`color` : couleur de la police 

- _Code RGB_ : définit les composantes de __rouge__, __vert__ et __bleu__ en
  indiquant leur proportion en pourcentage ou en notation absolue (0-255).
  Ex. `rgb(75,0,130)`. 
- _Code HSL_ : Hue, Saturation, Luminosity (Teinte, Saturation, Luminosité). Ex. `hsl(16,100%,50%)`

Voir la liste de couleurs [ici](https://fr.wikipedia.org/wiki/Couleur_du_Web)
Outils : [gcolor3](https://github.com/Hjdskes/gcolor3)

[Exemple](./exemples/ex2/page5.html)

---
### Couleurs de fond
- `background-color` : indique la couleur de fond

[Exemple](./exemples/ex3/page1.html)

---
### Les flottants
- `float` : faire "flotter" un élément au tour du texte 
- Valeurs : `right` ou `left`
- `clear` : l'élément ne continue pas à flotter.
- Valeurs : `right`, `left`, `both` 

Voir [Exemple](./exemples/ex3/page.html)

---
### Images de fond
- `background-image: url("image.png")`

* [Exemple répétition](./exemples/ex3/page4.html)
* [Exemple répétition Y](./exemples/ex3/page4a.html)
* [Exemple cover ](./exemples/ex3/page4b.html)

---
### Identifiants et classes

```css
h2{
    ...
}
```

Toutes les balises `<h2>` sont modifiées 
---
### Identifiants et classes
#### Identifiants 
* Syntaxe _HTML_ : `<h1 id="titre">`
* Syntaxe _CSS_ : `#titre { ... }`
* Utilisation _unique_ (un seul `id="titre"` dans la page HTML)
---
### Identifiants et classes
#### Classes
* Syntaxe _HTML_ : `<h1 class="titre">`
* Syntaxe _CSS_ : `.titre { ... }`
* Utilisation multiple (plusieurs `class="titre"` autorisés dans la page HTML)

---
### Identifiants et classes
#### Conteneurs
Destinés à _structurer_ le contenu.

- `<span class...>` ou `<div class...>` : appliquer une classe à une portion de code
  HTML qui n’est pas délimitée par des balises
- `<span id...>` ou `<div id...>` : idem pour les identifiants. 

- _Div_ : Pour les _blocs_
- _Spam_ : Pour les lignes (__"inline"__) 

[Exemple](exemples/ex3/page2.html)

---
### Héritage

* Les propriétés CSS _héritent_ des propriétés parentes. 

Voir [Exemple](./exemples/ex3/page3.html)

---
### Combinaisons de sélecteurs
```css
h2{
    ...
}
```
Toutes les balises `<h2>` sont modifiées 
---
### Combinaisons de sélecteurs

```css
X,Z{
    ...
}
```
Les modifications s’appliquent aux éléments X et aux éléments Z

Voir [Exemple](./exemples/ex4/page0.html)

---
### Combinaisons de sélecteurs

```css
X Z{
    ...
}
```
Correspond à tout élément  Z qui est un _descendant_ de l'élément X

Voir [Exemple](./exemples/ex4/page.html)

---
### Combinaisons de sélecteurs

```css
X>Z{
    ...
}
```
Correspond à tout élément  Z qui est un _enfant_ de l'élément X

Voir [Exemple](./exemples/ex4/page1.html)

---
### Combinaisons de sélecteurs

```css
*{
    ...
}
```
Tous les éléments 

Voir [Exemple](./exemples/ex4/pageetoile.html)

---
### Combinaisons de sélecteurs

```css
X~Z{
    ...
}
```
Correspond à tous les Z qui _suivent_ un élément X et qui sont __au même niveau__ (voisins / frères et sœurs)

Voir [Exemple](./exemples/ex4/page2.html)

---
### Combinaisons de sélecteurs

```css
X+Z{
    ...
}
```
Correspond à l’élément directement suivant à X 

Voir [Exemple](./exemples/ex4/page3.html)

---
### Combinaisons de sélecteurs

```css
X.maClasse{
    ...
}
```
Correspond à tout élément X ayant comme classe "maClasse"

Voir [Exemple](./exemples/ex4/page4.html)

---
### Combinaisons de sélecteurs

```css
.maClasse X{
    ...
}
```
Correspond aux éléments X descendants d’un élément ayant comme classe maClasse 

Voir [Exemple](./exemples/ex4/page5.html)

---
### Combinaisons de sélecteurs

- __`#abc p.rouge > a`__ :  cible les liens qui sont _enfants_ de paragraphes
  appartenant à la classe "rouge", eux-mêmes _descendants_ d'éléments dont
  l’identifiant est "abc".
- __`p > em.rouge.Italique,   h1.bleu`__ : cible les éléments mis en
  valeur par la balise em appartenant aux classes "rouge" et "Italique" et
  enfants de paragraphes, ou alors aux éléments h1 appartenant à la classe
  "bleu".
- __`p.rouge`__ : les paragraphes appartenant à la classe "rouge"
- __`p .rouge`__ : les éléments appartenant à la classe"rouge" et descendants d’un paragraphe.

---
### Combinaisons de sélecteurs
#### pseudo-éléments et pseudo-classes

* `A[B]` : Tous les éléments A avec un attributs B
- `a[title]` : liens avec un attribut `title` 
- `a[title="titre"]` : liens avec `title` titre
- `a[title*="tre"]` : liens avec `title` qui contient tre

Voir [exemple](exemples/ex5/page3.html)

---
### Pseudo-classes
- indique _l'état_ dans lequel l'élément doit être pour être ciblé.
- `:hover` : Lorsque l'utilisateur __survole__ l'élément ciblé
```css
p:hover{
    color : blue ;
}
```

Voir [exemple](exemples/ex5/page1.html)

---
### Pseudo-classes
- indique _l'état_ dans lequel l'élément doit être pour être ciblé.

Spécialement pour  les _liens_ :
- `:active` : au moment du click 
- `:focus`  : lorsque l'élément est activé avec la souris
- `:visited` : modifie le lien après que l'utilisateur l'a visité.

Voir [exemple](exemples/ex5/page2.html)

> _Attention_ :  `focus + active` rendre presque invisible l'effet 
d'active. 

---
### Pseudo-classes
* `:first-child` : désigne le premier enfant d'un élément
* `:first-of-type` : cible le premier élément d'un type donné 
* `:not(X)` : cible les éléments qui ne sont pas représentés par X
* `:nth-child(an+b)` : cible les éléments fils dont les positions correspondent au motif an+b.

Voir [exemple](exemples/ex5/page4.html)

---
### Validateur

https://jigsaw.w3.org/css-validator/
---
### Jeu
https://flukeout.github.io/

-  voir 12, 15, 16, 19, 22, 24, 26

---
### Les bordures
- `border` : Définit les propriétés de la bordure d'un élément.
- `border-width` (largeur) : `thin` (fin), `medium` (intermédiaire) ou `tick` (épais)
- `border-width` : `3px`
- 1 valeur :  largeur pour les quatre côtés
- 2 valeurs :  1 (haute et basse) , 1 (droit et gauche)
- 3 valeurs : 1 (haute), 1 (droit et gauche), 1 (basse)
- 4 valeurs : 1 (haute), 1 (droit), 1(basse), 1(gauche) 

---
### Les bordures
- `border` : Définit les propriétés de la bordure d'un élément.
- `border-style` : 
 * `dotted` : série de points 
 * `dashed` : série de tirets 
 * `solid` :  ligne droite continue
 * `double` : deux lignes droites 
 * `groove` et `ridge` : effets 3D. 

---
### Les bordures
- `border-color` : couleur de la bordure. 

Voir [exemple](exemples/ex5/page5.html)

---
### Les bordures
Pour modifier une propriété d'un seul côté de la bordure : 
- `border-top-color`
- `border-bottom-width`
- `border-left-style`
- `border-right-color`

---
### Les bordures arrondies
- `border-radius` : arrondir les angles 
```css
// 1px: haute - gauche
// 2px: houte - droite 
// 3px: bas   - droite 
// 4px: bas   - gauche 
elem { 
    border-radius : 1px 2px 3px 4px;
}
```

Voir [exemple](exemples/ex5/page6.html)

--- 
### Les ombres
`box-shadow` : pour les _blocs_ :
 - décalage horizontal
 - décalage vertical
 - adoucissement du dégradé
 - couleur 

Voir [exemple](exemples/ex5/page7.html)

--- 
### Les ombres
`text-shadow` : pour le _texte_ :
 - décalage horizontal
 - décalage vertical
 - adoucissement du dégradé
 - couleur 

Voir [exemple](exemples/ex5/page8.html)

---
### Opacité
- `opacity` : valeur entre 0 et 1
- 1.0 : totalement opaque 
- 0.0 : totalement transparent 

Voir [exemple](exemples/ex5/page9.html)

---
### Marges et Bordures 
Tout élément HTML est considéré comme contenu dans une _boîte_, dont on peut définir :
- l’aire intérieure (background)
- l’espace intérieur (padding)
- la bordure (border)
- la marge extérieure (margin)

<img src="./border.png" width="500"/>

---
### Marges et Bordures 

<img src="./border2.png" width="700"/>

---
### Marges et Bordures 
#### Marge extérieure
En _pixels_ (px), en taille __relative__ (em) ou en _pourcentage_

- `margin-top`
- `margin-right`
- `margin-bottom`
- `margin-left`
- `margin` : top right bottom left

- Voir [Exemple](./exemples/ex6/page1.html)

---
### Marges et Bordures 
#### Marge extérieure
`margin : auto` : pour _centrer_ l'élément !

- Voir [Exemple](./exemples/ex6/page2.html)
---
### Marges et Bordures 
#### Marge intérieure

- `padding-top`
- `padding-right`
- `padding-bottom`
- `padding-left`
- `padding` : top right bottom left

- Voir [Exemple](./exemples/ex6/page3.html)

---
### Marges et Bordures 
#### Dimensions et marges
- `box-sizing : content-box`. Width correspondent à la taille du _contenu_ uniquement
- `box-sizing : border-box`. Width correspondent à contenu + marges intérieures + bordure

- Voir [Exemple](./exemples/ex6/page4.html)

---
###  L’affichage en cas de dépassement
Propriété `overflow` : si le contenu d’un élément est supérieur aux dimensions (largeur et hauteur) de cet élément :

- `visible` : le contenu dépassant de l’élément sera affiché  (_chevauchement_)
- `hidden` : le contenu dépassant de l’élément ne sera pas affiché
- `auto` : une barre de défilement sera ajoutée si cela est nécessaire

- Voir [Exemple](./exemples/ex6/page5.html)
---

## Ordre d'application et héritage 
---
### Un conflit CSS

```css
p{ color : red ; }
.class1{ color : blue ; }
#id1{ color : yellow ; }
```
Quel couleur pour 

`< p class="class1" id="id1" > < /p >` ?

---
### Un conflit CSS
```css
p{ color : red ; }
.class1{ color : blue ; text-decoration: underline; }
#id1{ color : yellow ; }
```
Souligné ou pas ?

`< p class="class1" id="id1" > < /p >` 
---
###  Précision des sélecteurs 
Le sélecteur le _plus précis_ imposera ses styles aux sélecteurs moins précis en cas de conflit.

Degré de précision :
1. `#id`
2. `.class`
3. Éléments 

Voir [Exemple](./exemples/ex7/page.html)
---
### Héritage 
``` 
div{ color : red;}
```

Rouge ou pas ? 

```
< div > < p > < /p > < /div >
```
---
### Héritage 
- Les éléments enfants hérite les propriétés de leur parent.
- En cas de _conflit_, la propriété de l'enfant est utilisée.
- Propriétés tels que `margin`, `width`  et `border` ne sont pas hérité. 

Voir [Exemple](./exemples/ex7/page1.html)
---

### N'oubliez pas ...
de consulter la [référence](https://developer.mozilla.org/fr/docs/Web/CSS)
des propriétés. 
---
### QCM

https://www.wooclap.com/CMCSS
