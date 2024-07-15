# 📙 Python


<h1 style="background-color: yellow; padding: 10px; text-align: center; font-size: 24px; font-family: Arial, sans-serif;">
    Méthodes de Liste
</h1>


```python
# Exemple de liste
my_list = [1, 2, 3, 4, 5]

# append()
my_list.append(6)
print(my_list)  # Output: [1, 2, 3, 4, 5, 6]

# clear()
my_list.clear()
print(my_list)  # Output: []

# copy()
my_list = [1, 2, 3]
my_list_copy = my_list.copy()
print(my_list_copy)  # Output: [1, 2, 3]

# count()
count = my_list.count(2)
print(count)  # Output: 1

# extend()
my_list.extend([4, 5])
print(my_list)  # Output: [1, 2, 3, 4, 5]

# index()
index = my_list.index(3)
print(index)  # Output: 2

# insert()
my_list.insert(2, 'a')
print(my_list)  # Output: [1, 2, 'a', 3, 4, 5]

# pop()
item = my_list.pop(2)
print(item)  # Output: 'a'
print(my_list)  # Output: [1, 2, 3, 4, 5]

# remove()
my_list.remove(3)
print(my_list)  # Output: [1, 2, 4, 5]

# reverse()
my_list.reverse()
print(my_list)  # Output: [5, 4, 2, 1]

# sort()
my_list.sort()
print(my_list)  # Output: [1, 2, 4, 5]
```

<h1 style="background-color: yellow; padding: 10px; text-align: center; font-size: 24px; font-family: Arial, sans-serif;">
    Méthodes de Dictionnaire
</h1>

```python
my_dict = {'a': 1, 'b': 2, 'c': 3}

# clear()
my_dict.clear()
print(my_dict)  # Output: {}

# copy()
my_dict = {'a': 1, 'b': 2, 'c': 3}
my_dict_copy = my_dict.copy()
print(my_dict_copy)  # Output: {'a': 1, 'b': 2, 'c': 3}

# fromkeys()
keys = ('a', 'b', 'c')
value = 0
new_dict = dict.fromkeys(keys, value)
print(new_dict)  # Output: {'a': 0, 'b': 0, 'c': 0}

# get()
value = my_dict.get('b')
print(value)  # Output: 2

# items()
items = my_dict.items()
print(items)  # Output: dict_items([('a', 1), ('b', 2), ('c', 3)])

# keys()
keys = my_dict.keys()
print(keys)  # Output: dict_keys(['a', 'b', 'c'])

# pop()
value = my_dict.pop('b')
print(value)  # Output: 2
print(my_dict)  # Output: {'a': 1, 'c': 3}

# popitem()
item = my_dict.popitem()
print(item)  # Output: ('c', 3)
print(my_dict)  # Output: {'a': 1}

# setdefault()
value = my_dict.setdefault('d', 4)
print(value)  # Output: 4
print(my_dict)  # Output: {'a': 1, 'd': 4}

# update()
my_dict.update({'e': 5, 'f': 6})
print(my_dict)  # Output: {'a': 1, 'd': 4, 'e': 5, 'f': 6}

# values()
values = my_dict.values()
print(values)  # Output: dict_values([1, 4, 5, 6])
```

<h1 style="background-color: yellow; padding: 10px; text-align: center; font-size: 24px; font-family: Arial, sans-serif;">
    Function Lambda
</h1>


```python

# Exemple de fonction lambda simple
x = lambda a, b, c : a + b + c
print(x(5, 6, 2))  # Output: 13


# Exemple de fonction de haut niveau avec une fonction lambda
def myfunc(n):
  return lambda a : a * n

mydoubler = myfunc(2)
print(mydoubler(11))  # Output: 22




