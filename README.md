# Python Cheat Sheet 

Collection of functions and Python commands gathered from various online sources. 


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





