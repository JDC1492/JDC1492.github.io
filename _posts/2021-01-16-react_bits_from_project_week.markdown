---
layout: post
title:      "React bits from Project week"
date:       2021-01-17 02:39:13 +0000
permalink:  react_bits_from_project_week
---


The final project is completed. I've learned about and created with React. Out of everything I've become familiar with at the flatiron school, the react framework has certainly made it high on my list. `(I love them all equally :-] )`

Using React, I created a  web application through the use of components. Components could propably be compared to the individual bricks for bulding a house. Just as each brick is used to build that house, the same could be said about components. In our case though, each brick holds some peice of information that serves a purpose for that house.  

While my project isnt a large one, I found myself writing components in the style of both functional and class components. As I'm still learning about both,  I'd find it tough to choose which one I prefer between the two.  I **CAN** confidently say that both equally have their advantages. I can share a bit of what I learned about both.

Class Components and functional components both require a certain syntax to be wirtten for each. 

a basic class component is written like :

```
class Arcade extends React.Component {
  render() {
    return <h1> I wanna buy {this.props.game}!</h1>;
  }
}
```

a functional class:

```
function Arcade(props) {
  return <h1>I wanna buy {props.game}!</h1>;
}
```

Within these examples you can also see another difference between the two. The render method has to be called to return JSX inside of a class component. For a functional component,  it does not.  Another difference is that Class components are capable of making use of the various lifecycle methods, which could be thought of as moments in time of a components life. Functional components dont have access to these *exactly*.... but are afforded the use of hooks.  From the official documentation:

> Hooks are functions that let you “hook into” React state and lifecycle features from function components.
> 

As I learn more about react I find myself more interested in the possibile things that I could build. I plan to continue being curious about code and aim to become a bit better in each attempt I make.





