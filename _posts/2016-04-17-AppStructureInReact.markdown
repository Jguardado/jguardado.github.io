---
layout: post
title: App Structure with React
date: 2016-04-25T14:37:44.000Z
categories: update
---


<h1>How to Structure your App in React</h1>

It's that time again to decide which framework you want to build your application in. You've done you're research, read all of the blogs about Angular, Backbone, Ember, and many others and you've come to the decision to use React. Maybe its because it one of the mot popular frameworks or maybe you wanted to verge into component based interfaces. Whatever the rational was hopefully it coincided with how React will be the best tool for the job, which should always be your number one concern when making decisions about your project.

React uses render statements to directly create elements on the DOM. This frees up the ability to create isolated components. These components can be arragned rather freely as well as be reused which also gives react the added benefit of a more simplicitic design. However, the free form design still requires some basic skelton to make sure all of the render statements and components can be view on the DOM.

The first step in setting up your React application after you've required React in you package.json or added the script tag to you html page is to connect React to you html page. This is done by adding an ID tag to a div in your html. Most commonly this tag is named "app" and it would look like this . This is establishing a point of contact for your react components, and at this point you can move over to seperate JS files to do the majority of your coding. React is best used with lots of modularity and seperation of concerns, as you can see at the onset.

Now that we have moved over to our JS files will want to make sure you do one of two options, depending which edition of Javascript you are writing in. If you are using ES5 you will require React at the top of the page. This will look like this: 