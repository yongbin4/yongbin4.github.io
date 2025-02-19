---
layout: single
title:  "For Python Beginners!"
categories: coding python
toc: true
author_profile: false
---

## Python foundations<br/>
**Here are few things I scribbled down when I revised python after long service in Korean Army.**

### Object-Oriented Programming
[link]<https://realpython.com/python3-object-oriented-programming/>

Now i know that instance is inside a class.

* Class
* class attributes
  * Instance
  * Instance attributes

.\_\_init\_\_() , .\_\_str\_\_() are called dunder methods because they begin and ends with double underscores.

### Class and Instances
Classes are used to create user-defined data structures. Classes define functions called methods, which identify the behaviors and actions that an object created from the class can perform with its data.

A class is a blueprint for how something should be defined. It doesn’t actually contain any data. The `Dog` class specifies that a name and an age are necessary for defining a dog, but it doesn’t contain the name or age of any specific dog.

While the class is the blueprint, an instance is an object that is built from a class and contains real data. An instance of the `Dog` class is not a blueprint anymore. It’s an actual dog with a name, like Miles, who’s four years old.

Put another way, a class is like a form or questionnaire. An instance is like a form that has been filled out with information. Just like many people can fill out the same form with their own unique information, many instances can be created from a single class.

### Namespace and Scope
This document will explain what namespaces and Scopes in Python. Python namespaces, the structures used to organize the symbolic names assigned to objects in a python program. Objects are everywhere in Python. Literally everything that python program creates or acts on is an object.

 The statement x = ‘foo’ creates a symbolic name x that refers to the string object ‘foo’.

 Python namespaces work like a dictionary in python. In namespace, keys are object names and the values are the object themselves.

## There are four types of namespaces

1. Built-in
2. Global
3. Enclosing
4. Local

# Built-In Namespace

The built-in namespace contains the names of all of python’s built-in objects. 

![Text, letter Description automatically generated](/assets/images/namespace1.png)

# Global namespace

The global namespace contains any names defined at the level of the main program. Also interpreter creates a global namespace for any module that is imported to program

# The Local and Enclosing Namespaces

The interpreter creates a new namespace whenever a function executes. That namespace is local to the function and remains in existence until the function terminates. ­­­­­![Graphical user interface, text, application Description automatically generated](/assets/images/namespace2.png)­­­­­

The Globals() function

![Graphical user interface, text, application Description automatically generated with medium confidence](/assets/images/namespace3.png)

```
Global functions can be modified
and changed.
```

The locals() function

![Graphical user interface, application, Teams Description automatically generated](/assets/images/namespace4.png)

Local function is just a copy of the local namespace.

Modify Variables Out of Scope

Only mutable argument can be modified outside of scope (local, global)

The global declaration

![Graphical user interface, application, Word Description automatically generated](/assets/images/namespace5.png)

Same logic applies to nested functions.

  ![](/assets/images/namespace6.png)
