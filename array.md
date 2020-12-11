---
description: Lists are used to store multiple items in a single variable.
---

# List

Lists are used to store multiple items in a single variable.

Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.

Lists are created using square brackets:

```python
a = [1,2,3,4,5]
b = ["apple", "banana", "orange", "cherry"]

print(a)
print(b)
```

{% hint style="info" %}
List items can be of any data type.
{% endhint %}

### List Items

List items are ordered, changeable, and allow duplicate values.

#### List Index

List items are indexed, the first item has index `[0]`, the second item has index `[1]` etc.

```python
#    0 1 2 3 4 5th position
a = [1,2,3,4,5,6]

print (a[0])
>>> 1

print (a[3])
>>> 4
```

When we say that lists are ordered, it means that the items have a defined order, and that order will not change.

#### List Append

If you add new items to a list, the new items will be placed at the end of the list. You can use `append` to add new item to the list.

```python
a = [1,2,3,4,5]
a.append(6)

print(a)
>>> [1,2,3,4,5,6]
```

{% hint style="info" %}
**Note:** There are some list methods that will change the order, but in general: the order of the items will not change.
{% endhint %}

The list is changeable, meaning that we can change, add, and remove items in a list after it has been created.

#### List Insert

You can also insert the item in specific position in the list:

```python
a = [1,2,3,4,5,6]
a.insert(2,37)    #Insert number 37 in 2nd position

print(a)
>>> [1,2,37,3,4,5,6]
```

#### List Same Value

Since lists are indexed, lists can have items with the same value:

```python
a = ["apple", "cherry", "orange", "cherry", "apple"]

print(a)
>>> ['apple', 'cherry', 'orange', 'cherry', 'apple']

print(a[1])
>>> cherry
```



