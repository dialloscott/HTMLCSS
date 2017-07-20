#Introduction

##Que ce que le html (Definition)

HTML est le langage utilisée pour créer les pages Web que vous visitez tous les jours. Il fournit une manière logique de structurer le contenu des pages Web.
Analysons l'acronyme "HTML", car il contient beaucoup d'informations utile. HTML signifie HyperText Markup Language.

	- Un langage de balisage est un langage informatique qui définit la structure et  la présentation du texte brut.
	- Les langages de balisage fonctionnent en entourant le texte brut avec des informations que l'ordinateur peut interpréter, "marquant" pour le traitement.
	- HyperText est affiché sur un ordinateur ou un périphérique qui permet d'accéder à d'autres textes via des liens, également appelés «hyperliens». En fait, vous avez probablement cliqué sur de nombreux hyperliens sur votre chemin vers d autre d autre site web par exemple quora ou ...

	Dans ce cours, vous apprendrez à utiliser les principes fondamentaux du HTML pour structurer, présenter et lier le contenu. Vous apprendrez également à utiliser CSS, ou Cascading Style Sheets, pour classer le contenu HTML que vous ajoutez aux pages Web.

    ##Commençons!
   Le DocTyping

Un navigateur doit savoir dans quelle langue un document est écrit avant de pouvoir traiter le contenu du document.

Vous pouvez laisser les navigateurs Web savoir que vous utilisez la langue HTML en commençant votre document HTML avec une déclaration de type de document.
Un navigateur doit savoir dans quelle langue un document est écrit avant de pouvoir traiter le contenu du document.

Vous pouvez laisser les navigateurs Web savoir que vous utilisez la langue HTML en commençant votre document HTML avec une déclaration de type de document.

La déclaration est la suivante:

<! DOCTYPE html>
Cette déclaration est une instruction. Il indique au navigateur quel type de document attendre, ainsi que la version HTML utilisée dans le document. <! DOCTYPE html> doit être la première ligne de code dans tous vos documents HTML.

Remarque: Si vous n'utilisez pas la déclaration doctype, votre code HTML fonctionnera probablement, mais il est risqué. À l'heure actuelle, le navigateur supposera correctement que vous utilisez HTML5, car HTML5 est la norme actuelle. À l'avenir, cependant, une nouvelle norme remplacera HTML5. Les futurs navigateurs peuvent supposer que vous utilisez une norme différente et plus récente, auquel cas votre document sera interprété de manière incorrecte. Pour vous assurer que votre document est interprété pour toujours correctement, incluez toujours <! DOCTYPE html> au tout début de vos documents HTML

##Preparation du document 

Génial! Les navigateurs qui lisent votre code savent s'attendre au HTML lorsqu'ils tentent de lire votre fichier.

La déclaration <! DOCTYPE html> n'est que le début, cependant. Il indique seulement au navigateur que vous envisagez d'utiliser HTML dans le document, il n'ajoute pas de structure ou de contenu HTML.

Pour commencer à ajouter de la structure et du contenu HTML, nous devons d'abord ajouter des balises <html> d'ouverture et de fermeture, de la sorte:

<! DOCTYPE html>
<Html>

</ Html>
Tout ce qui entre <html> et </ html> sera considéré comme un code HTML. Sans ces balises, il est possible que les navigateurs puissent interpréter incorrectement votre code HTML et présenter le contenu HTML de manière inattendue.


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

exemple
<!DOCTYPE html>
<html>
  <head>
    <title>My Coding Journey</title>
  </head>
  <body>
  </body>
</html>


Quel type d'information sur la page Web peut contenir l'élément <head>?

Eh bien, si vous regardez le haut de votre navigateur (ou à l'un des onglets que vous avez peut-être ouvert dans cette fenêtre du navigateur), vous remarquerez les mot HTMLCSS, qui est le titre de cette page Web.

Le navigateur affiche le titre de la page car le titre peut être spécifié directement à l'intérieur de l'élément <head>, en utilisant un élément <title>.

<! DOCTYPE html>
<Html>
    <title> Mon titre </ title>
  </ Head>
</ Html>
Si nous devions ouvrir un fichier contenant le code HTML dans l'exemple ci-dessus, le navigateur afficherait les mots Mon titre dans la barre de titre (ou dans le titre de l'onglet).

## le corps de la page

Nous avons ajouté du HTML, mais nous n'avons toujours pas vu de résultats dans le navigateur Web à droite. Pourquoi donc?

Avant de pouvoir ajouter du contenu qu'un navigateur affiche, nous devons ajouter un corps au fichier HTML. Une fois que le fichier a un corps, de nombreux types de contenu peuvent être ajoutés dans le corps, comme le texte, les images, les boutons et bien plus encore.

<! DOCTYPE html>
<html>
   <head>
    <title> J'apprends à coder! </ title>
  </ head>
  <body>
  </ body>
</ Html>
Tout le code ci-dessus démontre ce qu'on appelle parfois "boilerplate code".

Le terme "boilerplate code" est utilisé pour décrire le code HTML de base requis pour commencer à créer une page Web. Sans tous les éléments du code de référence, vous risquez de démarrer sans les exigences minimales considérées comme les meilleures pratiques.

Remarque: Le reste du cours utilisera des exemples de code comme celui ci-dessus. Pour économiser de l'espace, cependant, les exemples de code évitera d'inclure des éléments communs comme la déclaration, la tête, etc. Sauf indication contraire, vous pouvez supposer que le code dans les blocs de code d'exemple appartient directement au corps du fichier HTML.

## Quelle que clarification

Dans la dernière unité, vous avez appris la quantité minimale de code HTML requise pour structurer avec succès une page Web, parfois appelée "boilerplate".

Nous avons ajouté une déclaration, une tête, un titre et un corps, mais nous avons encore du contenu que le navigateur peut afficher. Dans cette unité, nous allons apprendre à utiliser certains des éléments HTML les plus courants qui ajoutent du contenu aux pages Web.

Gardez à l'esprit que HTML a été créé à l'origine pour marquer ou présenter un texte. Les premières unités de ce cours se concentreront uniquement sur la façon dont HTML peut être utilisé pour marquer le texte. Plus tard dans le cours, nous allons plonger plus profondément dans des techniques de style plus avancées à l'aide de CSS.

Commençons!

##Les titres 


Les rubriques en HTML peuvent être comparées aux en-têtes d'autres types de médias. Par exemple, dans les journaux, de larges titres sont généralement utilisés pour attirer l'attention du lecteur. D'autres fois, les titres sont utilisés pour décrire le contenu, comme le titre d'un film ou un article éducatif.
HTML, il existe six rubriques différentes ou des éléments de titre. Les rubriques peuvent être utilisées à des fins diverses, comme des sections de titres, des articles ou d'autres formes de contenu.

Voici la liste des éléments de titre disponibles en HTML. Ils sont commandés de la plus grande à la plus petite taille.

<H1> - utilisé pour les rubriques principales, toutes les autres rubriques plus petites sont utilisées pour les sous-positions.
<H2>
<H3>
<H4>
<H5>
<H6>
Le code d'exemple suivant utilise un titre destiné à attirer l'attention du lecteur. Il utilise le plus grand titre disponible, l'élément de titre principal:
<h1>SALUT les gens</h1>

## Les Paragraphes

Souvent, les titres sont destinés à accentuer ou à agrandir seulement quelques mots.

Si vous souhaitez ajouter du contenu au format des paragraphes, vous pouvez ajouter un paragraphe en utilisant l'élément de paragraphe <p>.


 ## Les listes 

 ``` List non ordonnees
  
Souvent, il est préférable d'afficher certains types de contenu dans une liste facile à lire.

En HTML, vous pouvez utiliser la liste non ordonnée pour le texte que vous décidez de formater en points de balle. Une liste non ordonnée décrit les éléments de la liste individuelle avec un point de balle. Vous avez probablement utilisé une liste non ordonnée lors de l'inscription d'une liste d'épicerie ou d'une liste de fournitures scolaires.

Pour créer une liste non ordonnée à l'aide de HTML, vous pouvez utiliser l'élément <ul>. L'élément <ul>, cependant, ne peut pas contenir du texte brut et ne peut pas automatiquement formater le texte brut avec des points de balle. Les éléments de la liste individuelle doivent être ajoutés à la liste non ordonnée à l'aide de l'élément <li>.

<ul>
  <Li> Limes </ li>
  <Li> Tortillas </ li>
  <Li> Poulet </ li>
</ ul>
Dans l'exemple ci-dessus, la liste a été créée à l'aide de l'élément <ul> et tous les éléments de la liste individuelle ont été ajoutés en utilisant les éléments <li>.


## Les listes ordonnees

Bon travail! Certaines listes, cependant, nécessiteront un peu plus de structure. HTML fournit la liste commandée lorsque vous avez besoin d'un ordre supplémentaire que les listes non ordonnées ne fournissent pas.

Les listes commandées sont comme des listes non ordonnées, sauf que chaque élément de liste est numéroté. Vous pouvez créer la liste commandée avec l'élément <ol>, puis ajouter des éléments de liste individuels à la liste en utilisant les éléments <li>.

<Ol>
  <Li> Préchauffez le four à 350 degrés. </ Li>
  <Li> Mélanger la farine de blé entier, le bicarbonate de soude et le sel. </ Li>
  <Li> Crème au beurre, sucre dans un bol séparé. </ Li>
  <Li> Ajouter les oeufs et l'extrait de vanille dans un bol. </ Li>
</ Ol>


## lien encrage
Vous pouvez ajouter des liens vers une page Web en ajoutant un élément d'ancrage <a> et incluant le texte du lien entre les balises d'ouverture et de fermeture.
ceci est lien vers Wikipedia
<a>wikipedia</a>
L'élément d'ancrage dans l'exemple ci-dessus est incomplet sans l'attribut href.

Vous pouvez ajouter des liens vers une page Web en ajoutant un élément d'ancrage <a> et incluant le texte du lien entre les balises d'ouverture et de fermeture.

<a> Ceci est un lien vers Wikipedia </a>
Attends une minute! Techniquement, le lien dans l'exemple ci-dessus est incomplet. Comment est exactement le lien ci-dessus supposé fonctionner s'il n'y a pas d'URL qui conduira les utilisateurs à la page actuelle de Wikipédia?

L'élément d'ancrage dans l'exemple ci-dessus est incomplet sans l'attribut href.

Les attributs fournissent encore plus d'informations sur le contenu d'un élément. Ils vivent directement à l'intérieur de la balise d'ouverture d'un élément. Les attributs sont composés des deux parties suivantes:

Le nom de l'attribut.
La valeur de l'attribut.
Pour les éléments d'ancrage, le nom de l'attribut est href et sa valeur doit être définie sur l'URL de la page que vous souhaitez que l'utilisateur visite.

<a href="https://www.wikipedia.org/"> Ceci est un lien vers Wikipedia </a>
Dans l'exemple ci-dessus, l'attribut href a été défini sur la valeur de l'URL correcte https://www.wikipedia.org/. L'exemple montre maintenant l'utilisation correcte d'un élément d'ancrage.

```exercices

Ajoutez un lien qui indique: En savoir plus. N'ajoutez pas l'URL pour le moment.
Ajouter ce url sur le lien 
https://wikipedia.org

## Attributes des lien


Avez-vous déjà cliqué sur un lien et avez-vous observé la page Web qui s'avançait dans une nouvelle fenêtre? Dans l'affirmative, vous pouvez remercier l'attribut target de l'élément d'ancrage.

L'attribut target spécifie qu'un lien doit s'ouvrir dans une nouvelle fenêtre.
Pour un lien à ouvrir dans une nouvelle fenêtre, l'attribut target requiert une valeur de _blank. L'attribut cible peut être ajouté directement à la balise d'ouverture de l'élément d'ancrage, tout comme l'attribut href 
exemple <a href="https://Wikipedia.org" target="_blank">wikipedia</a>