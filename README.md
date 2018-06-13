# My-React-Learning-Curve

## Abstract

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
      render(){
        return(
        
        );
      };
    }
```
