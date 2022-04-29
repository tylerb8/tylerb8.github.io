---
layout: essay
type: essay
title: Something's Off
# All dates must be YYYY-MM-DD format!
date: 2022-04-28
labels:
  - Software engineering
  - Athletic software engineering
  - Technical Interviews
  - JavaScript
  - Coding Standards
  - ESLint
  - Design Patterns
  - Semantic UI React
  - Meteor
---

## What are Design Patterns
A design pattern isn’t a finished design that can be implemented directly into code but rather a description or template of how to solve a problem that can be used in many different situations. In software engineering, a design pattern is like a template. It allows you to generalize solutions so that they can be reused in commonly occurring problems. Before taking this class, I have personally never heard of design patterns in software development. However, after gaining a better understanding of design patterns, the advantages are abundant such as reusability, improved efficiency, and enables the prevention of subtle issues by using effective software design techniques. 

Although there are numerous types of design patterns, in this essay, we will be looking at just six: Prototype Design Pattern, Observer Design Pattern, Publish and Subscribe Design Pattern, Model-View-Controller Design Pattern, Singleton Design Pattern, Factory Design Pattern, and how my group has implemented them in a website called [Manoa Eats.](https://manoa-eats.xyz/#/) 

## Types of Design Patterns

- Prototype Design Pattern:
The Prototype design pattern is about class instantiation, which allows you to inherit attributes and methods from other classes. One of the ways the prototype design pattern was used was as a javascript class in the API directory to encapsulate the MongoDB collections.
<br>
- Observer Design Pattern: 
The observer design pattern is a behavioral design pattern that allows us to communicate with the class’s objects. The observer pattern specifically enabled us to be notified during a change to a class. When a change was made to a class, such as submitting an auto form with Uniform a HandeChange, which is Reactive Data, will allow the MongoDB collection to update accordingly. An example is in the Addreview.jsx file when submitting a form. When new data was entered into the form, and the submit button was pressed, a notification would be enacted, and the function SubmitForm will run, which allows the data to be inserted into the Reviews Collection. 
<br>
- Publish and Subscribe Design Pattern: 
The publish/subscribe pattern allows the exchange of messages between publishers and subscribers. The publisher first publishes messages to a channel that the subscriber can then sign up to use. This enables the subscribers not to receive all messages directly but only specifically required messages. This design pattern is used in all our files in our page directory. We first created API classes that made a simple schema or database with MongoDB. The publications are handled through our /Startup/server/Publications.js, which publishes the content to the user, vendor, and or admin. Our website uses “withTracker,” which connects Meteor data to React components for a page to subscribe to publications. First, the page will subscribe to the corresponding channel; then, it will return the related data once the data is ready. 
<br>
- Model-View-Controller Design Pattern: 
The Model-View-Controller (MVC) design pattern represents how the information is presented and accepted by the user. The user first uses the controller, which manipulates the model, and updates the view, which the user then sees. In our case, the controllers are the forms created using React Uniforms, which then manipulates the model (MongoDB) and finally updates the user’s view (React). 
<br>
### Singleton Design Pattern:
The singleton design pattern is used as a global variable/class. This provides only one instance but a global point of access to that instance. The singleton design pattern is used in our page components by exporting the created component to a page layout. One example is the Restaurant.jsx component which is used in the AllRestaurant.jsx page. The AllRestaurant.jsx page uses the Restaurant.jsx component as a template to list out all the restaurants as card components. 
<br>
### Factory Design Pattern: 
The factory design pattern provides an interface for creating objects in superclasses that can use subclasses to create the instance of the class. This allows us to create objects without exposing the underlying logic of the class. This is one of the four main design patterns and can be seen everywhere in our code. One example is creating a simple schema “RestaurantsCollections” in API/Restaurantscollections.js/ to define our variables in the collection. We then instantiated that API class in our files in our restaurant components and page directories. 


~
