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