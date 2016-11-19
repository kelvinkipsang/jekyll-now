---
layout: post
title: The Story of self Parameter in Python, Demystified(part 2)
---

Let me first clarify that Point.distance and p1.distance in the previous blog are a bit different.

```python

>>> type(Point.distance)
<class 'function'>
>>> type(p1.distance)
<class 'method'>

```


We can see that the first one is a function and second, a method. A peculiar thing about methods (in Python) 
is that the object itself is passed on as the first argument to the corresponding function. In the case of the above example, 
the method call p1.distance() is actually equivalent to Point.distance(p1). Generally, when we call a method with some
arguments, the corresponding class function is called by placing the method's object before the first argument.
So, anything like obj.meth(args) becomes Class.meth(obj, args). The calling process is automatic while the receiving process 
is not (its explicit).

This is the reason the first parameter of a function in class must be the object itself. Writing this parameter 
as self is merely a convention. It is not a keyword and has no special meaning in Python. We could use other names 
(like this) but I strongly suggest you not to. Using names other than self is frowned upon by most developers and 
degrades the readability of the code ("Readability counts").

## Self Can Be Avoided
By now you are clear that the object (instance) itself is passed along as the first argument, automatically. This implicit behavior can be avoided by making a method, static. Consider the following simple example.

```python

class A(object):

    @staticmethod
    def stat_meth():
        print("Look no self was passed")

```

Here, @staticmethod is a function decorator which makes stat_meth() static. Let us instantiate this
class and call the method.

```python

>>> a = A()
>>> a.stat_meth()
Look no self was passed

```

From the above example, we are clear that the implicit behavior of passing the object as the first
argument was avoided using static method. 
All in all, static methods behave like our plain old functions.

```python

>>> type(A.stat_meth)
<class 'function'>
>>> type(a.stat_meth)
<class 'function'>

```
