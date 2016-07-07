---
layout: post
title: Getters & Setters
---



Getters and Setters are used to effectively protect your data, particularly when creating classes. For each variable, the get method returns its value, while the set method sets the value.

Getters start with get, followed by the variable name, with the first letter of the variable name capitalized.
Setters start with set, followed by the variable name, with the first letter of the variable name capitalized.

*Example:*
public class Vehicle {
  private String color;

  // Getter
  public String getColor() {
    return color;
  }

 // Setter
  public void setColor(String c) {
    this.color = c;
  }
}

The getter method returns the value of the attribute.
The setter method takes a parameter and assigns it to the attribute.
The keyword this is used to refer to the current object. Basically, this.color is the color attribute of the current object.

Once our getter and setter have been defined, we can use it in our main:
public static void main(String[ ] args) {
  Vehicle v1 = new Vehicle();
  v1.setColor("Red");
  System.out.println(v1.getColor());
}

//Outputs "Red"
Try It Yourself

Getters and setters allow us to have control over the values. You may, for example, validate the given value in the setter before actually setting the value.

 [try the code here](http://code.sololearn.com/759/#java)
