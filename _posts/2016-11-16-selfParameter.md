---
layout: post
title: The Story of self Parameter in Python, Demystified
---

If you have been programming in Python (in object oriented way of course) for some time,
I'm sure you have come across methods that have self as their first parameter.
It may seem odd, especially to programmers coming from other languages, 
that this is done explicitly every single time we define a method.
As The **Zen of Python goes**, *"Explicit is better than implicit"*.

So, why do we need to do this? Let's take a simple example to begin with.
We have a Point class which defines a method distance to calculate the distance from origin.


```python

class Point(object):
    def __init__(self,x = 0,y = 0):
        self.x = x
        self.y = y

    def distance(self):
        """Find distance from origin"""
        return (self.x**2 + self.y**2) ** 0.5

```

Let us now instantiate this class and find the distance.

```python

>>> p1 = Point(6,8)
>>> p1.distance()
10.0

```
In the above example, __init__() defines three parameters but we just passed two (6 and 8).
Similarly distance() requires one but zero arguments were passed. Why is Python not complaining about
this argument number mismatch?

## What Happens Internally?
Part two comes out soon
