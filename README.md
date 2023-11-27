# 02-GDWFSDVSWEBAJAVAEXAIII1B_262381_20220708161857

### Évaluation d'entraînement - Dynamiser vos sites web avec Javascript

<br>

---

## Projet jeu de dés: 

### **__Livrable Attendu pour l'examen de ce bloc__**

**Création d’un petit jeu sur navigateur web à l’aide du DOM.**

**En fin de prestation, le commanditaire doit recevoir les différents éléments suivants :**

- `Un jeu fonctionnel`

- `Une interface lisible qui correspond à la maquette fournie.`

---
---

<br>
<br>

---

## fonctionnalités globales : 

**En front-desk (côté client) :**

- La possibilité de créer une nouvelle partie

- La possibilité de retenir le score courant

- La possibilité de lancer le dé

- La possibilité d’avoir 2 joueurs

## Modalité pédagogique adoptée

- Fait en Mobile First avec SASS 

=

```
@mixin responsive($key) {
  @if map-has-key($breakpoints, $key) {
    @media screen and (min-width: map-get($breakpoints, $key)) {
      @content;
    }
  } @else {
    @media screen and (min-width: $key) {
      @content;
    }
  }
}
```

---
---

<br>

## Contexte du Projet:

### Règles :

- **[Règles du jeux, voir la page 2 contexte projet!](./dynamiser-js.pdf)**

<br>

---
---

---

- Dépôt git avec commit réguliers

- le code sera structuré

- Le jeu devra être fonctionnel

- Les ressources seront disponibles dans un dossier images

    - La font sera Lato (google font) : https://fonts.google.com/specimen/Lato
    
    - Le Framework CSS de votre choix

=

### Norme de validation stricte pour le référentiel:

```
Ce référentiel suit une norme de validation stricte, également connue sous le nom de 
[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.3/).
Ce guide explique notre approche des types et du format de commit. 
Les clauses doivent suivre une syntaxe stricte pour être correctement traitées par les éléments 
d'automatisation tels que les outils de publication et les sites Web de lecture de code.

Cette norme est toujours conforme à 
[la dernière spécification Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.3/).
```

### format des messages:

Le commit commence par un type, suivi d'une description courte et concise de l'objectif du commit (issue JIRA).
Le type est l'un des types prédéfinis décrits ci-dessous.

<type>(<scope>): <subject>

<body>

<footer>


### Types

Les types de commit suivants sont pris en charge :

* build: Modifications affectant la construction du système ou les dépendances externes
(Exemple scope: Gulp, Brocoli, NPM).

* ci: Changements vers les fichiers et scripts de configuration ci (intégration continue)
(Exemple scope: Travis, Circle, BrowserStack, SauceLabs).

* docs: Un changement de documentation qui n'affecte pas le code.

* feat: une nouvelle fonctionnalité.

* fix: Une correction de code erronée (Bugfix).

* perf: Changements de code qui améliorent les performances.

* refactor: Un changement de code qui ne corrige pas un bogue ou n'ajoute pas de fonctionnalité.

* style: Un changement qui n'affecte pas la signification du code
(format d'espace blanc, format d'indentation, etc.)

* test: Une modification qui ajoute des tests utiles ou manquants, ou qui corrige des tests existants
ou met à jour des structures de test.

* chore: Autres changements qui ne modifient pas le code ou les fichiers de test.

* reverts: retourner ou changer un commit à un état précédent.

#### Ambit (Scope)

Une scope fait référence à la catégorie ou au segment du dépôt qui sera affecté par 
cette validation. 
Ceci est facultatif et dépend du commit (si le commit n'affecte pas le scope du dépôt, le scope
peut être entièrement omise).

#### Sujet

Le sujet doit consister en une seule chaîne courte et impérative décrivant le changement. 
Écrire un sujet à la première personne du présent simple est préférable.
N'ajoutez pas de point à la fin du sujet.

#### Corp

Le corps doit être composé d'une, deux ou trois phrases. 
Le corps peut être utilisé pour donner un contexte supplémentaire, répertorier les limitations,
expliquer le quoi mais pas le comment, répertorier les comportements supplémentaires et 
spécifier la maintenance future.

#### Pie de Page

Les références aux éléments associés, tels que les numéros de issues associés,
sont incluses dans le pied de commit de validation. Le format du pied de commit de validation
doit respecter le modèle suivant : `Closes #Num`.

### Exemples

Ces exemples montrent comment écrire des commits basés sur le type.

```
docs: Documenter l'utilisation correcte du serveur

Nous avons reçu de nombreuses demande de soutien de part des utilisateurs qui utilisent le serveur
incorrectement. Cela documente l'utilisation correcte du serveur.
```

```
feat: ajouté un lecteur vidéo

Un lecteur vidéo a été ajouté afin que les utilisateurs puissent regarder les vidéos du site.
```

```
fix: Correction du bogue du bouton de mise à jour

Parfois, le bouton d'actualisation ne fonctionne pas correctement. Code ajouté pour résoudre ce 
problème.
```

```
refactor: Nous restructurons la structure de la base de données

Nous avons restructuré la structure de la base de données.
```

```
style: Améliorer la lisibilité du code

Plusieurs parties du code ont été refactorisées pour améliorer la lisibilité sans
modifier le comportement.
```

```
test: Ajouter des tests au code existant

Des tests ont été ajoutés à la partie existante du code pour assurer la stabilité de l'application.
```
---

## Barème et critères d’évaluation

```
1. Connaître et utiliser un environnement de développement (2 points):

  VSCode avec plusieurs extensions et plugins:

    - Bem helper pour une bonne html et css

    - Conventional commit + smart commit JIRA

    - CSS Flexbox cheatsheet

    - CSS Grid cheatsheet

    - Error Lens

    - ES Lint

    - Git Graph

    - HTML Hint

    - Live server (évidement)

    - Live preview (mieux que l'autre)

    - Prettier/Prettier ES Lint

    - Quokka (vraiment geniale!!!!❤️❤️)

    - Version Lens ⭐⭐

    - json crack ⭐⭐⭐⭐⭐

    - pretty typescript errors

    - template string converter

```

---

```

2. Écrire un algorithme et l’intégrer dans une page web avec des scripts événementiels et avec un langage de script côté client (5 points).


  Pour écrire un algorithme et l’intégrer dans une page web avec des scripts événementiels et avec un langage de script côté client, je vais utiliser JavaScript (même TypeScript pourquoi pas...  à voir dans le trajet), qui est le langage le plus répandu et le plus standardisé pour le développement web.
  
  Un algorithme est une suite d’instructions logiques qui permet de résoudre un problème ou d’effectuer une tâche (Bucles, iteration, callback, appelle de function, des objets, prototypes, des classe.... etc).
  
  Un script événementiel est un morceau de code qui s’exécute en réponse à un événement déclenché par l’utilisateur ou le navigateur (comme un clic, une saisie, un chargement, etc).
  
  Un langage de script côté client est un langage qui s’exécute dans le navigateur du client, sans avoir besoin de communiquer avec le serveur.
  
  JavaScript remplit ces trois fonctions (depende du contexte peut être aussi node js...).

```  

---

3. Utilisation des normes ECMAScript (JS) et du DOM (5 points):

    1. **Évitez l'utilisation globale** :
    
        - Essayez de garder vos variables dans la portée la plus restreinte possible pour éviter la pollution de l'espace de noms global.

        ---

    2. **Utilisez 'use strict'** :
    
        - Le mode strict peut vous aider à éviter les erreurs courantes en JavaScript.

        ---

    3. **Préférez 'const' et 'let' à 'var'** :
    
        - 'const' et 'let' ont une portée de bloc, tandis que 'var' a une portée de fonction.

        ---

    4. **Utilisez les promesses et async/await pour gérer l'asynchronie** :
    
        - Ils sont plus faciles à raisonner que les callbacks et peuvent vous aider à éviter l'enfer des callbacks.

        ---

    5. **Gérez les erreurs avec try/catch** :
    
        - Cela vous permet de gérer les erreurs de manière plus élégante et d'éviter que votre application ne se bloque.

        ---

    6. **Utilisez la déstructuration d'objets et de tableaux** :
    
        - Cela peut rendre votre code plus propre et plus facile à comprendre.

        ---

    7. **Utilisez les modèles de chaînes pour la concaténation de chaînes** :
    
        - Les modèles de chaînes sont plus lisibles et flexibles que la concaténation de chaînes traditionnelle.

        ---

    8. **Utilisez l'opérateur spread et rest (...)** :
    
        - Ces opérateurs peuvent faciliter le travail avec les tableaux et les objets.

        ---

    9. **Préférez la programmation fonctionnelle lorsque c'est possible** :
    
        - Des choses comme map, filter et reduce peuvent rendre votre code plus propre et plus facile à raisonner.

        ---

    10. **Utilisez des modules pour organiser votre code** :
    
        - Les modules peuvent vous aider à organiser votre code et à le rendre plus gérable.

---
---

<br>

**En ce qui concerne le DOM :**

11. **Minimisez la manipulation du DOM** :

    - La manipulation du DOM peut être coûteuse en termes de performances. Essayez de le faire le moins possible.

    ---

12. **Utilisez les sélecteurs CSS pour sélectionner les éléments** :

    - Les sélecteurs CSS sont un moyen puissant et flexible de sélectionner des éléments dans le DOM.

    ---

13. **Évitez le blocage du thread principal** :

    - Les opérations intensives de CPU ou de réseau peuvent bloquer le thread principal et rendre votre page moins réactive. Essayez d'éviter cela autant que possible.

    ---

14. **Utilisez des événements délégués** :

    - Au lieu d'ajouter des écouteurs d'événements à des éléments individuels, ajoutez-les à un élément parent et utilisez la propagation des événements.

    ---

15. **Utilisez requestAnimationFrame pour les animations** :

    - Cela vous permet d'avoir des animations fluides et efficaces.

    ---

16. **Évitez le reflow et la peinture autant que possible** :

    - Ces opérations peuvent être coûteuses en termes de performances.

    ---

17. **Utilisez les Web Workers pour les tâches intensives de CPU** :

    - Les Web Workers vous permettent d'exécuter du code dans un thread séparé, évitant ainsi de bloquer le thread principal.

    ---

18. **Préférez l'utilisation de bibliothèques ou de frameworks pour manipuler le DOM** :

    - Des bibliothèques comme jQuery ou des frameworks comme React ou Vue rendent la manipulation du DOM plus facile et plus sûre.

    ---

19. **Assurez-vous de nettoyer les écouteurs d'événements** :

    - Les écouteurs d'événements peuvent causer des fuites de mémoire s'ils ne sont pas correctement nettoyés.

    ---

20. **Utilisez l'API Fetch pour les requêtes réseau** :

    - Fetch est un moyen moderne et puissant de faire des requêtes réseau.

---

```

4. Connaissance et utilisation d’un framework de présentation de type adaptatif (5 points):


  Tailwind probablement pour moi le meilleur temp qu'il nous aide a faire le responsive..., et a accéléré parfait! ❤️

```

---

```

5. Déploiement de la réalisation en ligne (3 points):


- Netlify une bonne option

```


---

## Règle

<br>

A chaque développement de fonctionnalité sur une langage, creer une branche en la nommant comme la fonctionnalité a développer sur cette langage, et en anglais (En raison des accentuations françaises, nous prendrons l'anglais).

1. ère fonctionnalité random = dev/random-JS

2. e block de style dice throw animation = dev/dice-throw-animation-css

et puis en suite, commiter a la fin notre ticket jira DAJ-1 avec conventional commit, en faisant simplement git commit, et dans la nouvelle fenêtre ouvrant, pour exemple, tout dans la meme ligne:

- feat(DAJ-1): ✨ ajouter fonctionne de addition #comment Cette fonction vous permet d'ajouter deux nombres entiers et de renvoyer le résultat #done  Tache terminé #time 2h 5m #assign utilisateur@exemple.com #label urgente"

voir smart commit jira pour plus information sur les paramètres smart

<br>
<br>

---
---
---
---
---
---
---
---

<br>
<br>

Ce qui suit est la licence Creative Commons Attribution-NonCommercial-NoDerivs 3.0 Unported 
(CC BY-NC-ND 3.0), une licence largement utilisée pour fournir des espaces gratuits pour partager 
de l'art, des œuvres et des connaissances à des fins non commerciales : 

### Creative Commons Attribution-NonCommercial-NoDerivs 3.0 Unported (CC BY-NC-ND 3.0) 
Cette licence permet aux utilisateurs de : 

* Partage : copiez et redistribuez le matériel sur n'importe quel support ou format 
Dans les conditions suivantes : 

* Attribution : Vous devez donner un crédit approprié indiquant qui a fait le travail original. 

* Non commercial : Vous ne pouvez pas utiliser le matériel à des fins commerciales. 

* Aucun dérivé : Le matériel ne peut être modifié, transformé ou adapté. Pour les exceptions suivantes :

* Aucune restriction supplémentaire - Vous pouvez combiner le matériel avec le travail et/ou 
le modifier pour répondre aux exigences des projets. 

Cette licence s'applique exclusivement au travail de Dumitru Stefan Fernando, 
"X-Station The New Union".

Cela signifie que l'utilisateur ne peut pas utiliser l'œuvre à des fins commerciales, ni modifier,
transformer ou adapter l'œuvre.

Ce travail ne peut être partagé et redistribué qu'intact, sans imposer de restrictions supplémentaires.
