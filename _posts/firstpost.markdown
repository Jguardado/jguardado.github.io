---
layout: post
---
<img src="/images/fulls/03.jpg" class="fit image"> 
<h2>Demystifying the Functional Instantiation Pattern</h2>

<h4>A Simple Explanation of Functional Instantiation.</h4>

The topic of Instantiation Patterns seemed rather daunting from the first time I heard about it. Even pronouncing the word can be a bit a of a tongue twister. As I began to digest the idea, grasping the concept and thinking about it’s practical usage, it became clear that the term “functional instantiation” casted a bigger shadow then the concept itself. If you are familiar with basic Javascript objects then you have already dealt with the crux of functional instantiation.

It is really as simple as utilizing the basic function object that we use everyday in Javascript. In the below example we have our normal function closure:

<img src="/images/screenshot1.png">


Within our newFunction’s closure we have the ability to create methods that are only associated with our current function closure scope. We can then create an object inside of the function. 


As properties of this object we can then store additional functions that can be easily accessed by the object. These internal functions are referred to as methods. That object is now stored inside of our current closure scope we can access these methods by referencing first the object then its property. As we see in the below example:



Functional Instantiation is an easy introduction to understanding prototype chains. In the functional pattern we do not require a prototype because our methods are stored as properties of our locally created object, which is already inside of our current closure scope. That means when we make reference to any of the newly created methods Javascript will look within it is current scope and locate the object we are referencing.


You must return the object out of the functional closure. In this case we are returning our object “instances”.

This is just the beginning of instantiation patterns. As you explore them closer you’ll find each how they posses unique characteristics. I hope that it is helpful to know that you are starting from a much more familiar point that you might have previously assumed.

