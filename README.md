# My-React-Learning-Curve

## Some Random Pointers

* *we need to keep id as root of element where we wanna embed our react components in main html*
* *ReactDOM has a function called render which main task is to render our main component in our html.*
``` javascript
ReactDOM.render(<main_app>,
                document.getElementById('root'))
```
* *ReactDOM.render will only take single component and target*
* *Use of JSX allows us to close the tag like this: <tagName/> if it doesn't have body like image tag.*
* *Creating Elements can be done using jsx as well:*
```javascript
  const element = {
    type: 'h1',
    props: {
      className: 'greeting',
      children: 'Hello, world!'
    }
  };

```
* *React Only renders the changes rather then reloading the entire page, React will compare the changes and updates only those*
* *React Component Should always be started with uppercase letter.*
* *Props should never be changed within the function hence making function pure. It won't show error though.*
* *Components when created with class should extends from React.Component class. For Eg:* *
```javascript
    class Class_Name extends React.Component
    {
      constructor();
      render(){
        return(
        
        );
      };
    }
```
* *constructor should always call super() before initializing any states*
* *All the states has to be defined in constructor()*
* *props will be preceded by this. when using class as component*
* *State inside constructor is a state* *
* *Class constructor should always call super() by passing props as arguments in it* 
* *Rendering when component is created is known as 'mounting' and destroying the component is known as 'unmounting'*
* *There are two methods which are known as 'lifecycle hooks' which are **componentDidMount()** and          **componentWillUnmount()** which    are called on creation and destruction respectively.*
* *this.setState() will take an object as argument and used to change the state of data so it will re-render the component      when some data is changed.For Eg:*
```javascript
  function user(username)
  {
    //This changes the old username with new one hence updating the component
    this.setState({userName:username})
  }
```
* *Updating State directly will no re-render the component hence setstate has to be used*
* *state of a component is local to it hence cannot be accessible outside that component*
* *state of a component is passed as props to its children.*
* *We use function for stateless component and class for stateful component*
* *Components data flow in unidirectional manner in top-down approach.*
> If you imagine a component tree as a waterfall of props, each component’s state is like an additional water source that joins it at an arbitrary point but also flows down.

* *To Use Function in class it should always be binded with constructor if you want that function to access state, or mainly    to use anything related with this keyword*
* *To Use Comment inside return statement you have to wrap it in braces as follow:*
```javascript
        {/*
          your stuffs
        */}
```

