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

**Sur l’onglet Summary d’une analyse de code, SonarCloud fournit 4 indicateurs. Quels sont-ils et quelles sont leurs utilités ?**

- Reliability: Bugs et erreurs dans le code
- Security: Parties de codes vulnairables qui peuvent être exploitées.          
- Maintainability: Parties de code difficile à maintenanir
- Security review: Code sensible qui nécessite d'être revu afin d'éliminer de potentiels problèmes de sécurité.

**À quoi sert l’indicateur Quality Gate ?**

C'est un indicateur booléen qui permet de définir si le code peut être mis en production ou non.