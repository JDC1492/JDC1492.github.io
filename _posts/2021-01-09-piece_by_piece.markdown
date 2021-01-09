---
layout: post
title:      "Piece by piece"
date:       2021-01-09 12:52:27 +0000
permalink:  piece_by_piece
---


Components seemed like such a small peice to the React framework when I first read about them. After a few weeks of labs and the readings, I look at components in a whole new light. Components could be looked at like lego blocks, small peices of connectable "blocks" that when placed together in an organized manner could create something much larger. 

Components allow us to keep our code organized and separated into re-usable. A common component could be a class component.   An example of this could be written as:

`class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}`

This bit of information provides us with a 'block' to place somewhere within our application. So wherever we place the `<Welcome />` componenet the return text that we see in the render method should be rendered or shown to the user on the page. Of course with a few extra steps such as exporting the file(telling this file be prepared to be used within another file)

`export default Welcome;`

and the importing of that file within another file `import Welcome from "./properFilePath"` 

With the necessary code in place we could easily place this code within the component tree to be shown as delcared in the actual class. A built out application may look something like this: 

`class App extends React.Component {
  render() {
    return (
		<Welcome />
		<Header />
		<Body />
		);
  }
}`





