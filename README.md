2025-2026 C21838 ElKheit Mohamed Babaha MLDS

Rapport De Projet

Ce mini=projet consiste  à  appliquer deux methodes de regression, notmment la regression lineaire et la regression logistique  à  deux datasets qui sont beginner friendly.

Dans le cadre de la regression lineaire, nous avons fait appel  à  des bibliotheque Python afin d'explorer et traiter les donnees du dataset Medical Insurance Cost.
Le dataset etant dejà   quasi-totalement organise, nous avons passe rapidement, apres verification du manque de champs null, à  la conversion des features/"classe" en valeurs numeriques.

La variable ciblee etant le cout ("charges") de l'assurence, nous avons visualise son evolution selon les autres 'features'.
Nous avons remarque que le tabagisme (fait d'etre fumeur) est proportionnellement corollaire au cout de l'assurance. 
Il est d'ailleurs le parametre qui influt le cout d'assurance medicale le plus, suivi du BMI (IMC) et des autres parametres comme la region, du sexe, de l'age et du nombre de dependants.
Comme il est aussi indique par la Matrice de chaleur.

Ensuite, on a fait appel a la bibliotheque Scikit-learn afin d'entrainer et d'evaluer notre model. Le modele a suivit la regle 80% du dataset pour l'entrainement et 20% pour le test.
A la fin de cette apprentissage, notre modele a un coefficient de dtermination R2 de 0.7998747145449959; et une erreur quadratique moyenne de 31845929.13415943.
Cela indique que ce modele est tres bien en ce qui concerne l'explication de la variance de la variable cible, mais que ces predictions ne sont pas precises.

Partie II: Regression Logistique
Dans ce cadre, nous avions fait appel a Iris, un dataset natif dans Scikit-learn. Ce dataset cathegorise les iris en trois types: Setosa, Versicolour, et Virginica. 
Dans ce projet, nous considerions celles de type Setosa comme etant la classe 0 et les deux autre type comme etant la classe 1. 
Ainsi on a un probleme de classification binaire (l'Iris est soit de classe 0, soit elle est de clasee1). 

On importe ainsi les bibliotheque Python qui nous permettent de traiter les donnees de ce dataset afin de prevoir si un Iris est de classe 0 ou pas.
On remarque que la distribution des classes est equilibree (33,3% pour chaqune des trois types d'iris).
On normalise les variables d'entree.
Puis on Modelise la probabilite d'appartenance a l'aide de la fonction sigmoid.
En evaluant le modele par la Matrice de confusion, on remarque l'abscence de Faux Positifs et de Faux Negatives.
De plus, l'Accuracy,Précision et le Rappel sont egales ou tres proches de 1 et aussi la training accuracy.
Cela pourrait etre du a la simplicite du dataset Iris et a sa petite taille.



