#React Funamentals

create app by npx will have all the dependenies
```npx create-react-app app-name```

React has two type of components in erlier version 15 or less then 16.0 
Class based component and functional components
class based component also called statefull componennt and functional stateless componnet

in 16 version
react has hooks feature which provides states in even functional component and we can call it container, statefull or smart component
presentational stateless or dumb componnet is the component which not used hooks like useState


We can access method as well by using props and fire event from the component
if you pass something in argument you will have to use bind method while calling the function like this functionName.bind(this, 'data to change')
In short bind method helps to passing argument on function - and its recommended
Alternatively you can use arrow function and inside that arrow function call the method with argument

inline style can be done by in object format with javascript syntax something like below

```
const myStyle = {
	color: 'red',
	border: '1px solid red'
}

<element style={myStyle}
```


Useful Resources & Links
create-react-app: https://github.com/facebookincubator/create-react-app
Introducing JSX: https://reactjs.org/docs/introducing-jsx.html
Rendering Elements: https://reactjs.org/docs/rendering-elements.html
Components & Props: https://reactjs.org/docs/components-and-props.html
Listenable Events: https://reactjs.org/docs/events.html


If else to show something
```
{
	coditions  ? 
	<div> show something 
	</div> : null
}```

we can also use javascript approach in render function to redner html in flag

```
render(){
  let something = null;
  if(true) {
    something = (
    <p>Hey am able to visible </p>
    )
  }

  // before return
  return(
    {something}
  )
}
```


Loop with map - same js approach

deeleting array with copy not with the reference is a good approach - splice to delete slice to copy
even use spread operator instead of slice - like that [...this.state.persons]

changing something in object dont use reference directly take a copy same lie array using spread operator or object.assign() - I prefer spread like below
```const obj = {
	...this.state.persons[index]
}```

CLASSES
trick to add multiple classes dynamically below
```let classes = ['red', 'bold'].join(' '); // red bold```


Radium can be used for pssudo and media query in js file in react js
another is styled-components
CSS module


SASS
```npm install node-sass --save```
and rename css to scss

Router
```npm install react-router-dom```


Keep less code in App.js speciallt the JSX try to make component for each sections and keep handlers and states in app js - so you can use them in all the componnets

