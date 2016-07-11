---
layout: post
title: Abstraction
---



Data abstraction provides the outside world with only essential information, in a process of representing essential features without including implementation details.
A good real-world example is a book. When you hear the term book, you don't know the exact specifics, such as the page count, the color, or the size, but you understand the idea, or abstraction, of a book.
The concept of abstraction is that we focus on essential qualities, rather than the specific characteristics of one particular example.

In Java, abstraction is achieved using abstract classes and interfaces.
An abstract class is defined using the abstract keyword.
- If a class is declared abstract it cannot be instantiated (you cannot create objects of that type).
- To use an abstract class, you have to inherit it from another class.
- Any class that contains an abstract method should be defined as abstract.

**Abstract Class**

For example, we can define our Animal class as abstract:
abstract class Animal {
  int legs = 0;
  abstract void makeSound();
}

The makeSound method is also abstract, as it has no implementation in the superclass.
We can inherit from the Animal class and define the makeSound() method for the subclass:
class Cat extends Animal {
  public void makeSound() {
    System.out.println("Meow");
  }
}
