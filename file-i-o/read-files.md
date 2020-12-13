---
description: Open a File on the Server
---

# Read Files

Assume we have the following file, located in the same folder as Python:

demofile.txt

> Hello! Welcome to demofile.txt
>
> This file is for testing purposes.
>
> Good Luck!

To open the file, use the built-in `open()` function.

The `open()` function returns a file object, which has a `read()` method for reading the content of the file:

```python
myfile = open("demofile.txt", "r")
print(myfile.read())
```

If the file is located in a different location, you will have to specify the file path, like this:

```python
myfile = open("D:\\myfiles\welcome.txt", "r")
print(myfile.read())
```

#### Read Only Parts of the File

By default the `read()` method returns the whole text, but you can also specify how many characters you want to return:

```python
myfile = open("demofile.txt", "r")
print(myfile.read(5))
#Return the 5 first characters of the file
```

#### Read Lines

You can return one line by using the `readline()` method:

```python
myfile = open("demofile.txt", "r")
print(myfile.readline())
```

{% hint style="info" %}
By calling `readline()` two times, you can read the two first lines.
{% endhint %}

You can use a loop to read the whole file line by line:

```python
myfile = open("demofile.txt", "r")
for x in myfile:
  print(x)
```

#### Close File

It is a good practice to always close the file when you are done with it.

```python
myfile = open("demofile.txt", "r")
print(myfile.readline())
myfile.close()
```

{% hint style="info" %}
You should always close your files, in some cases, due to buffering, changes made to a file may not show until you close the file.
{% endhint %}



Reference: [https://www.w3schools.com/python/python\_file\_open.asp](https://www.w3schools.com/python/python_file_open.asp)

