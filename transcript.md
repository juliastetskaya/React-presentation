Hi, my name's Julia and today I'll tell you about what React is and why you should learn it.

React is a JavaScript library for building fast and interactive user interfaces. It was developed at Facebook in 2011 and currently it's the most popular JavaScript library for building user interfaces. As you can see on this slide React is dominating the space of libraries and frameworks for building user interfaces. Other two popular players here are Angular and Vue. So if you want to expand your job opportunities as a front-end developer you should have React on your resume.

At the heart all React applications are components. The component is essentially a piece of the user interface. So when we are building applications with React we build a bunch of independent, isolated and reusable components and then compose them to build complex user interfaces.

Every React application has at least one component which we refer to as a root component. This component represents the internal application and contains other child components. So every React application is essentially a tree of components.

Here’s an example. Let’s imagine we want to create an application like Twitter. We can split this page into components like NavBar, Profile, Wall and SideBar. Here’s a representation of these components in a tree. So on the top we have App and below that we have NavBar, Profile, Wall and SideBar. Wall includes several Tweet components. And each Tweet component can include a Like component. SideBar component includes a Followers component and a Trends component. All these components we can reuse on other pages or even in different applications. So as you see each component is a piece of UI. We can build these components in isolation and then put them together to build complex UIs.

In terms of implementation a component is typically implemented as a JavaScript class that has some state and a render method. The state here is the data that we want to display when the component is rendered. And the render method as you can tell is responsible for describing what the UI should look like.

The output of this render method is a React element which is a simple plain JavaScript object that maps to a Dom element. It’s not a Real Dom element it’s just a plain JavaScript object that represents that Dom element in memory. So React keeps a lightweight representation of the Dom in memory which we referred to as the Virtual Dom. Unlike the browser or the Real Dom this Virtual Dom is cheap to create.

When we change the state of the component we get a new React element. React will then compare this element and his children with the previous one. It figures out what is changed and then it will update a part of the Real Dom to keep it in sync with the Virtual Dom. So that means when we are building applications with React unlike vanilla JavaScript or jQuery we not longer have to work with the Dom API in browsers. In other words we no longer have to write code or queries and manipulate the Dom or attach the event handlers to Dom elements. We simply change the state of our components and React will automatically update the Dom to match that state. And that’s exactly why this library is called React. Because when the state changes React essentially reacts to the state change and updates the Dom.

Here’s an example that React only updates what’s necessary. Even though we create an element describing the whole UI tree on every tick, only the text node whose contents has changed, gets updated by React DOM.

The main advantages of React. At first React Builds upon JavaScript fundamentals. Therefore, the React is easy to learn, especially by those programmers who already know JavaScript.

The second advantage is one direction data flow from Parent to Child. This helps components to be simple and predictable. The third advantage is most components in React consist of nothing more complicated than render, properties and state. And the last advantage is simple integration with large applications and other libraries.

All these advantages make React very popular today. It’s used by such famous companies as Facebook, Instagram, Netflix, the New York Times, Yahoo! Mail, WhatsApp, Dropbox and many-many others.

I hope you enjoyed my presentation and thank you for your attention.