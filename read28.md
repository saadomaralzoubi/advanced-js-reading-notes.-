## Preparation Materials

### The Component Lifecycle

it details the life of a component. Like us, components are born, do some things during their time here on earth, and then they die
<br>

A component can only be in one stage at a time. It starts with mounting and moves onto updating. It stays updating perpetually until it gets removed from the virtual DOM. Then it goes into the unmounting phase and gets removed from the DOM.<br>

### Mounting

Since class-based components are classes, hence the name, the first method that runs is the constructor method. Typically, the constructor is where you would initialize component state.

Next, the component runs the getDerivedStateFromProps.<br>

Now we come to the render method which returns your JSX. Now React “mounts” onto the DOM.

Lastly, the componentDidMount method runs. Here is where you would do any asynchronous calls to databases or directly manipulate the DOM if you need. Just like that, our component is born.

## Updating

This phase is triggered every time state or props change. Like in mounting, getDerivedStateFromProps is called (but no constructor this time!).<br>

Next shouldComponentUpdate runs. Here you can compare old props/state with the new set of props/state. You can determine if your component should re-render or not by returning true or false. This can make your web app more efficient by cutting down on extra re-renders. If shouldComponentUpdate returns false, this update cycle ends.<br>

## Unmounting

Our component lived a good life, but all good things must come to an end. The unmounting phase is that last stage of the component lifecycle. When you remove a component from the DOM, React runs componentWillUnmount right before it gets removed. You should use this method to clean up any open connections such as WebSockets or intervals.<br>

## Composition vs Inheritance

Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”. <br>

It's recommended that such components use the special children prop to pass children elements directly into their output.
