PLAN 

Props, State, Context

1 What they are in principle

Props is just a shorter way of saying properties. Props are the information that you pass to a JSX tag.

2. Why you'd want to use them
We use props in React to pass data from one component to another (from a parent component to a child component(s)). They are useful when you want the flow of data in your app to be dynamic.

3. How you'd want to use them

How to use props without destructuring
To use props, you have to pass in props as an argument in your function. This is similar to passing arguments into your regular JavaScript functions. Here's an example:

function Tool(props) {
  const name = props.name;
  const tool = props.tool;
    return (
      <div>
        <h1>My name is {name}.</h1>
        <p>My favorite design tool is {tool}.</p>
      </div>
    );
}

export default Tool


How to use props with destructuring
The code for this section is entirely the same as the last section except for the method for declaring the props. 

function Tool({name, tool}) {
  
    return (
      <div>
        <h1>My name is {name}.</h1>
        <p>My favorite design tool is {tool}.</p>
      </div>
    );
}

export default Tool


The difference is in the first line of code. Instead of passing props as an argument, we destructured and passed in the variables as the function's argument.

Everything else remains the same.

Note that you are not limited to just single variables as your props data – you can equally pass in functions and even data from objects.

How to set default values for props
If you do not want your props data to be empty when you create them, you can pass in a default value. Here's how to do that:

function Tool({name, tool}) {

    return (
      <div>
        <h1>My name is {name}.</h1>
        <p>My favorite design tool is {tool}.</p>
      </div>
    );

  }
  
  Tool.defaultProps = {
    name: "Designer",
    tool: "Adobe XD"
  }
export default Tool


4. Give an example 

5. How they are interelated
6. How they are like
7. How they are different
8. When you would use one vs another
9. Advantages & Disadvantages
10. Trade offs. 

----------------------

The plan is to write an article and deploy so that we can send the link to other bootcampers. 

