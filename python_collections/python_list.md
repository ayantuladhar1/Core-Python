Lists are used to store multiple items in a single variable.  

```python
thislist = ["apple", "banana", "cherry"]  
```

List items are ordered, changeable, and allow duplicate values.  
List items are indexed, the first item has index [0], the second item has index [1] etc.  
  
When we say that lists are ordered, it means that the items have a defined order, and that order will not change.  
  
The list is changeable, meaning that we can change, add, and remove items in a list after it has been created.  
  
Lists allow duplicate values:  
```python
thislist = ["apple", "banana", "cherry", "apple", "cherry"]
print(thislist)
```

To determine how many items a list has, use the len() function:  
  
Print the number of items in the list:  
```python
thislist = ["apple", "banana", "cherry"]
print(len(thislist))
```

List Items - Data Types  
List items can be of any data type:  
String, int and boolean data types:  
```python
list1 = ["apple", "banana", "cherry"]
list2 = [1, 5, 7, 9, 3]
list3 = [True, False, False]
```

A list can contain different data types:  
A list with strings, integers and boolean values:  
```python
list1 = ["abc", 34, True, 40, "male"]
```

Using the list() constructor to make a List:  
```python
thislist = list(("apple", "banana", "cherry")) # note the double round-brackets
print(thislist)
```

Access Items  
List items are indexed and you can access them by referring to the index number:  
```python
thislist = ["apple", "banana", "cherry"]
print(thislist[1])
```

Negative Indexing  
Negative indexing means start from the end  
-1 refers to the last item, -2 refers to the second last item etc.  
Print the last item of the list:  
```python
thislist = ["apple", "banana", "cherry"]
print(thislist[-1])
```

Return the third, fourth, and fifth item:  
```python
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:5])
```

This example returns the items from the beginning to, but NOT including, "kiwi":  
```python
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[:4])
```


This example returns the items from "cherry" to the end:


thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:])




Change the second item:


thislist = ["apple", "banana", "cherry"]
thislist[1] = "blackcurrant"
print(thislist)




Append Items
To add an item to the end of the list, use the append() method:

thislist = ["apple", "banana", "cherry"]
thislist.append("orange")
print(thislist)



To insert a list item at a specified index, use the insert() method.
The insert() method inserts an item at the specified index:


thislist = ["apple", "banana", "cherry"]
thislist.insert(1, "orange")
print(thislist)





Remove Specified Item
The remove() method removes the specified item.


thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")
print(thislist)



If there are more than one item with the specified value, the remove() method removes the first occurance:

Remove the first occurance of "banana":


thislist = ["apple", "banana", "cherry", "banana", "kiwi"]
thislist.remove("banana")
print(thislist)




Remove Specified Index
The pop() method removes the specified index.

Remove the second item:

thislist = ["apple", "banana", "cherry"]
thislist.pop(1)
print(thislist)




If you do not specify the index, the pop() method removes the last item.


thislist = ["apple", "banana", "cherry"]
thislist.pop()
print(thislist)




The del keyword also removes the specified index:

Remove the first item:


thislist = ["apple", "banana", "cherry"]
del thislist[0]
print(thislist)




Delete the entire list:


thislist = ["apple", "banana", "cherry"]
del thislist




Clear the List
The clear() method empties the list.
The list still remains, but it has no content.

thislist = ["apple", "banana", "cherry"]
thislist.clear()
print(thislist)





You can loop through the list items by using a for loop:
Print all items in the list, one by one:


thislist = ["apple", "banana", "cherry"]
for x in thislist:
  print(x)




Print all items by referring to their index number:




thislist = ["apple", "banana", "cherry"]
for i in range(len(thislist)):
  print(thislist[i])




Print all items, using a while loop to go through all the index numbers


thislist = ["apple", "banana", "cherry"]
i = 0
while i < len(thislist):
  print(thislist[i])
  i = i + 1




List Comprehension
List comprehension offers a shorter syntax when you want to create a new list based on the values of an existing list.

Based on a list of fruits, you want a new list, containing only the fruits with the letter "a" in the name.
Without list comprehension you will have to write a for statement with a conditional test inside:


fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist = []


for x in fruits:
  if "a" in x:
    newlist.append(x)


print(newlist)







fruits = ["apple", "banana", "cherry", "kiwi", "mango"]


newlist = [x for x in fruits if "a" in x]


print(newlist)





Python - Sort Lists


Sort the list alphabetically:

thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort()
print(thislist)




Sort Descending
To sort descending, use the keyword argument reverse = True

thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort(reverse = True)
print(thislist)


