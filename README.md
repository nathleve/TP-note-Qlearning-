# TP-note-Qlearning-
Ce git contient le TP noté sur le Q learning pour l'Ensai Nathan Leveque, Arthur Roblin, Ranujan Kathir

Ce TP noté/projet sur un algorithme de Q learning consiste à créer un algorithme de Q learning qui optimise la vente et l'achat d'action boursières. 
Ce git contient des jeux de données récupérée sur des sites de suivit des actions sur plusieurs années. 
Il contient aussi des notebooks contenant à la fois les fonctions pour définir notre algorithme de Q-learning ainsi que des essais d'utilisation de l'algorithme. 
Il comprend aussi des versions obsolètes de nos algorithmes dans un notebook nommé obsolètes si cela peut être utile.
Le système prix en compte pour notre algorithme de deep learning est composé du pirx des actions à l'instant t, la quantité d'action possédée par l'utilisateurs ainsi que son budget hors action(l'argent qu'il n'a pas investit).
Les actions possible par l'utilisateur sont la vente et l'achat d'actions dans la limite de son budget disponible. 
La récompense du système après une action et l'argent récolté. 
Le système est discrétisé pour notre algorithme. Cela veut dire que la quantité d'action possédées ainsi que le prix des actions sont réduit à des valeurs allant de 1 à n_nuance. Par exemple avec un nombre de nuance de 5 ont peut avoir 0%,20%,...,100% des actions d'un cours et les action peuvent valoir 0%,20%,...,100% de leur valeur maximal.
Les fonctions pour tranformer les données de base en des données discrétisées utilisables sont définis dans le notebook. 
L'algorithme peut théoriquement prendre n'importe qu'elle nombre de nuance et suivre autant d'action que voulue mais le temps de calcul augmente exponentiellement avec ces deux paramètres et nous déconseillons de les mettres trop élevées.
Finalement notre algorithme est utilisé en transformant nos données par exemple en enlevant une tendance linéaire ou en utilisant les variations relatives des valeurs des actions à la place de leurs valeurs absolue.
