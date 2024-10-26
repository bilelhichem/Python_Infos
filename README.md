# 📙 Python


<h1 style="background-color: yellow; padding: 10px; text-align: center; font-size: 24px; font-family: Arial, sans-serif;">
   Introduction to Python
</h1>


```python
# Exemple de Varaiable


A variable name can contain letters (a-z, A-Z), numbers, and underscores (_), but it cannot start with a number.
_data = 9 (true)
0_name = 9 (false)

# Data Types 


   integer  8  ,  9 , -1 ....
   float   9.5 , 8.5 , .....
   String   'ALgeria'
 x= 9 - >  print(type(x)) => integer

# Type Casting

int(), float(), str(), bool().

  Example of Type Casting in Python:
        _data = 9 
        print(type(_data))   ==> <class 'int'>
        __data = bool(_data) ==> <class 'bool'>
        print(type(__data))

# Basic Arithmetic Operators in Python: 

    Addition (+): Adds two values.
    Subtraction (-): Subtracts the second value from the first.
    Multiplication (*): Multiplies two values.
    Division (/): Divides the first value by the second, resulting in a float.
    Floor Division (//): Divides and returns the largest integer less than or equal to the result.
    Modulus (%): Returns the remainder when dividing the first value by the second.
    Exponentiation (**): Raises the first value to the power of the second.
    And operator : x and y
    Or operator  : x or y
    Not operator : a = true => not a => a = false


# Lists and Tuples :

  _data = ['algeria', 9 , true]

  List Methods : 


    -->   append() : add element in the end of the list
    -->   insert() : insert an element at a specific index   ==> _data.insert(position, element)
    -->   remove() : Removes the first occurrence of an element
    -->   pop() : Removes and returns an element at a specific index ==> example _data.pop(2)
    -->   sort(): Sorts the list in ascending order
    -->   len() : returns  lenght ==> len(_data)
    --> reversed(list_var)
    --> sorted(list_var)
    --> enumerate(list_var) : list_var = ["apple", 12, 42, "banana"]
                                for index, value in enumerate(list_var):
                                      print(index,value)
   --> zip(list 1 , list 2 ) : permet de combiner deux list 


# Sets :
       Les éléments d'un set sont non ordonnés
       Un set ne peut pas contenir d'éléments dupliqués

       _data = {1,2}

    le meme fonction que les listes

   --> update : _data.update({1,5}) ==> pour ajouter plusieurs éléments à un set

# Dictionary :

    car = { "key " : "element"}

       car.get(key)

# Python Modules

     import the math module : import math

     import the Random and choice Function :  from random import randint , choice ;

            exemple : b = ["ESI","EVRY","Lile"]    ==> prine(choice(b)) ==> Lile
                      randint(1,10) ==> 3


# Filter Function :  filter (function , iterable )
    exemple :   def myFunc(x):
                  if x < 18:
                      return False
                         else:
                      return True

      adults = filter(myFunc, ages)

# Map Function in python : map(function, iterable)


# Lambda Function : Une fonction lambda en Python est une petite fonction anonyme (sans nom) qui est définie en une seule ligne.
                    Les fonctions lambda sont souvent utilisées lorsqu'on a besoin d'une fonction simple et temporaire

    la creation : lambda arguments : expression

    exemple : square = lambda x: x ** 2
              print(square(5))  # Sortie : 25 

# String in Python

   text = "hello word"
         * Convert the string to uppercase
            print(text.upper())
         * Convert the string to Lowercase
            print(text. lower ())
         * Replace a substring
            print(text.replace("Hello", "Hi"))
         * Lets take a string with extra spaces
            my_string = " Hello, World!
            print(my_string. strip())  //   Lets use the strip function to remove the extra spaces
         * Lets explore the startswith and endswith functions
            my_string = "Hello, World!"|
            print(my_string. startswith("Hello")) //  Lets check the output for the startswith function
            print(my_string. endswith("World!")) //    Lets check the output for the endswith function
         * Lets explore the count function
            my _string = "Hello, World!"
            print (my_string. count ("o")) //  Lets check the occurence of "o"


# For Loop

        ex :
            a=['Delhi', 'Mumbai', 'Kolkata', 'Bangalore', 'Chennai']
               for city in a:
                     print(city)

# While Loop

      while i<=5：
             print(i)

# Ternary operation :

    condition = True
    res = "la condition est vraie" if condition else "la condition est fausse"

# Exception :
    arg = input()

          arg = input()
          try:
             char = arg[12]
          except IndexError: # Capture une exception d'indice
             print("Une exception d'indice a été levée")
          except: # Capture toute exception n'ayant pas déjà été testée
             print("Une exception a été levée")
          else: # Si aucune exception n'est levée, ce bloc est exécuté
              print("Aucune exception d'indice n'a été levée")
          finally: # Exécute ce code quoi qu'il arrive
               pass

# Introduction to OOPs Concept :
  class Person:
    def __init__(self, name, age):
        # Initialize the 'name' attribute of the Person object
        self.name = name
        # Initialize the 'age' attribute of the Person object
        self.age = age

# Créer une instance de la classe Person
p1 = Person("Nikhil", 36)

// __init__ C'est le constructeur qui s'exécute lors de la création d'une instance de Person


# Inheritance :

   Syntax:
     class BaseClass:
         # Attributes and methods of the base class
     class DerivedClass (BaseClass):
         # Additional attributes and methods specific to derived class


    exemple  ;
class Animal : 
     def __init__(self,name,age):
          self.name = name ;
          self.age = age  
     def display (self) :
      print(self.name , self.age);

class Dog (Animal):
     def __init__(self, name, age):
          super().__init__(name, age)  

p1 = Dog("Ol" , 12);

p1.display();



# Encapsulation :

     Attribute Protection Levels 

       def __init__(self, name, age):
        self.name = name  # attribut public
      def __init__(self, name, age):
        self._name = name  # attribut protégé cet attribut est protégé et qu'il ne devrait pas être modifié directement en dehors de la classe ou de ses sous-classes (c'est une           convention, pas une règle stricte).
     def __init__(self, name, age):
        self.__name = name  # attribut privé



# Classe abstraite :
   from abc import ABCMETA , abstractmethod ; // pour définir des classes abstraites

   
   
   class Programming(metaclass=ABCMeta) :
          @abstractmethod  
          def has_oop (self) :  // Dans les classes abstraites, les méthodes n'ont pas de valeur de retour.
               pass

   class Pascal(Programming):  
       def has_oop(self):
          return "No"

 // Dans les classes héritées à partir d'une classe abstraite, il est obligatoire d'implémenter les mêmes méthodes définies dans la classe abstraite. Par ailleurs, on ne peut pas créer d'instance directement à partir d'une classe abstraite, mais on peut en créer à partir des classes qui en héritent.

# Interface in Python : 
   from abc import ABCMeta, abstractmethod

class FormalParserInterface(metaclass=ABCMeta):
    
    @abstractmethod
    def load_data(self, file_path):
        raise NotImplementedError

    @abstractmethod
    def extract_text(self, file_path):
        raise NotImplementedError

class MyParser(FormalParserInterface):

    def load_data(self, file_path):
        pass

    def extract_text(self, file_path):
        pass

# Création d'une instance de MyParser
MyParser()



# méthode magique  :

   --> Une méthode magique en Python est une méthode spéciale qui commence et se termine par deux underscores (__)

   --> Ces méthodes sont appelées magiques parce que Python les exécute automatiquement dans certaines situations, sans que tu aies à les appeler directement

   --> exemple :

    def __init__(self) est une méthode magique très courante est appelée automatiquement quand tu crées un nouvel objet de la classe
    p = Person("Alice")

  --> isinstance() est une fonction intégrée en Python qui vérifie si un objet appartient à une classe spécifique ou à une sous-classe. Elle renvoie True si l'objet est une instance de cette classe, sinon elle renvoie False.
   exemple :

   if isinstance(other, MyFloat) : Dans ce cas, isinstance(other, MyFloat) vérifie si l'objet other (l'objet avec lequel tu compares self) est une instance de la classe MyFloat.




# Getters et Setters en Python :

   Les getters et setters sont des méthodes utilisées pour accéder et modifier les attributs d'une classe

   class Person:
      def __init__(self, nom: str) -> None:
          self.__nom: str = nom

      def get_name(self) -> str:
          return self.__nom

     def set_name(self, name: str) -> None:
         self.__nom: str = name
  
 

# Module MyPy :

  MyPy est un outil qui aide à vérifier si tu utilises correctement les types dans ton code Python. 

  Comment installer MyPy  : python3 -m pip install -U mypy



# Introduction aux tests en programmation :

     1. Tests unitaires avec unittest : 
     unittest est un framework de test intégré dans Python. Il permet de tester de petites unités du code (comme des fonctions ou des méthodes). Le principe est simple : tu écris      des tests pour vérifier que chaque fonction se comporte correctement dans différentes situations.

      import unittest
      * Fonction simple à tester
          def addition(a, b):
                return a + b
  
      * Classe de tests
          class TestAddition(unittest.TestCase):
                   def test_addition(self):
                         self.assertEqual(addition(1, 2), 3)  # Vérifie si 1 + 2 = 3
                           self.assertEqual(addition(0, 0), 0)  # Vérifie si 0 + 0 = 0
                             self.assertEqual(addition(-1, 1), 0) # Vérifie si -1 + 1 = 0

     * Exécuter les tests
          if __name__ == "__main__":
               unittest.main()

    2. Tests avec pytest
    pytest est un autre framework de test Python qui est plus flexible et convivial que unittest. Il est souvent préféré pour des projets plus complexes grâce à ses
    fonctionnalités avancées.

         def addition(a, b):
             return a + b

       * Tests avec pytest
            def test_addition():
                assert addition(1, 2) == 3
                assert addition(0, 0) == 0
                assert addition(-1, 1) == 0




   3. Les mocks et patchs
   
      Mocks : Simulent des objets réels pendant un test, permettant de tester ton code sans exécuter les véritables objets ou appels externes.
      Patches : Remplacent temporairement des fonctions ou méthodes pour éviter d'exécuter du code réel ou complexe pendant les tests.
      

  

   




```
# 📈 Python for Data Science 

<h1 style="background-color: yellow; padding: 10px; text-align: center; font-size: 24px; font-family: Arial, sans-serif;">
   Introduction to Python for Data Science
</h1>
   
    
```python

 # Introduction à Pandas :

   Pandas est une bibliothèque Python utilisée principalement pour la manipulation et l'analyse des données. Elle permet de travailler efficacement avec des structures de données    appelées DataFrames et Series. Ces structures sont similaires aux tableaux et matrices

   installer pandas dans Python : pip install Pandas
   import : import pandas as pd ;

   * df =  pd.read_cvs("");  // pour lire les fichier cvs
   * df.head() affichier seulment 5 premier ligne de cvs  mais  df.head(n)  Ce code va afficher les n premières lignes du DataFrame
   * df.columns affichier les columns de cvs
   * df.select_dtypes("type") // On peut préciser quel type de données on peut choisir.
   * salary_variance = df['MonthlyIncome'].var() // var() : Cette fonction calcule la variance d'une série de données
   * salary_std_dev = df['MonthlyIncome'].std() // std() : Cette fonction calcule l'écart-type


 #  Données catégorielles  :

   Les données catégorielles représentent des valeurs discrètes qui appartiennent à des catégories spécifiques. Elles ne sont pas numériques

   Il existe deux sous-types :

   1) Données nominales : Elles représentent des catégories qui n'ont pas d'ordre ou de classement particulier. ● Exemples : Le genre, la couleur, la profession, l'état civil,

   2)Données ordinales : Ces données représentent des catégories qui ont un ordre ou un classement spécifique. ● Exemples : Le niveau d'éducation, la satisfaction des clients,

   Pour analyser ces données, on peut : ● Calculer des fréquences et des proportions, et créer des visualisations de données comme : ○ Des graphiques en barres, ○ Des diagrammes     circulaires (camemberts), ○ Des histogrammes.

   On utilise des bibliothèques Python telles que pandas, matplotlib et seaborn pour manipuler et visualiser ces données.
 



 # Mesures de tendance centrale :

   Les mesures de tendance centrale permettent de décrire et résumer les données
   Les trois principales mesures sont : la moyenne, la médiane, et le mode.

   1. Moyenne (Mean) :
          Moyenne= Somme de toutes les valeurs / Nombre total de valeurs
   2. Médiane (Median) : La médiane est la valeur du milieu lorsque les données sont triées dans un ordre croissant ou décroissant
          Étapes pour calculer la médiane :
              --> Trier les données en ordre croissant.
              --> Si le nombre de valeurs est impair, la médiane est la valeur du milieu.
              --> Si le nombre de valeurs est pair, la médiane est la moyenne des deux valeurs centrales.

   3. Mode (Mode) :
         c'est la valeur qui se répète le plus souvent


   Mesures de tendance centrale en python :

          moyenne = df["SALARY"].mean();
          mediane = df["SALARY"].median();
          mode = df["SALARY"].mode();



 # Les mesures de forme et de position: 

   Les mesures de forme et de position sont des outils statistiques qui aident à décrire la distribution des données et à comprendre leur répartition. Voici une explication          simple avec des exemples pour chaque point

      * Asymétrie (Skewness) :
            Cela vous dit si les données sont plus étirées d'un côté que de l'autre. Si c'est étiré vers la gauche, c'est asymétrique à gauche. Si c'est étiré vers la droite,                 c'est asymétrique à droite. Si c'est équilibré, c'est symétrique.
      * Aplatissement (Kurtosis) :
            Cela vous montre si les données ont plus ou moins d'extrêmes (valeurs très grandes ou très petites). Un aplatissement élevé signifie plus d'extrêmes, un aplatissement             faible signifie moins d'extrêmes.
      * Percentiles et quartiles sont des outils de position qui vous aident à voir où se situe une donnée par rapport au reste du groupe.


  # La bibliothèque scipy.stats :

      scipy.stats propose des fonctions qui aident à :

      Calculer des statistiques comme la moyenne, la médiane, l'écart-type, etc.
      Travailler avec des distributions de probabilité (normales, binomiales, Poisson, etc.).
      Tester des hypothèses (par exemple, le test T, le test de chi-carré).
      Générer des données aléatoires suivant différentes distributions.
      Calculer des mesures de corrélation ou d'association entre variables (par exemple, la corrélation de Pearson, Spearman).

      instalation : pip install scipy      
      import : import scipy.stats as stats ;

      *) SciPy Stats module is used to calculate the skewness and kurtosis of a variable called monthly
         --> Calculate skewness and kurtosis
             salary_skewness = stats.skew(df[ 'MonthlyIncome']) // stats.skew() v>0 postive , 0<v negative , v = 0 eqiu
             salary_kurtosis = stats.kurtosis(df[ 'MonthlyIncome']) // stats.kurtosis()


 # NumPy (Numerical Python) :
   est une bibliothèque open source qui permet de travailler efficacement avec des tableaux et des matrices de grandes dimensions

   instalation : pip install numpy
   import : import numpy as np ;

   // Random Numpy

   np.random.seed(10)  # Fixe la graine
   random_numbers = np.random.rand(5)  # Génère 5 nombres aléatoires entre 0 et 1
   print(random_numbers)  # Affiche les nombres aléatoires générés



 # Matplotlib :
   Matplotlib est une bibliothèque très flexible et puissante pour la visualisation de données. Que vous souhaitiez simplement tracer des courbes ou créer des visualisations plus    complexes

   instalation : pip install Matplotlib
   import : import matplotlib.pyplot as plt ;

    import matplotlib.pyplot as plt

      x = [0, 1, 2, 3, 4]
      y = [0, 1, 4, 9, 16]

      plt.plot(x, y) ou plt.scatter(x,y)
      plt.xlabel('x')
      plt.ylabel('y')
      plt.title('Graphique en courbes simple')
      plt.show()


 # Scikit-learn :

     k-mean clustering :  algorithme qui regroupe des données similaires en clusters
     import :   from sklearn.cluster import KMeans

 # sklearn  :
   scikit-learn (ou sklearn) est une bibliothèque très puissante et populaire en Python pour le machine learning et l’analyse des données. Elle propose une large gamme d'outils      pour des tâches de modélisation, de prétraitement, et d'évaluation.

   * La modélisation consiste à créer un modèle mathématique ou statistique qui représente une relation ou un phénomène observé dans les données
   * Le prétraitement est l'étape qui consiste à préparer les données avant leur utilisation dans un modèle. Cela peut inclure des tâches comme :
         Nettoyage des données : supprimer ou corriger les données manquantes, erronées ou dupliquées.
         Transformation des données : normaliser ou standardiser les valeurs pour les rendre comparables.
         Sélection de caractéristiques : choisir les variables les plus pertinentes pour le modèle afin d'améliorer sa performance.

   * L’évaluation nous permet de savoir si le modèle est efficace et fiable pour faire des prédictions.


  # Kmean :

    KMeans est un algorithme de clustering non supervisé qui regroupe les données en un certain nombre de clusters

      Initialisation : L'algorithme choisit un certain nombre de centroids (points centraux) de manière aléatoire. Chaque centroid représente le centre d'un cluster.
      Attribution des points aux clusters : Chaque point de données est attribué au cluster dont le centroid est le plus proche, basé sur une mesure de distance (généralement la                                              distance euclidienne).
      Mise à jour des centroids : Une fois que tous les points ont été attribués, les centroids sont recalculés en prenant la moyenne des points dans chaque cluster.
      Répétition : Les étapes 2 et 3 sont répétées jusqu'à ce que les centroids ne changent plus de manière significative, ce qui signifie que les clusters se sont stabilisés

      from sklearn.cluster import KMeans;

      km = KMeans(n_clusters=3); // vous voulez diviser vos données en 3 clusters
      y_predicted = km.fit_predict(df[[ 'age', 'trestbps']]);   // entraîne l'algorithme KMeans sur les données fournies  et Cela signifie que l'algorithme va trouver les
                    clusters basés sur les données d'entrée et Après l'entraînement, la méthode predict retourne les labels des clusters pour chaque point de données


```
   <img src="https://github.com/user-attachments/assets/90bfd157-cd7c-4ff8-8c3c-7c7cb5d5829a" alt="KMeans Clustering Example" width="100%" height="400" >

  <img src="https://github.com/user-attachments/assets/5d4dc8af-1c6c-4ff3-97a1-d7f235efd3fa" alt="KMeans Clustering Example" width="100%" height="400" >


```python


   Si l'on examine plusieurs cas dans le graphique, on peut constater qu'il y a des erreurs dans la répartition des données dans les clusters, car nous n'avons pas effectué de       prétraitement.

   # Example :



```
  <img src="https://github.com/user-attachments/assets/ea551839-76fb-4ef1-8e98-f0a33dff4bc1" alt="KMeans Clustering Example" width="100%" height="400" >
```python 


  
    
  


  
     


  






​	
       








   


 






    
  





      

       

   
         

   


























