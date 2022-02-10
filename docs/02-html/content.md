
## Initiation Web (G1INWEB)
## HTML (CM1 et CM2)
---
## Déjà vu ...
---
### Internet
Internet est un ensemble de __réseaux interconnectés__,
utilisant un ensemble de _protocoles_ de communication et
_d'échanges de données_ standardisés.

---
### World Wide Web
Le World Wide Web est un système fonctionnant au-dessus
d'Internet, et basé sur des _liens hypertextes_. Il est
constitué de pages _Web_ organisées en __sites Web__,
lesquelles sont consultables grâce à un _navigateur_ Web

---
## HTML
### Objective

Écrire et modifier des pages Web dans un langage normalisé de description de contenus (_HTML_).

---
### HTML (HyperText Markup Language) 

- Langage de _balisage d'hypertexte_
- Langage _standardisé_ utilisé pour la description des __pages Web__
- _Hyperlien_:  permet de passer d’un document à un autre
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
### Balises et attributs
Exemples : 
```html
<img src="photo.png" width=300 />

<a href="page.html">click! </a>
```
De manière générale:
```html
<balise att1="val1" att2="val2" attn="valn" > ...  </balise> 
```
---
### Balises et attributs
#### Balises auto-fermantes
- Certaines balises ne sont pas utilisées par paire
- il n’y a rien à mettre entre la balise ouvrante et la balise fermante

Exemple : un retour à la ligne ` <br /> `
---
### Balises et attributs

#### Commentaires
- Ils facilitent la compréhension de votre code HTML
- Ils ne sont pas affichés par le navigateur 

```html
<!-- Ceci est un commentaire -->
```

