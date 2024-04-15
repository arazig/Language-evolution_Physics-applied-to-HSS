# Language-evolution_Physique-applique-aux-SHS
Projet de groupe - Développement modèle d'évolution du language à partir de l'article "Sharp transition towards shared vocabularies in multi-agent systems"

## Simulations pour l'article : https://arxiv.org/pdf/physics/0509075.pdf

Membres du groupe :

Tony Lauze
Amine Razig
Lilou Soulas

**Résumé du "naming game" :**

N personnes sont réunies autour d'un ensemble de M objets, et essaient de créer un langage commun pour désigner ces objets. Chaque personne dispose d'un inventaire, c'est à dire d'une liste d'associations mot-objet. Au début du jeu, tous les inventaires sont vides. A chaque étape, deux personnes sont prises au hasard, l'un parle (le speaker), l'autre écoute (le hearer) et procède à une interaction (voir règles de cette interaction dans l'article, ou dans le petit schéma en-dessous).


Le système sera représenté par un dictionnaire, où chaque clé (numérotée de 1 à N) est une personne, et où chaque valeur est l'inventaire de la personne.

Pour chaque inventaire, il faudrait donc à nouveau un dictionnaire, mais comme dans l'artcile ils n'utilisent, "sans perte de généralité', qu'un seul objet (c'est à dire M=1), on aura, au lieu d'un "dictionnaire de dictionnaires", un dictionnaire de listes :

Chaque entrée du dictionnnaire est une personne, et est associée à une liste : la liste des mots dont la personne dispose pour nommer l'objet.
