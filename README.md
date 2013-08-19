Krip
====

web-frameworks are about HTML+CSS+Javascript that simplify creation of web applications, built around MVC.
This is not that framework. In fact, it probably barely classifies as a framework in the conventional sense. 
It is an entirely new way of thinking about web-applications that makes them easy to implement, deploy, 
compose with each other and integrate with legacy systems and API systems.

1. Developing a product managers perspective. 
-----------------------------------------------

Have you ever been in a product management session of a web application? Have you watched how the PM walks up to a 
whiteboard and draws the elements s/he wants and draws arrows describing what should happen next? When a developer starts
to develop this thing which, after a few passes of cleaner diagramming gets pretty well specified, s/he must now convert
this specification into a composition of PHP/Ruby/your-favorite-web-app-language/HTML-templates/CSS/DigitalAssets/MobileExceptions etc. etc. etc. The code coming out at the end of it is complex, has taken far more effort than it needed, and usually painful to maintain.

Imagine, however, if all you needed to do was to take the clean diagramming, add a few details to it, and you have a 
functioning application. Not only that -- when you come up with a flow, you can re-use it in other applications 
as a part of a library. Then imagine that when comes the moment of site redesign, as it invariably does every year, 
modifications needed are minor, and easy to do --- making it a one week project, not a 2 quarter one. 

2. How is this possible? 
-------------------------

Before we describe this, a little bit of terminology may be necessary. Every piece of code is intended to produce an Outcome. 99% of the developer's job is to express how the outcome may be achieved through a very tight and precise sequence of operations. E.g. fetch this piece of data, render it like this, make it sensitive to these events and when the events occur, do something else. 

This is INTENTIONAL programming. Every piece of code written has a specific intention to move us closer to the desired outcome. Programming language fanatics will understand this as the "operational semantics" of the system. Intentional systems describe "how to make it happen". 

The opposite of INTENTIONAL programming is EXTENSIONAL programming. In extensional programming, one does not specify a tight series of operations, but expresses a desired outcome. A product manager's wire-frame is an example of extensional programming. Programming language fanatics will understand this as "denotational semantics" of the system. Extensional systems describe "what must happen". 

Of course, short of magic, extensional programming is generally not realizable (i.e., we can never build a properly extensional programming system, that allows us to say things like: find me the primes less than 17000 in under a microsecond). But, there are constrained domains where this is possible and we can create extensional systems that achieve this goal. 

This project is intended to produce an EXTENSIONAL web application framework that will allow extensional specifications of web-operations and let them be automatically implemented in one or more different web-technologies. Once a web-application can be specified in extensional terms, all the benefits listed above become possible since the implementation is now free to select from many available intentional paths to achieve the desired outcome. 

3. What needs to happen?
--------------------------

0. Create a basic extensional specification language. Pick 2-3 target applications and express them in this framework. Iterate to get the basic specification to a reasonable state. 
1. Implement the basic spec in a single web-technology target (e.g. Apache+PHP+HTML+CSS+Jquery). 
2. Extend specification languages to add more complex and or advanced features and repeat. 


