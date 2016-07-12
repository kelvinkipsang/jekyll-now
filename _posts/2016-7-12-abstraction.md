---
layout: post
title: applications of Abstractions
---


*Abstraction* means providing the essential features without showing its inner details or hiding internal implementation

1.We can enhance the internal implementation without effecting outside world. 
2.Abstraction provides security. A class contains lot of data and the user does not need the entire data.
3.he advantage of abstraction is that every user will get his own view of the data according to his requirements and will not get confused with unnecessary data.

Let’s begin with abstraction. A real world example is the http protocol. This protocol presents an interface to clients. The client passes a message to a server, using this interface, and there’s an expected behavior that goes along with it. If you POST a URL to a server, for example, the client expects a certain sequence of events to happen.


Suppose you are having a mobile,it has information about two aspects first one User aspects and nest one is Engineer aspects . For a user mobile manufacturer hides the Engineer aspects which is necessary only when you give your mobile to service centre for repairing . So when you press numbers to make call you don't care about whats happening there inside after pressing buttons,you just enjoy calling,So in this way abstraction provides Easiness,Simplicity.

Now suppose you went to atm,swiped your card to withdraw money,some instructions to be followed displayed on the screen,you provide some info like pin code of your account,again some options appeared on screen like withdraw,balance check....,Now these things are happening inside,but you are not knowing that how queries are being generated based on your inserted info in atm machine,after queries generation which database these queries are going to,where that database is located,which database is being used whether Oracle or Mysql,which language has been used for these implementation like whether java or c or c++,You as a user not knowing anything about these info,so its tough to hack that machine,because you don't have enough knowledge about internal implementation,you are using just UI(user interface) for your transaction,If you will try to know about any information mentioned above from the bank people they may call the police by thinking that you are a hacker.

So Actually i want to convey that this way they provide easiness to user and security to systems.
