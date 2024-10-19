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

<img width="378" alt="Screenshot 2024-10-19 at 10 19 59 PM" src="https://github.com/user-attachments/assets/c1fb527b-c053-4758-9074-8b2e68cd8df0">






   


 






    
  





      

       

   
         

   


























