# Industrialisation logiciel

## TP 2

### Réponses aux questions du TP

#### Exercice 1: GitHub Actions

#### B.

**Quelles étapes sont réalisées par cette action ?**

Lorsque une requête _PULL_ ou _PUSH_ est effectuée, GitHub va créer un container Linux et installer les dépendances Python nécessaires et tester l'application avec PyTest.

**Une étape est définie au minimum par 2 paramètres, lesquels sont-ils et à quoi servent-ils ?**

Une dépendance et un nom d'étape.

**La première étape contient un paramètre ‘with’, a quoi sert-il ?**

À définir la version de Python à utiliser.

#### Exercice 2: Qualité de code

#### A.

**Sur l’onglet Summary d’une analyse de code, SonarCloud fournit 4 indicateurs. Quels sont-ils et quelles sont leurs utilités ?**

- Reliability: Bugs et erreurs dans le code
- Security: Parties de codes vulnairables qui peuvent être exploitées.          
- Maintainability: Parties de code difficile à maintenanir
- Security review: Code sensible qui nécessite d'être revu afin d'éliminer de potentiels problèmes de sécurité.

**À quoi sert l’indicateur Quality Gate ?**

C'est un indicateur booléen qui permet de définir si le code peut être mis en production ou non.

#### B.

**Quelle est la différence entre les sections New code et Overall Code dans l’onglet Summary ?**

_New Code_ est l'analyse des parties du codes qui ont été modifiées ou ajoutées. _Overall_ est l'analyse complète de tout le code.

**Y a-t-il des Code Smells ? Si oui, combien et pour quelle(s) raisons(s) ?**

Oui, il y en a 3. Deux _Code Smell_ sont pour le fait que le paramètre 'deferred' n'est pas utilisé, il conseil donc de l'effacer. Le dernier est dû au fait que sans l'utilisation du paramètre 'deferred', la fonction 'spend_money()' fait exactement la même action que 'spend_cash()', ce qui est redondant, il propose donc de modifier sont implémentation.

**Y a-t-il des Security Hotspots ? Si oui, combien et pour quelle(s) raison(s) ?**

Oui, il y en a 1. Il indique que l'image s'execute avec un utilisateur ayant les droits administrateur par défaut. Il dit d'être sûr que s'est sécurisé dans ce cas.