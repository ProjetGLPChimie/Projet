# Projet

****Chimie****

OBJECTIFS: Creér le tableau périodique

On peux procèder de deux manières:

1ère

Nous allons tout d'abord créez un fichier données(ou plusieurs fichiers données) dans lequel(s) on va entrer tous les données de chaque atome.
Puis on à l'aide d'un Buffered reader nous allons lire ces données.
Ensuite nous allons coder une classe Atome qui prendra en arguments les données de l'atome C-A-D(element_symbol, number_of_nucleons, atomique_mass,????,) )
Chaque atome sera stocker dans un ArrayList.

2éme:

Au lieu de de créez un fichier et taper tous les données dans celui-ci, on pourras considérer que notre tableau de periodique comme une sorte de carte.Donc on aura a traiter avec les coordonnées.

1.Nous savons que les colonnes sont le nombre de couches.
2.Nous savons aussi que les lignes sont le nombre d'électrons sur leur dernière couche.

Nous avons 7 colonnes , de 1 a 7 a chaque fois nous avaonçons d'une colonne(ou on decends si on prends dans l'axe des ordonnées en négatif c-a-d y=-1,y=-2 etc) le nombre de couches extérieur augemente de 2^n.

Nous avons 18 colonnes, de 1 à 18.De 1 a 

Que doit faire notre programme?

1.Calculer la masse d'un atome.
Pour cela on auras besoin de connaitre :
1.1 A=le nombre de nucléons (On recupère cela depuis notre ArrayList) 
1.2 Masse_nucléons=la masse d'un nucléons

La formule a utiliser seras : A*Masse_nucleons


2.Calculer le nombre de protons,electrons,neutrons.

3Déduire de la masse molaire, volume molaire, les quantités de matières, et viceversa, d'un atome ou d'une molécule.
(ex. quantité d'élément oxygène dans 100g de saccharose)


