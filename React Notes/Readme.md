React JS:-
    - React js is javascript library uaed for building  user interface and single page application.
    - created by jordan walke at facebook.
    - it is most popular javascript library for frontend development.
    - 40 million developer are useing react for their programming stuff.
    - Now we are using rect js version 19 or v19.

History of React.Js:-
    - react js begin as an internal tool for dynamic facebook components.
    - created in 2011 but remain private initialy.
    - React js  was open sourcce by jordan walke & Tom Ochino at JS Conference at 2013.
    - initialy faced critism for combining html code in javascript on a single page.
    - It slowly gained success...., Now 40M+ developers are using react js.

Pre-requisite to download and use react js:-
    1. Node JS
    2. VS COde
    3. Extention (ES7 react/redux/graphql)

Ways of creating React JS Project:-
    1. CRA (Create-react-app)   ---->> Oldest Methods off creating react application

        install  --> npx create-react-app project_name
        execute --> npm start / npm run start

        Note: Now on 2025 onwards (CRA method is dead) -> RIP CRA

    2. React + Vite -->> This the fastest methods of creating react app(2min)

        install  --> npm create vite@latest
        execute --> npm run dev

File/Folder structure of react js :-

1. node_modules :
 - this is the folder which contain all necessary library & dependencies by react js.
 - you can ignore this folder completely

2. public :
 - this folder contains all static files lie images, videos, icons etc...

3. src(source) folder :
 - this folder contains all source file(the source file including react components, js files & css files etc...)
 - it is the main folder where we can create pages & component and write some code.

4. .ginIgnore file :
 - this file including all the files & folder that unnecessary for our react js project.
 - it simply ignor these files from our react js in deplyment time so that we can write unnecessary fileshere.

5. Eslint.config :
 - Eslint is a code analysis tool for identifying problematic pattern in javascript and if we face some dificulties or write some wrong code, it directlly indicate that in red marks or yellow marks.

6. index.html file :
 - the main file where react application is loaded serving as the entry point for the web browser.


 Package.json :->

  - this files contains all the details or configuration of this project
  - it includes name, varsion, description, script etc...

   Script :
    - div  -> we can execute the project (npm run dev)
    - build  -> we can generate the builkd file (npm run build)

   Dependencies :
   - in dependencies we will see react & react-dom.
   - react js is just a library for creating dynamic user interface.
   - React DOM used to render those dynamic components on web browser/web page.
   - React Native is used to render those components on applications (android & IOS)

   DevDependencies :
   - it stores the developement dependency like some extra package / library

 Extra Knowledge :->

 - Application are of 2 types
  1. Native Application :
    - if you develop any native application on spacific platform then it runs only spacific device.
     ex. if we developes native android app, then it always run on playstore.
    - Native Apps (android) -> java, kotlin
    - Native Apps (IOS) -> swift, c#

  2. Cross platform application :
    - if we develope any platform application then it execute both android & IOS device.
    - Cross Platform (android, IOS) -> React Native, Flutter

7. package-lock.json file :
 - it stores dependency of dev-dependency in package.json file.

Some Tools used on react js :-

- NPM -> node package manager (to install some external package/execute code etc...) - globally
- NPX -> node package execute (to install some local package & also execute some code) - locally
- RAFCE -> React Arrow Functional Component Expression
- RFCE -> React Functional Component Expression

Naming Convention in react js :-

 1. camelCase :
   - it is used for variable, function, methods, properties etc...
   - capitalized of each word except the first one.
   - ex. currentState
 2. PascalCase :
   - it is used for components name, class name, file name etc...
   - capitalized of each word.
   - ex. CurrentState
 3. snake_case :
   - it is not  commen in javascript but it is used heavilly in python.
   - Each word in separated by "_" and in small letter.
   - ex. current_state

 4. Kabab-case :
   - it is common for file name, css classes, ids etc...
   - Each word is separated by Hypen(-). and letter should be both capital & small.
   - ex. current-state


JSX in React :-

- JSX stands for javascriptXML, means (javascript + HTML).   
- JSX helps to write pure HTML code in javascript.
- Each JSX expression must have one parent element, which means if you try to return multiple element, react will through error, so that we can take a parent element to wrap the HTML code.

Components in React Js:-
    - In react js , a component is esentially a JS function or class that returns JSX.
    - In react components are of 2 type:-
        1. Class Based Component :- 
            -  Class Based component are created before 2016, where functional based components are not used.
            - Ex: 

                import React froom 'react';

                export class Welcome extends component{
                    render(){
                        return Hello World
                    }
                }

        2. Functional Based Component
            - Now we are using functional based component in everywhere.
            - This is modern and most recommended way oof writing react js component
            - Ex: 

                import React from 'react';
                export function Welcome(){
                    return Hello World
                }

Fragment in React JS:-
    - In react js, a component can't return multiple element, without a wrapper div.
    - When we give a wrapper div and bind all html element it return our all statement
    - Ex: 

        import{Fragment} from 'react';

        const App = () => {
        return (
            <fragment>
            <h1>Today is a great day</h1>
            <h2>Today we learn react</h2>
            </fragment>
          )
        }


        or


        const App = () => {
        return (
            <>
            <h1>Today is a great day</h1>
            <h2>Today we learn react</h2>
            </>
          )
        }

Dynamic Value in JSX:-
    - We can add any variable of your component in JSX using {} syntax.
    - EX: -

        function MyComponent(){
            const value ="Hello";
            retunt <p>{value}</p>;
        }

    - JSX allows you to write javascript expression inside curlly braces. We can do the dynamic value in operation, function call, expression....

            1. Variable --> We can embed any JS variable within JSX by enclosing it in curlly braces. The value of the variable will be inserted into the DOM at the respective location

            2. Expression -> JSX allow you to write js expression inside curl braces. this includes operation, function call, and other javascript expression

            3. Function call -> function, especially those that return JSX, can be invoked directly within your jsx.

Conditional Value in JSX :-
    - As per our normal condition, react alsso provide some conditions.
    - Ex:-

        return<p>{age >= 18 ? "Adult" : "Minor"}</p>

    - There are 4 types of condition we can apply oon react JS....
    1. Normal if case -> The code repeated multiple time, so its a drawback of applying condition in this way.
    2. Ternary operator -> In this way, the code doesn't repeated .And ternary operator is a good way of applying condition in react.
    3. Complex if case -> Sometime you might face complex if case.
    4. function call -> It prevents cluttering of variable outside and encapsulated such logics inside a function.

Import and Export :-
    - There are tree types of import and export statement are there
        1. Default Export and Import
            - default Export: - A file can have only one default export.
            - defaulr import:- When importing a default export, you can name the import whatever you like.

        2. Named Export and Import
            - Name Expot:- A file can have multiple named exports. Each named export must be explicitly exported.
            - Name Import :- When importing name export , the names must the export names exactly. Name Exports must be enclosed in curly braces.

        3. Mixed Export and Import
            - Mixed Export: - A file can have both default export & named import.
            - Mixed Import:- A file can have both default import & named export.

Looping in JSX/ React :-
    - We dont have for loops in JSX, so we have to use  .map() method of arrays.
        Syntax:-

            return(
                <ul>
                {students.map((student) => {
                    <li key = {student}> {student} </li>
                })}
                </ul>
            );

    - React Js uses Keys to differentiate each elements.

useState:- 
    - The react useState hoolls allows us to track state in a functional component.
    - state is basically refers to data or properties that need to be traking in an application
    - to use useStaate, first we import it into our component or files.
    Ex:-   importuseState fom "react;

    syntax:- 
        const[state,setState] = useState(0)

    - in the above syntax:-
        state = initial state
        setState = updates state

useEffect:-
    - useEffect is a hook allows us you to perform side effect in a component.
    - some examples of side effects are updating dom, fecth data ,timer etc...
    - useEffect mainly accept 3 argument.

    1. side effect function ->> This function use to apply side effects
    2. clean up function  ->> it is use to clean our previous states in a components
    3. dependency array ->> used to provide some dependency like, how our function will be work(time,seconds etc.....)

    - When we use, useEffect 1st we immport it, then we used it in a component

react-Routing:-
    - React Router is a standard library for creating dynamic routes and navigation in React JS Applications. It allows you to manage navigation in your app by defining routes that connect the URL paths to specific components.

    useParams Hooks:-
    www.webbucket.com/id-187332478641  -> Student details(We can use it, by the help of useparams)

    useNavigate Hooks:-
        home -> btn -> clicke -> about
        about -> btn -> clicke -> dashboard

Props:-
    - Props -> properties
    - React components use props to comuunicate with each other.
    - Every parent component can pass some information to its child components by giving them props.
    - props is like your HTML attributes but you can pass any javascript value through them, including objects =, arrays & function.

useContext ---->
    - react context is a way to manage state globally.
    - the problem->
        -> State should be held by the highest parent component in the stack that requires access to the state.
        -> To illustrate, we have many nested component, the components at the top and buttom of the stack need access to the state.
        -> to do this without context, we will need to pass the state as "props" through each nested component. this process is called "props drilling"

        -Solution:-
            -> We can useContext hook.
            -> useContext hooks have 3 State
                1. create context
                2. provide context
                3. consume context


useRef:------>
    - The useRef hooks allows you to persist value between renders .
    - It can be used to store a mutable value that doesnot cause a re-render when updated.
    - it can be used to access DOM element directly.
    - useRef() only return one item. it return a object called current.

    useRef() -
        1. persit value ----> value can be changed but it doesnot re-render that value when it changed.
        2. reference to another object

seMemo Hooks:---->
    - memo(memoization) ----remembering
    - The react useMemo hooks returns a memoized value.
    - the useMemo hooks can be used to keep expensive operation/task/function from running smoothly

React-redux:------>
    - Redux toolkit is a set of tools for building Redux Application with react.
    - It provide  a simplified way to manage global state by combining the benefits of Redux and react.

    Key Features of reactredux toolkit:-----
    1. Simplyfied store Setup:   RTK provides a simple way to setup a redux store with a single fuction call.
    2. Automatic Redux Store Configuration:  RTK automatically configures the redux store with the necessary middleware and setting.




Topic left in react JS:-
    1. props
    2. useState
    3. useEffect
    4. useContext
    5. React - Router
    6. useRef
    7. react-redux
    8. useMemo
    9. useCallback


Q2. Answer 

import React, { useState } from 'react';

function ToggleButton() {
  const [showText, setShowText] = useState(false); 

  const toggleVisibility = () => {
    setShowText(!showText);
  };

  return (
    <button onClick={toggleVisibility}>
      {showText ? "Hide" : "Show"}
    </button>
  );
}

export default ToggleButton;

// useState answer 
Q3. Answer 

import React, { useState } from 'react';

function FormComponent() {
  const [formData, setFormData] = useState({
    name: '',
    email: '',
  });

  const handleChange = (event) => {
    setFormData({
      ...formData,
      [event.target.name]: event.target.value,
    });
  };

  const handleSubmit = (event) => {
    event.preventDefault();
    // You could send this data to a server here
    console.log('Submitted data:', formData);
  };

  return (
    <div>
      <form onSubmit={handleSubmit}>
        <label>
          Name:
          <input type="text" name="name" value={formData.name} onChange={handleChange} />
        </label>
        <br />
        <label>
          Email:
          <input type="email" name="email" value={formData.email} onChange={handleChange} />
        </label>
        <br />
        <button type="submit">Submit</button>
      </form>
      <div>
        <strong>Submitted details:</strong>
        <p>Name: {formData.name}</p>
        <p>Email: {formData.email}</p>
      </div>
    </div>
  );
}

export default FormComponent;




Question Practice-----------------
Props -> 

1. Create a UserCard component that accepts props for name, email, and avatar
and displays them inside a card.

2. Build a parent component that holds a list of users (objects with name, email, and
avatar) and passes each user as a prop to the UserCard component to display.

3. Create a Button component that accepts props for text, color, and onClick
function. When clicked, the button should execute the onClick function passed in the
props.

useContext -> 

1. Create a theme toggler using useContext that allows users to switch between a
light and dark theme for the whole app. Pass the theme context to different components
and adjust styles accordingly.

2. Build a simple shopping cart where you can add and remove items. Use
useContext to manage the cart state and make it accessible to child components like
Cart and Product.

3. Implement a user authentication system using useContext. Create a
UserContext and show different content based on whether the user is logged in or not
(e.g., display login form or user profile).

useRef -> 

1. Basic useRef Usage

Write a React component that has an input field and a button. When the button is clicked, focus should move to the input field using useRef.

2. Persisting Values Without Re-render

Create a counter component where clicking a button increases the counter value, but the component should not re-render when the counter updates. Use useRef to store and update the counter.

3. Tracking Previous State Value

Build a React component that displays a number and a button. Every time the button is clicked, the current number is stored in a useRef variable, and the UI displays both the current and previous number.

4. Accessing DOM Elements Without Re-render

Create a React component with multiple input fields. Use useRef to store references to each input field and add a button that clears all input fields when clicked, without causing a re-render.