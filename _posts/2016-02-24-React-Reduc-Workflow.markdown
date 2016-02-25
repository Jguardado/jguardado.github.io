---
layout: post
title: React, Redux, and Worklflow
date: 2016-02-25T14:37:44.000Z
categories: update
---

<img src="/images/fulls/01.jpg" class="fit image">

<h1>React, Redux, and Workflow</h1>

When deciding to build an application its important to consider which framework best suits your objectives. If you've surveyed your options and concluded that React.js is your best choice then your left with an additioanl decision. Which model framework will you use to supplement your React views?

I've recently built an application in React and Redux and found it to be a very effective tool for my specfic purposes. The redux documentation is very easy to read and fortunately there is a pleathora of advice online for how exactly to go about building with this pairing. When choosing to dive into this stack you'll want to remmeber one key point. The workflow for React and Redux is one directional. 

An important aspect of React components is their state. This is an easily misunderstood intricacy of using Redux with React. When coupling with Redux there are two very similar views. One is the React Component and the other is the Redux Container. Containers serve the same purpose as the components except they provide access to the one way directional operations of the Action, Reducer, Container flow that exists in Redux. The idea of "state" takes on two forms at this point. Because the React state is what is immediately accessible and rendered from the component. Whenever there are changes to the state the view is re-rendered. This is very useful when doing things like making a view visible or not. However when reading through the redux documentation you might find another reference to state. This "state" is representative of the store, or the collection of redux states that are passed along to the containers to be rendered to the DOM.


To simplify this process I recommend that you start at the begining of the chain. All changes are initiated by actions. An action can be anything from an item select to an API request. Once and action is triggered the results for that action are stored in the a reducer. Reducers capture the results of the action and assist in making that action's results passable into the conatiner space. This interconnectedness comes from the appropriate chaining via imports (in ES6). For each step you must import the proceeding steps exported action. When using Redux you'll also have a central collection of all reducers that has access to all the actions and reducers. This is the compiled reucers file. It connect the action the reducers and indicates name of the results object or array that can now be imported into a container.

Within Containers you should only be changing the state of by the usage of actions. This way you can maintain the one way directional workflow that is designed into the React/Redux combo. I've found that one can run into serveral unexpected problems when trying to alter the state directly. You might have heard some references to mutating the state. This is an example of that. Alternatively you can alter the state of a React component directly. For anyone who is an Angular developer this is the opposite of two way data binding. The cyclical nature of this process allows to capture each state as its render and opens the door to easy acces to previous states.

I hope this posts helps provide a bit of explaination to teh workflow between React and Redux. Fortunately for all of us the documentation for both frameworks are fairly easy to follow and have lots example and clear explanations to the important concepts. I've included links to both below you your convenience. Happy Coding.

<a href="https://facebook.github.io/react/docs/getting-started.html">React Docs</a>

<a href="http://redux.js.org/">Redux Docs</a>

