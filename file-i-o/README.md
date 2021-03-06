---
description: I/O means input output.
---

# File I/O

File handling is an important part of any web application.

Python has several functions for creating, reading, updating, and deleting files.

#### File Handling

The key function for working with files in Python is the `open()` function.

The `open()` function takes two parameters; _filename_, and _mode_.

There are four different methods \(modes\) for opening a file:

`"r"` - Read - Default value. Opens a file for reading, error if the file does not exist

`"a"` - Append - Opens a file for appending, creates the file if it does not exist

`"w"` - Write - Opens a file for writing, creates the file if it does not exist

`"x"` - Create - Creates the specified file, returns an error if the file exists

In addition you can specify if the file should be handled as binary or text mode

`"t"` - Text - Default value. Text mode

`"b"` - Binary - Binary mode \(e.g. images\)

#### Syntax

To open a file for reading it is enough to specify the name of the file:

```python
myfile = open("demofile.txt")
```

The code above is the same as:

```python
myfile = open("demofile.txt", "rt")
```

{% hint style="info" %}
Because `"r"` for read, and `"t"` for text are the default values, you do not need to specify them.
{% endhint %}



