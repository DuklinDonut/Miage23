# Semaine 02

---
### Patricia
- En préparation de la présentation sur l'analyse d'Artefact et AVL, j'ai revu le cours sur la rétro-ingénierie, ce qui me permet d'avoir des points d'analyse sur lesquels me concentrer pour les deux projets. J'ai utilisé des points d'arrêt pour avancer dans le code. Ce cours sera particulièrement utile pour mon alternance, où je devrai migrer plusieurs applications vers la version la plus récente de Java. Naviguer dans de gros projets que je ne connais pas me fait moins appréhender. J'ai desormais les outils nécessaires pour aborder des projets logiciels complexes et prendre les bonnes décisions en matière de conception. La pratique des TP de C3P sera d'une grande utilité.

- Laisser le récepteur du message décider signifie que lorsqu'un message est envoyé à un objet, c'est cet objet lui-même qui détermine comment il répondra au message en fonction de sa propre classe et de ses méthodes. On a utilisé cela pour l'implémentation des méthodes booléennes, chaque sous-classe de Boolean implémentait ainsi ses propres méthodes. Cela a permis d'exploiter le polymorphisme.

- L'une des principales leçons de cette semaine est l'importance de remplacer les structures conditionnelles statiques par des messages envoyés aux objets en exploitant les hiérarchies de classes. Cela permet à chaque objet de prendre des décisions concernant son comportement en fonction de sa classe. En d'autres termes, l'envoi de messages est un choix dynamique, et les classes sont des représentations de ces choix potentiels. Ainsi, lorsque nous adressons un message à un objet, la classe de cet objet détermine la méthode appropriée à exécuter.

- J'ai davantage appris sur l'héritage. Chaque classe a une seule superclasse, et en pharo toutes les classes héritent de Object. L'héritage des variables est statique et se fait lors de la définition de la classe, tandis que l'héritage du comportement est dynamique et se fait au moment de l'exécution.
  
- Nous avons pratiqué les concepts de "self" et "super" à travers des exercices de lookup. Ces exercices m'ont permis de comprendre que "self" représente le récepteur du message et que le processus du lookup commence dans la classe du récepteur en remontant la hiérarchie des classes si nécessaire. En ce qui concerne "super," j'ai appris que "super" représente également le récepteur du message mais il modifie le processus de recherche en commençant par la classe au-dessus de celle contenant l'expression "super," ce qui donne une recherche statique.

- J'ai appris qu'il faut éviter la duplication car elle copie les bugs. Nous devons aussi éviter les nombres magiques dans le code et les longs messages en privilegiant de nombreux petits messages.

### Ezzahra

L'une des principales leçons de cette semaine a été de souligner l'importance de remplacer les structures conditionnelles statiques par l'envoi de messages aux objets, en exploitant les hiérarchies de classes. Cette approche permet à chaque objet de prendre des décisions concernant son comportement en fonction de sa propre classe. Ainsi, l'envoi de messages devient une démarche dynamique, tandis que les classes deviennent des représentations de ces choix potentiels. Lorsqu'un message est adressé à un objet, c'est la classe de cet objet qui détermine la méthode à exécuter.

Mon apprentissage a également porté sur le concept d'héritage. Chaque classe a une seule superclasse, et dans le contexte de Pharo, toutes les classes héritent de la classe Object. L'héritage des variables est statique, déterminé lors de la définition de la classe, tandis que l'héritage du comportement est dynamique et se réalise au moment de l'exécution.

Nous avons eu l'occasion de mettre en pratique les notions de "self" et "super" à travers des exercices de recherche. Cela m'a permis de comprendre que "self" représente le récepteur du message, et le processus de recherche commence dans la classe du récepteur, remontant la hiérarchie des classes si nécessaire. En ce qui concerne "super," j'ai appris que ce terme représente également le récepteur du message, mais il modifie le processus de recherche en débutant par la classe supérieure à celle contenant l'expression "super," créant ainsi une recherche statique.

J'ai ainsi retenu l'importance d'éviter la duplication, car elle entraîne la copie de défauts potentiels. De plus, il est recommandé d'éviter les "nombres magiques" dans le code, et de favoriser l'utilisation de nombreux petits messages plutôt que de longs messages.

De plus, au cours de mes travaux avec Pharo, j'ai identifié un bug au sein de la plateforme. Fort de cette découverte, j'ai ouvert une pull request pour signaler le problème. Grâce à cette démarche, l'équipe de développement a pu prendre connaissance de la situation et a rapidement entrepris les mesures nécessaires pour corriger ce bug. Cela a été une expérience enrichissante, démontrant l'impact positif que l'engagement dans la communauté open source peut avoir sur l'amélioration des logiciels.
