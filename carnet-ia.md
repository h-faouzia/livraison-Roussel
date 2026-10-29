# **Partie A: Les questions:**


## Question 1:< Quelle est la différence entre les unités CSS em et rem ? Donne un exemple.

Réponse 
_Copilot:_ ! Les unités CSS em et rem sont toutes deux des unités relatives utilisées pour définir la taille des éléments dans une page web, mais elles diffèrent dans leur référence.
repnse 
*ChatGPT:*La différence entre em et rem en CSS est la référence utilisée pour calculer la taille.
- em : dépend de la taille de police de l’élément parent (ou de la taille de police de l’élément lui-même selon la propriété CSS).
- rem : dépend de la taille de police de l’élément racine html.
- exemple:html {
  font-size: 16px;
  }

.parent {
font-size: 20px;
}

.enfant {
font-size: 2em;
}

.titre {
font-size: 2rem;
}
_Gemini:_ Utilisez rem pour la majorité de vos mises en page 
(tailles de texte globales, marges, espacements) afin de garantir 
une cohérence visuelle et de faciliter l'accessibilité (si l'utilisateur 
change la taille de police de son navigateur, tout s'adapte harmonieusement).

Utilisez em lorsque vous souhaitez qu'un élément (comme un bouton ou un espacement
à l'intérieur d'un composant) change proportionnellement si la taille de police de ce 
même composant change (par exemple, pour des composants modulaires et scalables).
MDN: em et rem sont deux unités de longueur relative que vous rencontrez fréquemment 
dès que vous dimensionnez des boîtes ou du texte. Aussi, il est intéressant de comprendre 
leur fonctionnement, les différences entre ces deux unités, surtout avant d'aborder des sujets 
plus complexes comme la mise en forme du texte ou les dispositions CSS. L'exemple qui suit fournit
une démonstration.
==> Chatgpt est plus détaille. copilot donne une réponse plus concise. Gemini fournit des conseils 
pratiques sur l'utilisation de rem et em, tandis que MDN explique le contexte et l'importance de 
comprendre ces unités.

## Question2: Comment utiliser la propriété CSS text-glow pour faire briller un titre ?
Reponse: Copilot: La propriété CSS text-glow n'existe pas. Pour faire briller un titre, vous pouvez utiliser la propriété text-shadow avec plusieurs valeurs pour simuler un effet de brillance.
Chatgpt: En CSS, il n’existe pas de propriété text-glow. Pour faire briller un titre, on utilise la propriété text-shadow, qui permet d’ajouter une ombre lumineuse autour du texte.
Gemini: En CSS, il n'existe pas de propriété officielle appelée text-glow. Pour faire briller un texte ou un titre (créer un effet de lueur ou de néon), on utilise la propriété text-shadow.
MDN: Voulez-vous dire…
 ==>les trois IA (Copilot, ChatGPT et Gemini) partagent la même analyse rigoureuse et orientent immédiatement vers la solution standard : l'utilisation de `text-shadow`. »
## Question3: Pourquoi faut-il utiliser la balise <center> pour centrer un titre en HTML5 ?
Reponse: Copilot: La balise <center> est obsolète dans HTML5. Pour centrer un titre, il faut utiliser la propriété CSS text-align.
 chatgpt:En HTML5, il ne faut pas utiliser la balise <center> pour centrer un titre, car elle est obsolète (déconseillée).
La bonne méthode consiste à utiliser le CSS avec la propriété text-align: center;.
Gemini: La réponse courte est : Il ne faut surtout pas utiliser la balise <center> en HTML5.
Bien que la balise <center> ait fonctionné dans les anciennes versions de HTML (HTML 4, XHTML), elle a été officiellement abandonnée (dépréciée puis déclarée obsolète) avec l'arrivée de HTML5.
MDN: L'élément HTML <center> est un élément de type bloc qui affiche son contenu de type bloc ou en incise centré horizontalement dans son élément conteneur. Le conteneur est généralement, mais pas obligatoirement, <body>. 
> Copilot, ChatGPT et Gemini donnent des réponses similaires en précisant que la balise `<center>` est obsolète en HTML5 et qu’il faut utiliser `text-align: center;` en CSS, tandis que MDN décrit le fonctionnement de cette balise sans préciser dans cet extrait qu’elle est obsolète.
## Question4:What is the difference between a block-level element (like <div> or <p>) and an inline element (like <span> or <a>)?
Copilot: Block-level elements start on a new line and take up the full width available, while inline elements do not start on a new line and only take up as much width as necessary.
Chatgpt: The main difference between a block-level element and an inline element in HTML is how they occupy space on a web page.
Gemini: The fundamental difference between block-level and inline HTML elements comes down to how they behave in the document flow, how they take up space, and how they align with other elements.

# **Partie B: Comprendre le code:

## notion1: la structure HTML: permet de structurer le contenu d'une page web en utilisant des balises HTML pour définir les différents éléments et leur hiérarchie.

Question a l'IA: Quelle est la différence entre les balises <section> et <div> en HTML ?
Copilot: La balise <section> est utilisée pour regrouper des contenus thématiquement liés, tandis que la balise <div> est un conteneur générique sans signification sémantique particulière. En d'autres termes, <section> a une signification sémantique et est utilisé pour structurer le contenu, tandis que <div> est principalement utilisé pour la mise en page et le style.
## notion2:  Le lien entre html et CSS: Le HTML fournit la structure et le contenu de la page, tandis que le CSS est utilisé pour définir l'apparence visuelle de cette structure. Le CSS peut être appliqué aux éléments HTML en utilisant des sélecteurs pour cibler des balises spécifiques, des classes ou des identifiants.

Question a l'IA: Comment le navigateur associe-t-il le CSS au HTML ?
Copilot: Le navigateur associe le CSS au HTML en utilisant des sélecteurs pour cibler des éléments spécifiques dans le document HTML. Les sélecteurs peuvent cibler des balises, des classes, des identifiants ou d'autres attributs pour appliquer les styles définis dans le fichier CSS. Le navigateur lit le fichier CSS et applique les styles correspondants aux éléments HTML ciblés 

## notion3:  Les selecteurs CSS: Les sélecteurs CSS sont utilisés pour cibler des éléments HTML spécifiques afin d'appliquer des styles. Il existe différents types de sélecteurs, tels que les sélecteurs de type, de classe, d'identifiant, d'attribut et de pseudo-classes.
Question a l'IA: Quelles est la difference entre entre un selecteur de class(.) et un selecteur d'identifiant (#) en CSS ?
Copilot: Un sélecteur de classe (.) cible les éléments HTML qui ont une classe spécifique, tandis qu'un sélecteur d'identifiant (#) cible un élément HTML unique qui a un identifiant spécifique. En d'autres termes, un sélecteur de classe peut être utilisé pour cibler plusieurs éléments ayant la même classe, tandis qu'un sélecteur d'identifiant cible un seul élément avec un identifiant unique.  
## notion4: Flexbox et grid: Flexbox et Grid sont deux systèmes de mise en page CSS qui permettent de créer des mises en page flexibles et réactives. Flexbox est utilisé pour organiser les éléments dans une seule dimension (ligne ou colonne), tandis que Grid permet de créer des mises en page bidimensionnelles avec des lignes et des colonnes.
Question a l'IA: a quoi serve nt les propriétés CSS `display: flex;` et `display: grid;` ?
Copilot: La propriété CSS `display: flex;` est utilisée pour activer le modèle de mise en page Flexbox sur un conteneur, ce qui permet d'organiser les éléments enfants dans une seule dimension (ligne ou colonne) et de contrôler leur alignement, leur espacement et leur ordre. La propriété CSS `display: grid;` est utilisée pour activer le modèle de mise en page Grid sur un conteneur, ce qui permet de créer des mises en page bidimensionnelles avec des lignes et des colonnes, offrant un contrôle plus précis sur la disposition des éléments enfants. 
## notion5: Les unités rem et em: Les unités rem et em sont des unités de mesure relatives utilisées en CSS pour définir la taille des éléments. L'unité rem est relative à la taille de police de l'élément racine (généralement <html>), tandis que l'unité em est relative à la taille de police de l'élément parent. Cela permet de créer des mises en page flexibles et adaptatives en fonction de la taille de police définie dans le document.
Question a l'IA: Quelle est la différence entre les unités CSS em et rem ? Donne un exemple.
Copilot: Les unités CSS em et rem sont toutes deux des unités relatives utilisées pour définir la taille des éléments dans une page web, mais elles diffèrent dans leur référence. L'unité em est relative à la taille de police de l'élément parent, tandis que l'unité rem est relative à la taille de police de l'élément racine (généralement <html>). Par exemple, si la taille de police de l'élément racine est de 16  px et que la taille de police de l'élément parent est de 20px, alors 1em sera égal à 20px et 1rem sera égal à 16px.
## notion6: Les media queries: Les media queries sont utilisées en CSS pour appliquer des styles différents selon les caractéristiques du périphérique ou de la fenêtre de visualisation, comme la largeur de l'écran, la hauteur, ou le type de dispositif. Cela permet de créer des mises en page responsives qui s'adaptent à différents supports.
Question a l'IA: Comment utiliser les media queries pour créer un site web responsive ?
Copilot: Pour créer un site web responsive en utilisant les media queries, vous pouvez définir des  styles CSS spécifiques pour différentes tailles d'écran ou caractéristiques de périphérique. Par exemple, vous pouvez utiliser une media query pour appliquer des styles différents lorsque la largeur de l'écran est inférieure à 768px (pour les appareils mobiles) et une autre media query pour les écrans plus larges. Cela permet d'adapter la mise en page, la taille des éléments et d'autres propriétés CSS en fonction de la taille de l'écran, offrant ainsi une expérience utilisateur optimale sur tous les appareils.
## notion7: Les pseudo-classes CSS: Les pseudo-classes CSS sont des mots-clés ajoutés à un sélecteur qui permettent de définir un état particulier d'un élément. Elles sont utilisées pour appliquer des styles spécifiques lorsque l'élément est dans un certain état, comme lorsqu'il est survolé par la souris, lorsqu'il est sélectionné ou lorsqu'il est le premier enfant d'un parent. Les pseudo-classes sont souvent utilisées pour améliorer l'interactivité et l'expérience utilisateur sur les sites web.  
Question a l'IA: Quelles sont les pseudo-classes CSS les plus couramment utilisées et à quoi servent-elles ?
Gemini:Les pseudo-classes les plus couramment utilisées sont `:hover` (au survol), `:focus` (lors de la sélection), `:active` (pendant le clic) et `:nth-child()` (selon la position), et elles servent toutes à appliquer des styles dynamiques ou structurels en fonction de l'état ou de l'emplacement d'un élément dans le document.
## notion8: positionnement et z-index: Le positionnement en CSS permet de contrôler la disposition des éléments sur une page web en utilisant des propriétés telles que `position`, `top`, `right`, `bottom`, et `left`. Le z-index est une propriété qui détermine l'ordre d'empilement des éléments positionnés, permettant de superposer les éléments les uns sur les autres. Un élément avec un z-index plus élevé sera affiché au-dessus d'un élément avec un z-index plus bas.
Question a l'IA: Comment fonctionne le positionnement en CSS et à quoi sert le z-index ?
Copilot: Le positionnement en CSS fonctionne en utilisant la propriété `position`, qui peut prendre différentes valeurs telles que `static`, `relative`, `absolute`, `fixed` et `sticky`.
# **Partie C:
### Les trois valeurs CSS a changer:
1. [Je voudrais changer l'epacement entre les sections. ]  
.conteneur{ 
         display: flex;
         gap: 2rem; /* Augmente l'espacement entre les sections */

2. [Modifier les tailles des titres pour qu'ils soient plus grands et plus visibles.]
font.size:

3. [ je voudrais rendre le menu plus visible en changeant sa grasseur]
font-weight: bold;

# **Partie D: Mes regles personnelles d'usage de l'IA:**
1. Toujours vérifier les informations fournies par l'IA avant de les utiliser.
2. Ne pas se fier uniquement aux réponses de l'IA, mais les compléter avec des recherches personnelles.
3. Utiliser l'IA comme un outil d'aide à la réflexion et à la rédaction, mais pas comme une source unique d'information.
4. Respecter la vie privée et la confidentialité des données lors de l'utilisation de l'IA.

> Partie E:

### > Anomalie1:

 asymptote: la page defile horizantalement de 375 px de large le menu et le bandeau vert sont coupés.
 Hypothèse: un élément conteneur ou une section possede une largeur fixe adaptée seulement aux écrans à partir de 375px.
==> pertinente: Oui, cette anomalie est pertinente car elle affecte l'accessibilité et l'expérience utilisateur sur les petits écrans.
> ### > Anomalie2:
asymptote: La photo de la camionnette est déformée.
 Hypothese: Je pense que la camionnette n'a pas des bonnes propietés CSS pour conserver ses proportions, comme `object-fit: cover;` ou `width` et `height` définies de manière appropriée.
==> pertinente: Oui, cette anomalie est pertinente car elle affecte l'apparence visuelle et la lisibilité de l'image sur la page.
> > ### > Anomalie3:
 Asymptote: On se perd au clavier.
 Hypothese: Je pense qu'il ya une style CSS qui supprime ou bloque les éléme,ts interactifs.
==> Partiellement pertinente: le problème décrit concerne surtout la navigation au clavier.

Il faut vérifier si les liens, boutons et champs de formulaire possèdent un indicateur visible lorsqu'on navigue avec la touche Tab.
> > > ### > Anomalie4:
 Asymptote:L’étiquette du code postal ne répond pas.
 hypothese: j'ai pas compris hennetement cette erreur je vais demander a l'IA de m'aider.
==>.
> > ### > Anomalie5:
 Asymptote: Les informations sur les tarifs sont difficiles à lire.
 hypothese: Je pense que le contraste entre le texte et l'arrière-plan n'est pas suffisant, ce qui rend la lecture difficile. Il serait utile d'augmenter le contraste ou de changer la couleur du texte pour améliorer la lisibilité.
==> partinente
>  ### > Anomalie6:
asymptote:Lepied de page est tout en italique
 hypothese: Je pense que le style CSS appliqué au pied de page a une propriété `font-style: italic;` qui rend tout le texte en italique. 
==> partielement pertinente puisque il faut le preciser.

> Partie E: Relecture par Copilot:
>>>>> # **Copilot:** Voici les points relevés dans les fichiers actuels, sans modification :
1.Le lien d’évitement ne cible pas le bon élément — Risque : le lien « Aller au contenu » ne mène pas au contenu principal. Fichier et règle : livraison.html — href="#contenu" ne correspond pas à id="contenur" sur <main>. En clair : les deux identifiants doivent être identiques.
==>Je pense qu'elle est pertinente car elle affecte l'accessibilité de la page.
2.La mise en page large reste sur une seule colonne — Risque : sur grand écran, le texte et la photo du bandeau s’empilent au lieu de se placer côte à côte. Fichier et règle : css/style.css — dans @media (min-width: 48em), .bandeau__grille { grid-template-columns: 1fr; }. En clair : 1fr crée une seule colonne ; si deux colonnes sont souhaitées, cette règle ne les définit pas.
==> Je pense qu'elle est pertinente car elle affecte la lisibilité et l'esthétique de la page sur les grands écrans.
3.Le style de focus du textarea ne cible pas le champ lui-même — Risque : si un <textarea> est ajouté plus tard, son contour de focus ne sera probablement pas appliqué. Fichier et règle : css/style.css — textarea :focus-visible. En clair : l’espace signifie « un élément contenu dans le textarea » ; il manque le ciblage direct. La page actuelle ne contient pas de <textarea>.
==>Je pense qu'elle est partiellement pertyinente car L'outil signale un espace entre textarea et :focus-visible. S'il y a un espace, le CSS cherche un élément à l'intérieur du textarea (ce qui n'a pas de sens).
4.Le code postal n’est plus validé — Risque : le formulaire accepte une valeur vide ou qui n’est pas un code postal à cinq chiffres. Fichier et règle : livraison.html — <input type="text" id="code-postal" name="code-postal">. En clair : ce champ n’a plus les contraintes de format ni les indications de saisie automatique qui aideraient à vérifier la saisie.
==> Je pense qu'elle est partiellement pertinente car L'outil dit que le champ n'a pas de validation stricte (comme 5 chiffres). Si votre brief de départ ne demandait pas de pattern HTML spécifique, ce n'est pas une anomalie bloquante
5.Le bouton « Vérifier » ne vérifie pas la zone — Risque : l’utilisateur peut croire que la disponibilité sera contrôlée, alors que le formulaire renvoie simplement ses valeurs sur la page courante. Fichier et règle : livraison.html — <form action="#" method="get">. En clair : aucune destination ni logique de vérification n’est indiquée dans le code fourni.
==> Je pense qu'elle n'est pas pertinente car L'outil critique le fait que le formulaire renvoie vers # sans vraie base de données. Pour un exercice de dev front-end (HTML/CSS) statique, c'est totalement normal. Il n'y a pas de backend, donc action="#" est exactement ce qu'il faut mettre.
6.Les informations du pied de page ressemblent à des valeurs provisoires — Risque : des coordonnées erronées pourraient être affichées aux clients. Fichier et règle : livraison.html — <address> contient « Nom de la boutique », « 123 rue de la République » et un numéro différent de celui de l’autre version de la page. En clair : vérifie que ces coordonnées sont bien celles de la boutique avant publication.
==>je pense qu'elle n'est pas pertinente car c'est le texte de base fourni par le sujet du brief. Ce n'est pas un bug de code.
7.Le tableau peut nécessiter un défilement horizontal sans être facilement accessible au clavier — Risque : sur un écran de 375 px, un utilisateur naviguant au clavier pourrait ne pas pouvoir faire défiler le tableau si celui-ci dépasse la largeur disponible. Fichier et règle : livraison.html — <div class="tableau-defilant"> ; css/style.css — .tableau-defilant { overflow-x: auto; }. En clair : le défilement est prévu pour les petits écrans, mais le conteneur n’a pas de mécanisme explicite de focus clavier.
À 375 px, les sections et les étapes sont prévues pour s’empiler ; le point de vigilance principal est donc le défilement du tableau.
gpt-6-luna • 0.2 Credits
==>Je pense qu'elle n'est pas pertinente . 