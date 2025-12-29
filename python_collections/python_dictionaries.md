Dictionary items are ordered, changeable, and does not allow duplicates.
Dictionary items are presented in key:value pairs, and can be referred to by using the key name.
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}

print(thisdict["brand"])
```

Print the number of items in the dictionary:
```python
print(len(thisdict))
```

Using the dict() method to make a dictionary:
```python
thisdict = dict(name = "John", age = 36, country = "Norway")
print(thisdict)
```

Get the value of the "model" key:
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
x = thisdict["model"]
```

Get Keys
The keys() method will return a list of all the keys in the dictionary.
Add a new item to the original dictionary, and see that the keys list gets updated as well:
```python
car = {
"brand": "Ford",
"model": "Mustang",
"year": 1964
}

x = car.keys()
print(x) #before the change

car["color"] = "white"
print(x) #after the change
```

Get a list of the values:
```python
x = thisdict.values()
```

Make a change in the original dictionary, and see that the values list gets updated as well:
```python
car = {
"brand": "Ford",
"model": "Mustang",
"year": 1964
}

x = car.values()
print(x) #before the change

car["year"] = 2020
print(x) #after the change
```

Get a list of the key:value pairs
```python
x = thisdict.items()
```

Check if "model" is present in the dictionary:
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
if "model" in thisdict:
  print("Yes, 'model' is one of the keys in the thisdict dictionary")
```

The pop() method removes the item with the specified key name:
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.pop("model")
print(thisdict)
```

The del keyword can also delete the dictionary completely:
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
del thisdict
print(thisdict)
```

The clear() method empties the dictionary:
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.clear()
print(thisdict)
```

Print all key names in the dictionary, one by one:
```python
for x in thisdict:
  print(x)
```

Print all values in the dictionary, one by one:
```python
for x in thisdict:
  print(thisdict[x])
```

Example:
You can also use the values() method to return values of a dictionary:
```python
for x in thisdict.values():
  print(x)
```

You can use the keys() method to return the keys of a dictionary:
```python
for x in thisdict.keys():
  print(x)
```

Loop through both keys and values, by using the items() method:
```python
for x, y in thisdict.items():
  print(x, y)
```

Make a copy of a dictionary with the copy() method:
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
mydict = thisdict.copy()
print(mydict)
```

Make a copy of a dictionary with the dict() function:
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
mydict = dict(thisdict)
print(mydict)
```
