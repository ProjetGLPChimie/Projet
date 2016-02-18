# Projet

****Chimie****

liens utiles : http://www.elementschimiques.fr/?fr/elements/z/24



OBJECTIFS: Creér le tableau périodique


On peut procèder de deux manières:



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

Nous avons 18 colonnes, de 1 à 18.

J'ai reussi a trouver une algo qui nous permet de classer tous les elements de la 1ere ligne au 12 eme ligne.

A partir de la 12 éme cela ne marche plus , mais ce que je propose c'est de les mettre dans des "if".

Demo de l'algo :

Prenons par exemple l'atome Be.
Dans notre table de données les seuls informations qu'on peux utiliser c'est seulement le nombre de charges de l'atome en question.

Be a 4 charges.

On verifie a chaque 2^n que 4 est toujours compris entre 2^n et 2^n+1.

exemple Be

nombre charge =4;
 2^0<=4<2^1 :faux 
 donc on fait
 2^1<=4<2^2 : faux
 on continue encore 1 fois .
 2^2<=4<2^3 : vrai
 
 Nous avons d'ores et déjà notre y qui est y=2;
 
 maintenant pour avoir le x 
 
 on fait x=4-4=0;
         x=x-2;
         notre x seras -2 mais on retourn toujours la valeur positif
         if(x<o){
         return x=x*-1;
          }

Exemple Sc
nombre charge =21;
 2^0<=21<2^1 :faux 
 donc on fait
 2^1<=21<2^2 : faux 
 on continue encore .
 2^2<=21<2^3 : faux
  2^3<=21<2^4 : faux
 
 Nous avons notre y qui est y=3;
 
 maintenant pour avoir le x 
 
 on fait x=21-16=5;
         x=x-2;
         if(x<o){
         return x=x*-1;
          }
          else{
          return x;}
          
Donc notre x est 3;




Que doit faire notre programme?

1.Calculer la masse d'un atome.
Pour cela on auras besoin de connaitre :
1.1 A=le nombre de nucléons (On recupère cela depuis notre ArrayList) 
1.2 Masse_nucléons=la masse d'un nucléons

La formule a utiliser seras : A*Masse_nucleons


2.Calculer le nombre de protons,electrons,neutrons.

3Déduire de la masse molaire, volume molaire, les quantités de matières, et viceversa, d'un atome ou d'une molécule.
(ex. quantité d'élément oxygène dans 100g de saccharose)


