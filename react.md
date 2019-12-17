# ASSESSMENT 4: REACT ASSESSMENT
## Interview Practice Questions

Answer the following questions. First, without external resources. Challenge yourself to answer from memory. Then, research the question to expand on your answer. Even if you feel you have answered the question completely on your own, there is always something more to learn.  

1. Correctable True/False: Mark the following TRUE or FALSE. If FALSE, correct the statement to be TRUE.

- React is a modern, efficient answer to complex UI applications (true/false) true
- React will only render on the server using Node.js (true/false) true
- React is a full stack framework for modern web applications (true/false) false
- React is a flexible library that plays the role of V in an MVC framework (true/false) true
- You should always update a component's state directly using this.state (true/false) false
- React is made up of encapsulated components that manage their own state (true/false) true
- React components render HTML (true/false) true 


2. What are "smart" and "dumb" components? Explain the difference and also add why we bother to make the distinction between them.

  Your answer: 0

  Researched answer A Smart Component is any component which manages its own state. When working with Babel or ES6-style React, we've come to know this as any class-like object that extends Component. This includes either React.Component or in our case Nui.Types.Component.
                    
  export default Nui => class MyComponent extends Nui.Types.Component {
  render() {
    return (
      <h1>Hello World</h1>
    );
  }
}
A Dumb Component can very easily be defined as a stateless component. A stateless component is much more efficient than a stateful one, because it doesn't require as many computer resources to render (memory, CPU, and GPU in terms of graphic-intensive apps).
export default Nui => () => (
    <h1>Hello World</h1>
);
3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?

  Your answer: Manage our dependencies

  Researched answer: In general, a package is simply a folder with code and a package.json file that describes the contents. When you want to use another package, you first need to add it to your dependencies. This means running yarn add [package-name] to install it into your project.



4. What is the difference between component state and props? Your answer should include a short explanation of both.

  Your answer: State is internal, props are how we pass properties

  Researched answer: In a React component, props are variables passed to it by its parent component. State on the other hand is still variables, but directly initialized and managed by the component.

                    The state can be iniztialized by props.

                    For example, a parent component might include a child component by calling



5. How would you explain state to a friend who doesn't know code?

  Your answer:  states are objects that are managed within a component
