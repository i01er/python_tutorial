---
description: How can we get input from the user?
---

# Input

### String input

You can let user to input string value during the python program from console:

```python
# Create file input.py

name = raw_input ("What is your name ?") # name is a string
city = raw_input ("Where do you live ?") # city is a string

print "Welcome " + name + " from " + city
```

Save it and run by typing `python input.py` in console:

![](.gitbook/assets/image%20%2810%29.png)

{% hint style="info" %}
Python stops executing when it comes to the `input()` function, and continues when the user has given some input.
{% endhint %}

### Integer input

```python
#Create file num_input.py

age = input("How old are you ?") #age is an integer

print "You look like " + str(age) + " old" #str(age) is a string
```

#### Why str\(age\) ?

In this script, age is defined as an integer, however when we print out the result, mixing up string and integer will cause error. We need to change age from int to str by using `str(age)`. Otherwise we will get the error `cannot concatenate 'str' and 'int' objects`.

#### Versioning

In common,

{% hint style="info" %}
Python 3.6 uses the `input()` method.
{% endhint %}

{% hint style="info" %}
Python 2.7 uses the `raw_input()` method.
{% endhint %}



Reference: [https://docs.python.org/3/library/2to3.html?highlight=input\#to3-automated-python-2-to-3-code-translation](https://docs.python.org/3/library/2to3.html?highlight=input#to3-automated-python-2-to-3-code-translation)

[https://www.w3schools.com/python/python\_user\_input.asp](https://www.w3schools.com/python/python_user_input.asp)

