# State Management Course

# 🤔 **What is state management?**

There is a certain agreement in the developer community about some topics that are commonly seen as big problems: naming things, cache, and state management. When building UI and user experiences through web applications one of the biggest struggles is about how to deal with the application state.

## **But, what is state and why does it need to be managed?**

The process of web development deals with a pretty complex environment. The browser offers the developer a set of mutable nodes in a tree form: the DOM. Several frameworks came to light across the years to handle and work with this structure, one that stands out as a pioneer of the second era of Javascript is React.

The main rationale behind React is that to manipulate the DOM we need to write imperative javascript code. React came to say that we can do better: There is a way to write **declarative code** to create the UI.

> The UI is a function of the state.
In other words, **state is a data structure that represents a snapshot of the reality in the application interface** or more simply, it is a programmatic representation of what the user sees at a certain moment.
The state is the expectation that the user has for how the application should work, this is part of the constant battle that we fight when adding state to the applications. “Is what the user’s seeing exactly one to one with what the state internally represents?”.

## **What problems do we need to solve?**

Manage state is a known problem in computer science, there is a big branch of research that created a concept called finite state machines, a mathematical model that represents a "machine" that can be in exactly one of a finite number of states at any given time. The machine can transition to one state or another in response to some inputs. This definition is exactly what we want from our interfaces.

> Check out [xstate.js.org](https://xstate.js.org/) to learn more about state machines and javascript. If you are interested in implementing this pattern with React check out [this](https://kyleshevlin.com/how-to-use-usereducer-as-a-finite-state-machine) article to learn how to work with it using the `useReducer` hook.
Now, where does the state comes from? The state of our applications can be described as a mix of two types of data.

1. UI state: The kind of state that is derived from the user interaction with certain pieces of the UI, like Modals, alerts, even authentication. We have complete control and ownership of this state. The type of state that gets killed every time you refresh your browser. It is synchronous and easy to retrieve.
2. Server state or Cache state: The kind of data that is remotely persisted, asynchronous with shared ownership that can be potentially Out of Date.

React is in its core a **state management solution**, it offers the required tools to manage the state that belongs to the UI by itself but when we need to deal with what we call server state then React is not enough and we need to go out and look for a 3rd party library solution.

**Server state** presents new challenges to deal with like Caching, dedupe requests, incremental fetching, mutations, outdated requests, synchronization of the data.

In the early days of React and the Flux pattern, the solution for all this (and a few other quirks like prop-drilling) was just to mix and merge these two states and put it high on the app creating a **global state**. This is what libraries like Redux do but that was not enough to deal with the different natures of the state. A lot of developers experience the increased complexity of this type of global state solution.

So in summary:

- Server state is data that we don’t control. It is a snapshot of data that some API returned.
- UI state is predictable, easy to manage, and to reason with.

> Watch [this](https://www.youtube.com/watch?v=seU46c6Jz7E) talk from Tanner Linsley: It's Time to Break up with your "Global State” for more insights about this.

----

# 📚 Course/Workshop Overview

The React ecosystem have a wide variety of options to help you manage the state of your application, and as the applications grows in complexity also the solutions becomes more complex or smart.

In this course we will review several concepts and solutions to the state management problem in React applications, starting from the very basics learning what is the state and how the UI library itself can help us with this matter.

Some of the stuff that you will learn in this course are:

- React hooks and how React is a state management solution.
- react-query and how to split state in two categories UI state and server/cache state
- SWR as another option to handle the two main natures of the state.
- RTK as a global state management solution
- Mobx-state-tree, zustand, jotai and other libraries
- xstate as a different approach to the state management problem.

## 🎯What will be included in the course/workshop?

The course/workshop  attempt to be a very comprehensive collection of different resources and media to help your learning process and deep understanding of the different topics and concepts. The goal of the course is not just teach you about concepts but help you to create the tools and skills that will help you level up in your career.

To accomplish the aforemention goal the course/workshop includes:

- 🎥 Video explanation
- 💪 Challenges and solutions
- 📺 Screencasts
- 🎧 Video/Audio interviews
- 📒 Articles written by subject experts.

----

# 👨🏻‍💻 Who Am I?

I’m Matías Hernández

I’m a Chilean Software Engineer with several years of experience on the web development world. Building solutions is what drives me everyday to the contious learning process and I invite you to live the same experience.

I help other learn and level up their careers by sharing my own learnings and knowledge through different media like [video screencasts/courses at egghead](https://egghead.io/q/resources-by-matias-hernandez), [writing, ](http://matiashernandez.dev/)[podcasts](http://cafecon.tech/) and some [open source software.](http://github.com/matiasfha)

You can find me in [Twitter](http://twitter.com/matiasfha)

