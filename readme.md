# Introduction

## Que ce que le html (Definition)

HTML est le langage utilisée pour créer les pages Web que vous visitez tous les jours. Il fournit une manière logique de structurer le contenu des pages Web.
Analysons l'acronyme "HTML", car il contient beaucoup d'informations utile. HTML signifie HyperText Markup Language.

	- Un langage de balisage est un langage informatique qui définit la structure et  la présentation du texte brut.
	- Les langages de balisage fonctionnent en entourant le texte brut avec des informations que l'ordinateur peut interpréter, "marquant" pour le traitement.
	- HyperText est affiché sur un ordinateur ou un périphérique qui permet d'accéder à d'autres textes via des liens, également appelés «hyperliens». En fait, vous avez probablement cliqué sur de nombreux hyperliens sur votre chemin vers d autre d autre site web par exemple quora ou ...

	Dans ce cours, vous apprendrez à utiliser les principes fondamentaux du HTML pour structurer, présenter et lier le contenu. Vous apprendrez également à utiliser CSS, ou Cascading Style Sheets, pour classer le contenu HTML que vous ajoutez aux pages Web.

## Commençons!
#### Le DocTyping

Un navigateur doit savoir dans quelle langue un document est écrit avant de pouvoir traiter le contenu du document.

Vous pouvez laisser les navigateurs Web savoir que vous utilisez la langue HTML en commençant votre document HTML avec une déclaration de type de document.
Un navigateur doit savoir dans quelle langue un document est écrit avant de pouvoir traiter le contenu du document.

Vous pouvez laisser les navigateurs Web savoir que vous utilisez la langue HTML en commençant votre document HTML avec une déclaration de type de document.

La déclaration est la suivante:

``` 
<! DOCTYPE html> 
```
Cette déclaration est une instruction. Il indique au navigateur quel type de document attendre, ainsi que la version HTML utilisée dans le document. ```<! DOCTYPE html>``` doit être la première ligne de code dans tous vos documents HTML.

Remarque: Si vous n'utilisez pas la déclaration doctype, votre code HTML fonctionnera probablement, mais il est risqué. À l'heure actuelle, le navigateur supposera correctement que vous utilisez HTML5, car HTML5 est la norme actuelle. À l'avenir, cependant, une nouvelle norme remplacera HTML5. Les futurs navigateurs peuvent supposer que vous utilisez une norme différente et plus récente, auquel cas votre document sera interprété de manière incorrecte. Pour vous assurer que votre document est interprété pour toujours correctement, incluez toujours ```<! DOCTYPE html>``` au tout début de vos documents HTML

## Preparation du document 

Génial! Les navigateurs qui lisent votre code savent s'attendre au HTML lorsqu'ils tentent de lire votre fichier.

La déclaration ```<! DOCTYPE html>``` n'est que le début, cependant. Il indique seulement au navigateur que vous envisagez d'utiliser HTML dans le document, il n'ajoute pas de structure ou de contenu HTML.

Pour commencer à ajouter de la structure et du contenu HTML, nous devons d'abord ajouter des balises ```<html>``` d'ouverture et de fermeture, de la sorte:

```
<! DOCTYPE html>
<Html>

</ Html>
```
Tout ce qui entre ```<html>``` et ```</ html>``` sera considéré comme un code HTML. Sans ces balises, il est possible que les navigateurs puissent interpréter incorrectement votre code HTML et présenter le contenu HTML de manière inattendue.


## L anatomie html

Avant d'aller de l'avant, uniformisons le vocabulaire que nous utilisons lorsque vous apprendrez le HTML. Voici quelques-uns des termes que vous verrez utilisés dans ce cours:

Supports angulaires - En HTML, les caractères <et> sont connus sous le nom de supports angulaires.
Élément HTML (ou tout simplement, élément) - code HTML qui vit dans des parenthèses.
Étiquette d'ouverture - la première, ou ouverture, balise HTML utilisée pour démarrer un élément HTML.
Clé de fermeture - la deuxième, ou la fermeture, la balise HTML utilisée pour mettre fin à un élément HTML. Les étiquettes de fermeture ont une barre oblique (/) à l'intérieur d'eux.
À l'exception de quelques éléments HTML, la plupart des éléments consistent en une balise d'ouverture et de fermeture.

Dans l'exemple suivant, il existe un élément de paragraphe composé d'une étiquette d'ouverture (<p>) et d'une balise de fermeture (</ p>):

<P> Bonjour, là-bas! </ P>

## Le HEAD
Jusqu'à présent, vous avez déclaré au navigateur le type de document qu'il peut attendre (un document HTML) et ajouté l'élément HTML (<html>) qui contiendra le reste de votre code. Donnez également au navigateur des informations sur la page. Nous pouvons le faire en ajoutant un élément <head>.
L'élément <head> contiendra des informations sur la page qui n'est pas affichée directement sur la page Web actuelle (vous verrez un exemple dans l'exercice suivant)

### Exemple
```
<!DOCTYPE html>
<html>
  <head>
    <title>My Coding Journey</title>
  </head>
  <body>
  </body>
</html>
```
Quel type d'information sur la page Web peut contenir l'élément ```<head>```?

Eh bien, si vous regardez le haut de votre navigateur (ou à l'un des onglets que vous avez peut-être ouvert dans cette fenêtre du navigateur), vous remarquerez les mot HTMLCSS, qui est le titre de cette page Web.

Le navigateur affiche le titre de la page car le titre peut être spécifié directement à l'intérieur de l'élément ```<head>```, en utilisant un élément ```<title>```.
```
<! DOCTYPE html>
<html>
    <title> Mon titre </title>
  </head>
</html>
```
Si nous devions ouvrir un fichier contenant le code HTML dans l'exemple ci-dessus, le navigateur afficherait les mots Mon titre dans la barre de titre (ou dans le titre de l'onglet).

## le corps de la page

Nous avons ajouté du HTML, mais nous n'avons toujours pas vu de résultats dans le navigateur Web à droite. Pourquoi donc?

Avant de pouvoir ajouter du contenu qu'un navigateur affiche, nous devons ajouter un corps au fichier HTML. Une fois que le fichier a un corps, de nombreux types de contenu peuvent être ajoutés dans le corps, comme le texte, les images, les boutons et bien plus encore
```
<! DOCTYPE html>
<html>
   <head>
    <title> J'apprends à coder! </title>
  </head>
  <body>
  </body>
</html>
```
Tout le code ci-dessus démontre ce qu'on appelle parfois "boilerplate code".

Le terme "boilerplate code" est utilisé pour décrire le code HTML de base requis pour commencer à créer une page Web. Sans tous les éléments du code de référence, vous risquez de démarrer sans les exigences minimales considérées comme les meilleures pratiques.

Remarque: Le reste du cours utilisera des exemples de code comme celui ci-dessus. Pour économiser de l'espace, cependant, les exemples de code évitera d'inclure des éléments communs comme la déclaration, la tête, etc. Sauf indication contraire, vous pouvez supposer que le code dans les blocs de code d'exemple appartient directement au corps du fichier HTML.

## Quelle que clarification

Dans la dernière unité, vous avez appris la quantité minimale de code HTML requise pour structurer avec succès une page Web, parfois appelée "boilerplate".

Nous avons ajouté une déclaration, une tête, un titre et un corps, mais nous avons encore du contenu que le navigateur peut afficher. Dans cette unité, nous allons apprendre à utiliser certains des éléments HTML les plus courants qui ajoutent du contenu aux pages Web.

Gardez à l'esprit que HTML a été créé à l'origine pour marquer ou présenter un texte. Les premières unités de ce cours se concentreront uniquement sur la façon dont HTML peut être utilisé pour marquer le texte. Plus tard dans le cours, nous allons plonger plus profondément dans des techniques de style plus avancées à l'aide de CSS.

Commençons!

## Les titres 

Les rubriques en HTML peuvent être comparées aux en-têtes d'autres types de médias. Par exemple, dans les journaux, de larges titres sont généralement utilisés pour attirer l'attention du lecteur. D'autres fois, les titres sont utilisés pour décrire le contenu, comme le titre d'un film ou un article éducatif.
HTML, il existe six rubriques différentes ou des éléments de titre. Les rubriques peuvent être utilisées à des fins diverses, comme des sections de titres, des articles ou d'autres formes de contenu.

Voici la liste des éléments de titre disponibles en HTML. Ils sont commandés de la plus grande à la plus petite taille.

```<h1>```
utilisé pour les rubriques principales, toutes les autres rubriques plus petites sont utilisées pour les sous-positions.
 ```
<h2>
<h3>
<h4>
<h5>
<h6>
```
Le code d'exemple suivant utilise un titre destiné à attirer l'attention du lecteur. Il utilise le plus grand titre disponible, l'élément de titre principal:
<h1>SALUT les gens</h1>

## Les Paragraphes

Souvent, les titres sont destinés à accentuer ou à agrandir seulement quelques mots.

Si vous souhaitez ajouter du contenu au format des paragraphes, vous pouvez ajouter un paragraphe en utilisant l'élément de paragraphe <p>.


 ## Les listes 

 ### List non ordonnees
  
Souvent, il est préférable d'afficher certains types de contenu dans une liste facile à lire.

En HTML, vous pouvez utiliser la liste non ordonnée pour le texte que vous décidez de formater en points de balle. Une liste non ordonnée décrit les éléments de la liste individuelle avec un point de balle. Vous avez probablement utilisé une liste non ordonnée lors de l'inscription d'une liste d'épicerie ou d'une liste de fournitures scolaires.

Pour créer une liste non ordonnée à l'aide de HTML, vous pouvez utiliser l'élément ```<ul>```. L'élément ```<ul>```, cependant, ne peut pas contenir du texte brut et ne peut pas automatiquement formater le texte brut avec des points de balle. Les éléments de la liste individuelle doivent être ajoutés à la liste non ordonnée à l'aide de l'élément ```<li>```.

```
<ul>
  <li> Limes </li>
  <li> Tortillas </li>
  <li> Poulet </li>
</ul>
```
Dans l'exemple ci-dessus, la liste a été créée à l'aide de l'élément <ul> et tous les éléments de la liste individuelle ont été ajoutés en utilisant les éléments <li>.


## Les listes ordonnees

Bon travail! Certaines listes, cependant, nécessiteront un peu plus de structure. HTML fournit la liste commandée lorsque vous avez besoin d'un ordre supplémentaire que les listes non ordonnées ne fournissent pas.

Les listes commandées sont comme des listes non ordonnées, sauf que chaque élément de liste est numéroté. Vous pouvez créer la liste commandée avec l'élément <ol>, puis ajouter des éléments de liste individuels à la liste en utilisant les éléments <li>.

<ol>
  <li> Préchauffez le four à 350 degrés. </li>
  <li> Mélanger la farine de blé entier, le bicarbonate de soude et le sel. </li>
  <li> Crème au beurre, sucre dans un bol séparé. </li>
  <li> Ajouter les oeufs et l'extrait de vanille dans li bol. </li>
</ol>


## lien encrage
Vous pouvez ajouter des liens vers une page Web en ajoutant un élément d'ancrage <a> et incluant le texte du lien entre les balises d'ouverture et de fermeture.
ceci est lien vers Wikipedia
```<a>wikipedia</a>```
L'élément d'ancrage dans l'exemple ci-dessus est incomplet sans l'attribut href.

Vous pouvez ajouter des liens vers une page Web en ajoutant un élément d'ancrage <a> et incluant le texte du lien entre les balises d'ouverture et de fermeture.

```<a> Ceci est un lien vers Wikipedia </a>```
Attends une minute! Techniquement, le lien dans l'exemple ci-dessus est incomplet. Comment est exactement le lien ci-dessus supposé fonctionner s'il n'y a pas d'URL qui conduira les utilisateurs à la page actuelle de Wikipédia?

L'élément d'ancrage dans l'exemple ci-dessus est incomplet sans l'attribut href.

Les attributs fournissent encore plus d'informations sur le contenu d'un élément. Ils vivent directement à l'intérieur de la balise d'ouverture d'un élément. Les attributs sont composés des deux parties suivantes:

Le nom de l'attribut.
La valeur de l'attribut.
Pour les éléments d'ancrage, le nom de l'attribut est href et sa valeur doit être définie sur l'URL de la page que vous souhaitez que l'utilisateur visite.

```<a href="https://www.wikipedia.org/">``` Ceci est un lien vers Wikipedia ```</a>```
Dans l'exemple ci-dessus, l'attribut href a été défini sur la valeur de l'URL correcte https://www.wikipedia.org/. L'exemple montre maintenant l'utilisation correcte d'un élément d'ancrage.

### exercices

Ajoutez un lien qui indique: En savoir plus. N'ajoutez pas l'URL pour le moment.
Ajouter ce url sur le lien 
https://wikipedia.org

## Attributes des lien


Avez-vous déjà cliqué sur un lien et avez-vous observé la page Web qui s'avançait dans une nouvelle fenêtre? Dans l'affirmative, vous pouvez remercier l'attribut target de l'élément d'ancrage.

L'attribut target spécifie qu'un lien doit s'ouvrir dans une nouvelle fenêtre.
Pour un lien à ouvrir dans une nouvelle fenêtre, l'attribut target requiert une valeur de _blank. L'attribut cible peut être ajouté directement à la balise d'ouverture de l'élément d'ancrage, tout comme l'attribut href 
exemple ```<a href="https://Wikipedia.org" target="_blank">wikipedia</a>```
## Images

All of the elements you've learned about so far (headings, paragraphs, lists, and links) all share one thing in common: they're composed entirely of text! What if you want to add content to your web page that isn't composed of text, like images?
L'élément ```<img>``` vous permet d'ajouter des images à une page Web. Cet élément est spécial car il n'a pas de balise de fermeture, il n'a qu'une balise d'ouverture. C'est parce que l'élément ```<img>``` est un élément à fermeture automatique.
```
<img src="https://www.example.com/picture.jpg" />
```
Notez que l'élément ```<img>``` a un attribut requis appelé src, qui est similaire à l'attribut href dans les liens. Dans ce cas, la valeur de src doit être l'URL de l'image. Notez également que la fin de l'élément ```<img>``` a une barre oblique /. Ceci est nécessaire pour un élément à fermeture automatique.

Une partie d'un développeur Web exceptionnel rend votre site accessible aux utilisateurs de tous horizons. Plus précisément, les utilisateurs malvoyants nécessitent plus de soutien de votre page Web afin qu'ils puissent expérimenter le contenu de votre page.

HTML aide les utilisateurs malvoyants avec l'attribut ```alt```.

L'attribut alt est appliqué spécifiquement à l'élément ```<img>```. La valeur de alt doit être une description de l'image.

```<img src = "#" alt = "Un champ de tournesols jaunes" />```
Les attributs alt servent également aux fins suivantes:

Si une image ne parvient pas à charger sur une page Web, un utilisateur peut passer la souris sur la zone initialement destinée à l'image et lire une brève description de l'image. Cela est possible grâce à la description que vous fournissez dans l'attribut alt.
Les utilisateurs malvoyants naviguent souvent sur le Web à l'aide d'un logiciel de lecture d'écran. Lorsque vous incluez l'attribut alt, le logiciel de lecture d'écran peut lire la description de l'image sur l'utilisateur malveillant.
Remarque: Si l'image sur la page Web n'est pas celle qui transmet toute information significative à un utilisateur (malvoyant ou autrement), l'attribut alt ne doit pas être utilisé.

## Rupture de line 
Vous avez vu comment la modification de l'espacement entre le code dans un fichier HTML n'affecte pas le positionnement des éléments dans le navigateur. Si vous souhaitez modifier l'espacement dans le navigateur, vous pouvez utiliser l'élément de rupture de ligne HTML: ```<br />```.

L'élément de rupture de ligne est une balise à fermeture automatique. Vous pouvez l'utiliser n'importe où dans votre code HTML et une pause de ligne sera affichée dans le navigateur.
Remarque: les sauts de ligne ne sont pas la manière standard de manipuler le positionnement des éléments HTML, mais il est probable que vous les rencontrerez de temps en temps. Dans les unités ultérieures, vous apprendrez des techniques plus avancées pour le positionnement des éléments HTML.

## Indentation
Whitespace rend le code plus facile à lire en augmentant (ou en diminuant) l'espacement entre les lignes de code. Pour rendre la structure du code plus facile à lire, les développeurs Web utilisent souvent l'indentation.

Le World Wide Web Consortium (W3C) est responsable du maintien des normes de style HTML. Au moment de l'écriture, le W3C recommande 2 espaces d'indentation lors de l'écriture du code HTML. L'indentation est destinée à des éléments imbriqués dans d'autres éléments.
```
<ul>
  <li> Violon </li>
  <li> Viola </li>
  <li> Violoncelle </li>
  <li> Bass </li>
<ul>
```
Dans l'exemple ci-dessus, les éléments de la liste sont indentés avec deux espaces. Les espaces sont insérés à l'aide de la barre d'espace de votre clavier. Sauf si votre éditeur de texte a été configuré correctement, la touche ```"TAB"``` de votre clavier ne doit pas être utilisée pour l'indentation.

## Les Commentaires

Les fichiers HTML vous permettent également d'ajouter des commentaires à votre code.

Les commentaires commencent par ``` <! - et se terminent par ->```. Tous les caractères intermédiaires seront traités comme un commentaire.

```<! - C'est un commentaire que le navigateur n'apparaîtra pas. ->```
L'inclusion de commentaires dans votre code est utile pour de nombreuses raisons:

Ils vous aident (et d'autres) à comprendre votre code si vous décidez de revenir et de l'examiner à une date plus tardive.
Ils vous permettent d'expérimenter un nouveau code sans avoir à supprimer un ancien code.
```<! - Section des films préférés ->```
<P> Voici une liste de mes films préférés: </ p>
Dans l'exemple ci-dessus, le commentaire sert à indiquer que le texte suivant constitue une section particulière de la page.

```<! - <a href = "#" target = "_ blank>Facebook</a> ->```
Dans l'exemple ci-dessus, un élément HTML valide (un élément d'ancrage) a été "commenté". Cette pratique est utile lorsque vous souhaitez expérimenter un nouveau code sans avoir à supprimer un ancien code.



***Félicitations*** pour avoir complété la deuxième unité de HTML et CSS! Dans cette unité, vous avez appris comment ajouter du contenu à une page Web en utilisant certains des éléments HTML les plus courants.

***Examinons ce que vous avez appris jusqu'ici:***

Vous pouvez ajouter des titres de différentes tailles en utilisant les différents éléments de la rubrique: ```<h1> à <h6>```.
Les paragraphes sont ajoutés avec l'élément ```<p>```.
Les listes non classées sont créées avec l'élément ```<ul>``` et les éléments de liste sont ajoutés à l'aide de l'élément ```<li>```.
Les listes commandées sont créées avec l'élément ```<ol>``` et les éléments de liste sont ajoutés à l'aide de l'élément ```<li>```.
Vous pouvez ajouter des liens vers votre page Web à l'aide de l'élément ```<a>```, n'oubliez pas l'attribut href!
Les images peuvent être ajoutées avec l'élément ```<img>``` - n'oubliez pas l'attribut src!
Les images aident les utilisateurs malvoyants lorsque les éléments ```<img>``` incluent l'attribut alt.
Vous pouvez transformer n'importe quoi en un lien en l'enveloppant avec un élément ```<a>```.
L'espace blanc dans le fichier HTML n'affecte pas le positionnement des éléments dans le navigateur.
Le W3C recommande 2 espaces d'indentation pour les éléments HTML imbriqués.
Les commentaires sont utilisés pour prendre des notes dans un fichier HTML. Vous pouvez ajouter un commentaire avec ```<! - C'est un commentaire ->```.
Jusqu'à présent, le contenu que vous avez ajouté dans cette unité n'est pas très attrayant visuellement. Dans l'unité suivante, vous apprendrez à modifier l'apparence de votre contenu à l'aide de CSS.

## La configuration css
### Qu'est-ce que CSS?
Jusqu'à présent, vous avez appris les principes fondamentaux du HTML, y compris la structure de base requise pour configurer les fichiers HTML, ainsi que les éléments HTML communs utilisés pour ajouter du contenu à une page Web.

Malheureusement, les éléments HTML que nous avons utilisés pour ajouter du contenu à une page Web ont entraîné des résultats assez fous dans le navigateur. Par exemple, il semble que tout le contenu semble être de la même couleur, avoir la même police et n'offrir aucun contrôle direct sur la taille de la police (en dehors des six options d'en-tête différentes). Comment rendre notre HTML plus attrayant visuellement?

CSS ou Cascading Style Sheets, est un langage que les développeurs Web utilisent pour classer le contenu HTML sur une page Web. Si vous souhaitez modifier les couleurs, les types de polices, les tailles de police, les ombres, les images, le positionnement des éléments, etc., CSS est l'outil pour le travail!

Dans cette unité, vous apprendrez d'abord comment intégrer CSS afin que vous puissiez style du contenu. Vous découvrirez également la structure de base de CSS et apprenez à utiliser sa syntaxe. Dans les unités ultérieures, nous explorerons en détail comment modifier la couleur, les options de police et bien plus encore.

## Commençons!
Bien que CSS soit un langage différente de HTML, il est possible d'écrire un code CSS directement dans un fichier HTML. Ceci est possible en raison de l'élément ```<style>``.

L'élément ```<style>``` vous permet d'écrire un code CSS entre ses balises d'ouverture et de fermeture. Pour utiliser l'élément ```<style>```, il doit être placé à l'intérieur de ```<head>```.

```
<head>
  <style>

  </style>
</head>
```
Une fois que ```<style>``` est placé dans la ```<head>``` de la page Web, nous pouvons commencer à écrire le code CSS.
```
<head>
  <style>
    h2 {
     font-family: Arial;
    }
  </style>
</head>
```
Ne vous inquiétez plus pour le code CSS dans l'exemple ci-dessus, vous en apprendrez plus sur les détails du code CSS dans les leçons suivantes


## Structure vs Style
Bien que l'élément ```<style>``` vous permet d'écrire un code CSS dans des fichiers HTML, ce mélange de HTML et CSS peut entraîner un code difficile à lire et à conserver.

Il est courant pour les développeurs d'ajouter des quantités substantielles de style CSS personnalisé à une page Web. Lorsque tout ce code CSS est placé dans un élément ```<style>``` dans un fichier HTML, vous risquez les deux choses suivantes:

Création d'un grand fichier HTML difficile à lire et à gérer (par vous et d'autres développeurs). Dans l'ensemble, cela peut entraîner un flux de travail inefficace.
Maintenir une distinction claire entre la structure de la page Web (HTML) et le style de page Web (CSS)


## Le fichier .css
Heureusement, la solution suivante vous aidera à éviter de créer de gros fichiers HTML qui mélangent le code CSS: un fichier CSS!

Les fichiers HTML ne contiennent que le code HTML. De même, les fichiers CSS sont censés contenir uniquement un code CSS. Vous pouvez créer un fichier CSS en utilisant l'extension de nom de fichier .css, de la manière suivante: ```style.css```

Avec un fichier CSS, vous pouvez écrire tout le code CSS nécessaire au style d'une page sans avoir à sacrifier la lisibilité et la facilité d'entretien de votre fichier HTML.

## Liaison de fichier CSS a un fichier html

Vous pouvez utiliser l'élément ```<link>``` pour lier ensemble les fichiers HTML et CSS. L'élément ```<link>``` doit être placé dans la ```<head>``` du fichier HTML. Il s'agit d'une balise à fermeture automatique et nécessite les trois attributs suivants:

```Href```comme l'élément d'ancrage, la valeur de cet attribut doit être l'adresse ou le chemin d'accès au fichier CSS.
``` type``` Cet attribut décrit le type de document auquel vous vous connectez (dans ce cas, un fichier CSS). La valeur de cet attribut doit être définie sur ```text/css```.
```rel``` Cet attribut décrit la relation entre le fichier HTML et le fichier CSS. Parce que vous vous connectez à une feuille de style, la valeur doit être définie sur la feuille de style.
Lors de la liaison d'un fichier HTML et d'un fichier CSS ensemble, l'élément ```<link>``` ressemble à ce qui suit:

```<link href = "https://www.exemple.com/stylesheets/style.css" type = "text/css" rel = "stylesheet">```
Notez que dans l'exemple ci-dessus, le chemin d'accès à la feuille de style est une URL:

Https://www.exemple.com/stylesheets/style.css
La spécification du chemin d'accès à la feuille de style à l'aide d'une URL est une façon de relier une feuille de style.

## Revoyons: la configuration CSS
Bon travail! Vous avez appris comment lier un fichier HTML et un fichier CSS ensemble.

##  Examinons ce que vous avez appris jusqu'ici:

1. Le HTML et le CSS sont conservés dans des fichiers distincts afin de garder le code lisible , ainsi que de garder la structure séparée du style.

2. L'élément ```<style>``` vous permet d'écrire un code CSS dans un fichier HTML.

3. Une feuille de style CSS peut être liée à un fichier HTML à l'aide de l'élément ```<link>```, qui nécessite trois attributs:

- ```href ``` est égal au chemin d'accès du fichier CSS.
- ```type ``` égal à text/css.
- ```rel ``` égal à la feuille de style.
Dans cette leçon, vous avez appris les deux endroits dans lesquels vous pouvez écrire un code CSS, mais vous n'avez pas écrit de code CSS.

Dans la leçon suivante, vous apprendrez la structure de base et la syntaxe de CSS afin que vous puissiez commencer à utiliser CSS seul.

Si le fichier CSS est stocké dans le même répertoire que votre fichier HTML, vous pouvez spécifier un chemin relatif au lieu d'une URL, de la manière suivante:

```<link href = "/ style.css" type = "text/css" rel="stylesheet">```
L'utilisation d'un chemin relatif est un moyen très courant de lier une feuille de style.

## CSS
Vous avez appris comment séparer HTML et CSS en deux fichiers et les lier ensemble, mais vous n'avez pas appris comment la syntaxe CSS est utilisée pour façonner des éléments sur une page Web.

Dans cette leçon, vous apprendrez la structure de base et la syntaxe de CSS afin que vous puissiez commencer à coiffer les éléments de la page Web.

### Commençons!

## Sélecteurs d'éléments
Nous avons discuté du style des éléments HTML en utilisant CSS, mais comment est-il effectivement fait?

Pour classer un élément HTML à l'aide de CSS, vous devez d'abord sélectionner cet élément dans le fichier CSS. Par exemple, pour créer un élément ```<p>```, la syntaxe pour le sélectionner en utilisant CSS est:

```
p {

}
```
Dans l'exemple ci-dessus, tous les éléments de paragraphe sont sélectionnés à l'aide d'un sélecteur CSS. Le sélecteur (dans ce cas) est ```p```. Notez que le sélecteur CSS correspond essentiellement à la balise HTML de cet élément, mais sans les crochets.

***Remarque***: Le sélecteur ```p``` dans l'exemple ci-dessus sélectionnera tous les éléments ```<p>``` sur la page Web. Plus tard dans ce cours, vous apprendrez à utiliser des sélecteurs CSS plus spécifiques afin que vous puissiez sélectionner n'importe quel élément souhaité.

### Déclarations CSS
Maintenant que vous connaissez les bases de la syntaxe CSS, choisissons certains des éléments de la page Web.

## Sélecteurs multiples
Le style avec CSS serait très inefficace si vous étiez forcé de modifier manuellement la même propriété sur de nombreux éléments.

Par exemple, et si vous vouliez changer la couleur de 10 éléments différents en Aquamarine en CSS?

Heureusement, vous pouvez sélectionner plusieurs éléments à la fois afin que vous puissiez économiser du temps en définissant une propriété partagée.
```
h1, h2, p {
  color: green;
}
```
Dans l'exemple ci-dessus, le titre ```<h1>```, ```<h2>``` et le paragraphe ont tous été conçus pour apparaître en vert à l'aide d'un sélecteur à plusieurs éléments. Un sélecteur à plusieurs éléments peut vous faire gagner du temps lorsque vous souhaitez créer un style identique sur de nombreux éléments.


## Le sélecteur universel
Il existe un sélecteur spécial qui peut sélectionner instantanément chaque élément sur la page Web: le sélecteur universel.

```
* {
  font-family: Arial;
}
```
Dans l'exemple ci-dessus, le sélecteur universel, ```*```, est utilisé pour sélectionner chaque élément sur la page et définir la police dans Arial.

Qu'est-ce qui rend le sélecteur universel si spécial? Lorsque tous les éléments d'une page Web nécessitent le même style, il est souvent plus efficace de définir ce style à l'aide du sélecteur universel. Par la suite, vous pouvez modifier (ou supprimer) ce style pour des éléments spécifiques qui ne l'exigent pas.

Dans une leçon ultérieure, vous utiliserez le sélecteur universel pour vous aider à comprendre comment les éléments HTML sont définis dans le navigateur et comment positionner ces éléments.


## Indentation et espacement
Tout comme HTML, CSS suit certaines pratiques exemplaires pour l'espacement et l'indentation.
```
h1 {
  color :blue;
}

p {
  color: blue;
}
```
Un espace doit être utilisé entre le sélecteur et l'accolade d'ouverture ```({)```.
Il ne devrait pas exister d'espace supplémentaire entre l'ouverture et la fermeture des accolades ```({et})``` et les déclarations CSS (comme dans l'exemple ci-dessus).
Deux espaces d'indentation devraient être utilisés pour les déclarations CSS.
Une ligne d'espacement devrait exister entre les règles CSS. Dans l'exemple ci-dessus, il existe une ligne d'espacement entre la règle CSS pour l'en-tête et la règle CSS pour le paragraphe.
Les fichiers CSS peuvent devenir longs car le style est ajouté à une page Web. L'espacement et l'indentation appropriés permettent de garder le code CSS maintenable et lisible pour vous et d'autres développeurs.

## Les commentaires
Tout comme HTML, vous pouvez également laisser des commentaires dans votre fichier CSS. Les commentaires CSS commencent par ```/ * ``` et se terminent par ```* /```, ainsi:

```/ * Ceci est un commentaire en CSS! * / ```
L'inclusion de commentaires dans votre code est utile pour de nombreuses raisons:

Ils vous aident (et d'autres) à comprendre votre code si vous décidez de revenir et de l'examiner à une date plus tardive.
Ils vous permettent d'expérimenter un nouveau code sans avoir à supprimer un ancien code.
 ```
 / * Style de paragraphe * /
p {
  color: blue;
}
```
Dans l'exemple ci-dessus, un commentaire permet de spécifier le style CSS pour les paragraphes.

```
/ *
h1 {
  color: red;
}
* /
```
Dans l'exemple ci-dessus, une règle CSS valide a été "commentée". Cette pratique est utile lorsque vous souhaitez expérimenter un nouveau code sans avoir à supprimer un ancien code.


## Revoyons: la structure et syntaxe de base de CSS
Bon travail! Vous avez appris les bases de la structure CSS et de la syntaxe. Nous continuerons à bâtir sur ces bases car vous en apprendrez plus sur CSS.

### Examinons ce que vous avez appris jusqu'ici:

1. Un sélecteur CSS cible un élément HTML.

2. Déclarations CSS style éléments HTML. Les déclarations doivent contenir les deux éléments suivants:

Propriété - la propriété que vous souhaitez style.
Valeur - la valeur de la propriété que vous définissez.
3. Les déclarations CSS doivent se terminer par un point-virgule (;)

4. Une règle CSS consiste en un sélecteur CSS et les déclarations à l'intérieur du sélecteur.

5. Les sélecteurs à plusieurs éléments peuvent être utilisés pour modéliser plusieurs éléments à la fois.

6. Les commentaires gardent le code facile à lire et vous permettent d'expérimenter un nouveau code sans devoir enlever l'ancien code.

7. CSS suit certaines pratiques exemplaires pour l'espacement et l'indentation:

Une ligne d'espacement entre un sélecteur et l'accolade d'ouverture.
Pas d'espacement entre les déclarations CSS et les accolades d'ouverture et de fermeture de la règle CSS.
Deux espaces d'indentation pour les déclarations CSS.
Une ligne d'espacement entre les règles CSS.

## Un peu des pratiques

### Le pouvoire des couleurs
Dans la dernière unité, vous avez appris les bases de CSS

Comment lier des fichiers HTML et CSS ensemble
Le fonctionnement de la syntaxe CSS
En chemin, nous avons proposé différentes propriétés des éléments HTML, mais les détails de chaque propriété n'ont pas été expliqués. Par exemple, nous avons changé les couleurs des en-têtes et des paragraphes, mais nous n'avons pas exploré la puissance totale et la polyvalence de la couleur.

Les sites Web professionnels utilisent souvent divers aspects de la couleur afin de créer une expérience utilisateur (UX) visuellement attrayante. Dans cette leçon, vous apprendrez à utiliser CSS pour façonner les pages Web avec des couleurs.

## Commençons!

#### Avant-plan et arrière-plan

Avant de discuter des spécificités de la couleur, il est important de faire deux distinctions sur la couleur. La couleur peut affecter les aspects de conception suivants:

- La couleur du premier plan
- La couleur de fond

La couleur du premier plan est la couleur dans laquelle apparaît un élément. Par exemple, lorsqu'un titre est appelé vert, la couleur de premier plan de l'en-tête a été conçue.

À l'inverse, lorsqu'un titre est conçu de sorte que son arrière-plan apparaît jaune, la couleur d'arrière-plan de l'en-tête a été conçue

Dans CSS, ces deux aspects de conception peuvent être conçus avec les deux propriétés suivantes:

- ``` color ``` Cette propriété classe la couleur de premier plan d'un élément.

- ``` background-color ``` Cette propriété définit la couleur d'arrière-plan d'un élément.

```
  h1 {
  color: Red;
  background-color: Blue;
}

```
Dans l'exemple ci-dessus, le texte de l'en-tête apparaîtra en rouge, et l'arrière-plan apparaîtra en bleu.

## Les couleurs nommées

Au cours des derniers exercices, vous avez vu des exemples CSS qui utilisent des couleurs comme Rouge, Bleu ou Cyan. Dans CSS, ces couleurs sont techniquement connues sous le nom de couleurs nommées. Il y a 147 [colors nommees](http://www.colors.commutercreative.com/grid/).
À ce stade, vous vous demandez peut-être que vous mémorisez la liste des 147 couleurs nommées que CSS offre.
Heureusement, vous n'avez pas à le faire! Il existe de nombreuses ressources disponibles sur Internet qui répertorient toutes les couleurs nommées dans CSS, comme celle que nous vous avons associée ci-dessus. Si vous avez besoin d'une couleur nommée, une recherche Google rapide donnera les résultats que vous recherchez.

Essayons de nouvelles couleurs nommées!

```
p {
  color : Crimson;
  background-color: DarkMagenta;
}

```
## Les couleurs (RGB) en francais (RVB)
Bien que les couleurs nommées fournissent 147 options différentes, cela représente une petite quantité lorsque vous considérez la flexibilité du CSS. Pour profiter de la gamme complète de couleurs que CSS prend en charge, vous avez la possibilité d'utiliser des couleurs (RGB).

Les couleurs RGB (Rouge, Vert, Bleu) offrent l'option de 16 777 216 couleurs possibles. Comment est-ce possible?

Les couleurs RGB fonctionnent en mélangeant différentes quantités de rouge (R), vert (G) et bleu (B). Chaque couleur (R, G ou B) peut prendre 1 des 256 valeurs possibles (entre 0 et 255). Il en résulte 16 777 216 couleurs possibles.

Pour utiliser des couleurs RGB, vous pouvez utiliser la valeur rgb () lors du coiffage d'une couleur.

``` 
h1 {
  color: rgb(123, 20, 233);
  background-color: rgb(99, 21, 127);
}

```

Dans l'exemple ci-dessus, la valeur de la couleur est définie sur rgb (). Les trois nombres entre parenthèses représentent les valeurs pour R, G et B, dans cet ordre. Notez que vous pouvez utiliser rgb () pour les couleurs d'arrière-plan aussi.

Comment pouvez-vous indiquer la couleur des valeurs RVB dans l'exemple ci-dessus? Êtes-vous censé mémoriser 16 777 216 possibilités? Heureusement, non!

Il existe de nombreuses ressources sur Internet connues sous le nom de [color pickers](https://color.adobe.com/create/color-wheel/) qui vous permettent de voir le résultat de différentes valeurs RGB avant de décider d'utiliser une certaine couleur. Si vous avez besoin d'une ressource de sélection de couleur, une recherche Google rapide donnera les résultats que vous recherchez.

``` 
h1 {
  color: RGB(54, 74, 101);
}

p {
  background-color: RGB(23, 108, 10);
}
```


## Les Hex couleurs

Il existe un moyen supplémentaire de spécifier des couleurs dans CSS: les codes de couleurs hexadécimales, souvent appelés ```«codes de couleur hexadécimal»```, pour une courte durée.

Les codes de couleur Hex offrent également 16,777,216 options de couleurs, mais ils suivent une syntaxe différente.

Lors de la spécification d'un mélange de couleurs RGB, les valeurs sont dans la base 10. Les codes de couleur Hex, cependant, utilisent la base 16 ou la base hexadécimale (d'où le nom), pour spécifier des mélanges de couleurs.
```
h1 {
  color: #09AA34;
}
```
Lorsqu'on lit de gauche à droite, chaque groupe de deux caractères répond à une valeur pour rouge, vert et bleu, respectivement. Dans l'exemple ci-dessus, 09 fait référence à la valeur pour le rouge, AA se réfère à la valeur pour le vert et 34 fait référence à la valeur pour le bleu. Tous les codes de couleur hexadécimal commencent par un caractère #.

Existe-t-il une différence entre les valeurs RVB et les codes de couleurs hexadécimales?

Pas vraiment. Les valeurs RVB et les codes de couleurs hexadécimales sont différents pour représenter la même chose: la couleur. Il est possible de convertir en va-et-vient entre les valeurs RVB et les codes de couleurs hexadécimales (les sélectionneurs de couleurs aident souvent cette conversion).

Remarque: Lorsqu'un code de couleur hexadéifférique est entièrement composé de même caractère, la couleur hexadécimal peut être abrégée, de la manière suivante:
```
h1 {
  color: #FFFFFF;
  color: #FFF; /* nous donne la meme couleur */
}

h2 {
  color: #AA33BB;
  color: #A3B; /* nous donne la meme couleur */
}
```

## Les couleurs HLS

La révision actuelle de CSS, CSS3 (au moment de la rédaction de cet article), introduit une nouvelle façon de spécifier des couleurs à l'aide de couleurs HSL.

HSL signifie Hue, Saturation et Lightness. Plus précisément, c'est ce que chacun veut dire:

Hue - le terme technique qui décrit ce que nous entendons comme "couleur". En HSL, la teinte est représentée sur une roue de couleur. Il peut prendre des valeurs comprises entre 0 et 360.
Saturation - la quantité de gris dans une couleur donnée. Dans HSL, la saturation est spécifiée en utilisant un pourcentage entre 0% et 100%. Le pourcentage de 0% représente une nuance de gris, alors que 100% représente une saturation totale.
Légèreté: la quantité de blanc dans une couleur donnée. Semblable à la saturation, la légèreté est spécifiée en utilisant un pourcentage compris entre 0% et 100%. Le pourcentage de 0% représente le noir, alors que 100% représente le blanc. 50% est normal.
Vous pouvez utiliser les couleurs HSL dans votre CSS comme ceci:
```
h1 {
  color: hsl(182, 20%, 50%);
}
```
Notez que l'utilisation de HSL est très similaire à l'utilisation de RGB.

Remarque: Parce que HSL fait partie de CSS3, les navigateurs plus anciens peuvent ne pas l'être. Dans un exercice ultérieur, vous apprendrez comment contourner les problèmes de support pour les couleurs.

## Valeur Alpha: a
Vous avez appris que les codes de couleurs RVB et hexadécimales sont deux méthodes différentes pour représenter la même chose: la couleur. Cependant, il existe une caractéristique que les couleurs RVB supportent que les codes couleur hexadécimal ne soient pas: une opacité.

L'opacité est une mesure de la transparence d'une couleur. Pour modifier l'opacité dans les couleurs RVB, CSS offre la valeur rgba (). Notez la légère différence dans rgb () et rgba ().

Le caractère supplémentaire dans la valeur rgba () est connu sous le nom de valeur alpha. Il représente l'opacité d'une couleur. La valeur alpha peut être un nombre compris entre 0 ou 1, inclus.
```
h1 {
  color: rgba(123, 88, 9, 0.5);
}
```
Dans l'exemple ci-dessus, la valeur alpha a été définie sur 0,5. Ceci indique que la couleur du titre sera réglée à 50% de son opacité normale.

Remarque: La valeur alpha peut également être utilisée pour les couleurs HSL, en utilisant hsla ():
```
h1 {
  color: hsla(239, 45%, 22%, 0.4);
}
```
## Declarations des couleurs

Les couleurs RVB, les codes de couleur hexadélicos et les couleurs HSL offrent aux développeurs Web une quantité extraordinaire d'options de personnalisation des couleurs. Comme ces propriétés deviennent plus avancées, cependant, il est important de garder à l'esprit que tous les utilisateurs ne naviguent pas sur Internet avec le même navigateur, sans parler de la même version d'un navigateur donné.

Comment cela affecte-t-il le développement web? Les révisions plus récentes du HTML et du CSS affectent les anciens navigateurs. Les navigateurs plus anciens, au fil du temps, seront datés (éventuellement obsolètes) et ne pourront pas prendre en charge les nouvelles fonctionnalités CSS. Par exemple, de nombreux navigateurs plus anciens ne supporte pas RGBa, HSL ou HSLa.

Pour cette raison, nous devons inclure des options de couleur redondantes dans notre code CSS qui peuvent répondre à un large éventail de navigateurs différents.

Plus précisément, nous pouvons ajouter plusieurs déclarations de couleur CSS, au cas où le navigateur d'un utilisateur ne peut pas supporter une certaine déclaration.
```
h1 {
  color: rgb(22, 34, 88);
  color: rgba(22, 34, 88, 0.4);
}
```
Dans CSS, la dernière des déclarations multiples prend la priorité. Dans l'exemple ci-dessus, si le navigateur de l'utilisateur prend en charge rgba (), cette couleur sera appliquée à l'en-tête. Si ce n'est pas le cas, CSS utilisera la première déclaration de couleur rgb (), en tant que sauvegarde.

L'utilisation de déclarations redondantes vous permet de prendre en charge autant d'utilisateurs que possible sur plusieurs versions de différents navigateurs Internet.

## Revue: des Couleurs
Bon travail! Vous avez appris à façonner un aspect important de l'expérience utilisateur: la couleur.

Examinons ce que vous avez appris jusqu'ici:
La couleur de premier plan se réfère à la couleur réelle d'un élément, style avec la propriété de couleur.
La couleur d'arrière-plan se réfère à la couleur derrière un élément, avec la propriété de couleur d'arrière-plan.
Il existe 147 couleurs nommées disponibles.
Les couleurs RGB et hexadécimales offrent plus de 16 millions de possibilités de couleurs.
HSL est une nouvelle façon de définir les couleurs dans CSS3.
Vous pouvez modifier l'opacité d'une couleur avec des couleurs RGBa ou HSLa.
Tous les navigateurs ne prennent pas en charge les fonctionnalités CSS plus récentes, comme l'opacité ou HSL, de sorte que des déclarations supplémentaires devraient être faites pour supporter un large public d'utilisateurs.
Il existe de nombreuses ressources de sélection de couleurs disponibles sur Internet pour vous aider à sélectionner des couleurs spécifiques, ainsi que de fournir des couleurs dans différents formats.


## Famille de polices

Si vous avez déjà utilisé un processeur de texte formaté, il est probable que vous avez probablement utilisé une fonctionnalité qui vous a permis de modifier le «type de police» que vous avez tapé. L'expression «type de police» désigne le type de police de caractères technique ou famille de polices.

Pour modifier la police de caractères de votre page Web, vous pouvez utiliser la propriété ``` font-family```.

``` 
h1 {
  font-family: Garamond;
}
```
Dans l'exemple ci-dessus, la famille de polices pour tous les éléments de l'en-tête principal a été définie sur Garamond.

Lorsque vous définissez des caractères sur une page Web, gardez à l'esprit les points suivants:
- La police spécifiée dans une feuille de style doit être installée sur l'ordinateur d'un utilisateur afin que cette police s'affiche lorsqu'un utilisateur visite la page Web. Nous allons apprendre à contourner ce problème lors d'un exercice ultérieur.
- Vous avez probablement remarqué que nous ne spécifions pas une police de caractères dans les exercices précédents de ce cours. Comment le navigateur sait-il exactement quel type d'interface doit utiliser lors de l'affichage de la page Web? La police de caractères par défaut pour tous les éléments HTML est Times New Roman. Vous pouvez être familier avec cette police de caractères si vous avez déjà utilisé un traitement de texte formaté.
- C'est une bonne pratique de limiter le nombre de caractères utilisés sur une page Web à 2 ou 3.
- Lorsque le nom d'une police de caractères comporte plus d'un mot, il doit être placé entre guillemets (sinon il ne sera pas reconnu), de la manière suivante:

``` 
h1 {
  font-family: "Courier New";
}
```
## Serif vs Sans-Serif
La pratique de la typographie existe depuis des siècles! Au fil du temps, les typographes ont raffiné leur métier et ont développé de nombreux types de caractères, ce qui leur a permis, dans certains cas, de les classer comme l'un des deux types suivants: les polices Serif et les polices Sans-Serif.

- Serif: les lettres de ces polices ont des détails supplémentaires sur les extrémités de chaque lettre. Les exemples incluent des polices comme Times New Roman ou Georgia, entre autres.
- Sans-Serif: les lettres de ces polices n'ont pas de détails supplémentaires sur les extrémités de chaque lettre. Au lieu de cela, les lettres ont des bords droits et plats. Quelques exemples incluent Arial ou Helvetica.

La plupart des polices que nous allons étudier dans cette leçon seront soit des fontes serif ou sans serif.
