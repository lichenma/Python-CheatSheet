# Python Cheat Sheet 

Collection of functions and Python commands gathered from various online sources. 



### What is Python? 

Python is a "batteries included" programming language that in contrast to other languages like Java, allows users to more readily focus and solve domain problems instead of dealing with the complexity of how a computer operates. Python achieves this with the following attributes: 

* Python is a `high-level` language meaning that it abstracts underlying computer-related technical details. Python does not force users to think about computer memory management or proper declaration of variables and uses safe assumptions about what the programmer is trying to convey. 
* Python is a `general-purpose` language meaning that it can be used for all problems that a computer is capable of rather than specializing in a specific area such as statistical analysis. 
* Python is an `interpreted` language meaning that evaluation of code to obtain results can happen immediately rather than having to go through the time-consuming compile and run cycle. 
* Python has a standard library and numerous third-pary libraries yielding a vast array of existing codebases and examples for solving problems 
* Python has an active community and many user which means that finding solutions is really simple online


These features come at the minor cost of reduced language performation but this is a tradeoff that the vast majority of users are willing to make in order to gain the advantages that Python has to offer. 



### Dictionary 

Dictionaries are the go to data structure for Python which is a **collection which is unorder, changeable and indexed**. In python dictionaries are written with curly brackets and they have keys and values. 


Creating a dictionary
```python
thisdict = {
    "brand": "Ford", 
    "model": "Mustang", 
    "year": 1964
}

print(thisdict)
```


We can **access items** in the dictionary by referring to the `key name` or using the `get()`: 

```python
x = thisdict["model"]
x = thisdict.get("model")
```



We can also **change the value** of a specific item by referring to its key name: 

```python 
thisdict["year"] = 2018
```



We can loop through a dictionary using a `for` loop. 

```python
# printing key names in the dictionary 
for x in thisdict: 
    print(x)

# printing all values in the dictionary 
for x in thisdict: 
    print(thisdict[x])

# printing all values in the dictionary 
for x in thisdict.values():
    print(x)

# looping through keys and values using items 
for x, y in thisdict.items():
    print(x,y)
```


We can also determine if a **specified key is present** in a dictionary using the `in` keyword: 

```python
if "model" in thisdict: 
    print("model is one of the keys in the dictionary")
```


To determine **how many items** (key-value pairs) a dictionary has, use the `len()` method


```python 
print(len(thisdict))
```



**Adding an item** to the dictionary is done by using a new index key and assigning a value to it: 

```python
thisdict["color"] = "red"
```


**Removing an item** from the dictionary has several methods: 

```python 
# remove a specific key-value pair 
thisdict.pop("model")

# remove the last inserted item 
thisdict.popitem()

# another way to delete a specific key-value pair 
del thisdict["model"]

# delete the entire dictionary 
del thisdict 

# empty the dictionary 
thisdict.clear()
```


**Copying ad dictionary** is not as simple as just typing `dict2 = dict1` since `dict2` is only a reference to `dict1` so any chances made in dict1 will automatically be reflected in dict2. 

Ways to make a copy include using the built-in Dictionary method `copy()` and the `dict()` method. 



```python 
mydict = thisdict.copy()
mydict = dict(thisdict)
```


A dictionary can also contain many dictionaries and this is referred to as nested dictionaries. 


It is also possible to use the `dict()` **constructor** to make a new dictionary: 

```python 
thisdict = dict(brand="Ford", model="Mustang", year=1964)
```








