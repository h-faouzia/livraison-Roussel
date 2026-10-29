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
==>Voici une phrase pour résumer cela :

> les trois IA (Copilot, ChatGPT et Gemini) partagent la même analyse rigoureuse et orientent immédiatement vers la solution standard : l'utilisation de `text-shadow`. »
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> 
> Partie E:

### > Anomalie1:

> asymptote: la page defile horizantalement de 375 px de large le menu et le bandeau vert sont coupés.
> Hypothèse: un élément conteneur ou une section possede une largeur fixe adaptée seulement aux écrans à partir de 375px.
> ### > Anomalie2:
> 