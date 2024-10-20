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











          








   


 






    
  





      

       

   
         

   


























