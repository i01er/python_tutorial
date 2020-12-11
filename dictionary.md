---
description: How to use dictionary in Python
---

# Dictionary

Dictionaries are used to store data values in key:value pairs.

A dictionary is a collection which is unordered, changeable and does not allow duplicates.

Dictionaries are written with curly brackets, and have keys and values:

```python
dt = {
    "brand": "Honda",
    "model": "Fit",
    "year": 2005
}

print(dt)
>>> { 'brand': 'Honda', 'model': 'Fit', 'year': 2005 }
```

#### Dictionary Items

Dictionary items are unordered, changeable, and does not allow duplicates.

Dictionary items are presented in key:value pairs, and can be referred to by using the key name.

```python
dt = {
    "brand": "Honda",
    "model": "Fit",
    "year": 2005
}

print(dt["brand"])
>>> Honda
```

#### Unordered

When we say that dictionaries are unordered, it means that the items does not have a defined order, you cannot refer to an item by using an index.

#### Changeable

Dictionaries are changeable, meaning that we can change, add or remove items after the dictionary has been created.

#### Duplicates Not Allowed

Dictionaries cannot have two items with the same key:

{% hint style="info" %}
Duplicate values will overwrite existing values.
{% endhint %}

```python
dt = {
    "brand": "Honda",
    "model": "Fit",
    "year": 2005,
    "year": 2013
}

print(dt)
>>> { 'brand': 'Honda', 'model': 'Fit', 'year': 2013 }
```

#### Dictionary Length

To determine how many items a dictionary has, use the `len()` function:

```python
dt = {
    "brand": "Honda",
    "model": "Fit",
    "year": 2005
}

print(len(dt))
>>> 3
```

#### Dictionary Items - Data Types

The values in dictionary items can be of any data type:

{% hint style="info" %}
String, int, boolean, function and list data types, even a dictionary inside dictionary.
{% endhint %}

```python
dt = {
    "brand": "Honda",
    "model": "Fit",
    "year": 2005,
    "electric": False,
    "colors": ["blue", "white", "red", "black"],
    "version": {"GE": "1500cc", "GK": "1300cc"}
}

print(dt['version']['GE'])
>>> 1500cc
```



Reference: [https://www.w3schools.com/python/python\_dictionaries.asp](https://www.w3schools.com/python/python_dictionaries.asp)

