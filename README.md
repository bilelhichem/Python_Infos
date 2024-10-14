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

      

       

   
         

   


























