useState:- 
    - The react useState hooks allows us to track state in a functional component.
    - state is basically refers to data or properties that need to be traking in an application
    - to use useStaate, first we import it into our component or files.
    Ex:-   
    import useState fom "react;

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







import React, { useEffect, useState } from "react";

const Photos = () => {
  const [photos, setUsers] = useState([]);
  const [currentPage, setCurrentPage] = useState(1);
  const postsPerPage = 8;

  const getUsers = async () => {
    const response = await fetch("https://dummyjson.com/products");
    const data = await response.json();
    setUsers(data.products);
    console.log(data);
  };
  useEffect(() => {
    getUsers();
  }, []);

  const indexOfLastPost = currentPage * postsPerPage;
  const indexOfFirstPost = indexOfLastPost - postsPerPage;
  const currentPosts = photos.slice(indexOfFirstPost, indexOfLastPost);

  const totalPages = Math.ceil(photos.length / postsPerPage);

  const handleNextPage = () => {
    if (currentPage < totalPages) {
      setCurrentPage(currentPage + 1);
    }
  };

  const handlePrevPage = () => {
    if (currentPage > 1) {
      setCurrentPage(currentPage - 1);
    }
  };

  return (
    <div>
      <h1>Product Detels</h1>
      <ul>
        {currentPosts.map((item) => {
          return (
            <div className="box">
              <img src={item.images[0]} alt="img" height={100} width={100} />
              <h4 className="item">Price:{item.price} $</h4>
              <h2 className="item">Title: {item.title}</h2>
              <h3 className="item" id="des">
                Description: {item.description}
              </h3>
            </div>
          );
        })}
      </ul>
      <div>
        <button onClick={handlePrevPage}>Previous</button>
        <button onClick={handleNextPage}>Next</button>
      </div>
    </div>
  );
};

export default Photos;








# Reference in react :
- it is inbuilt object in react.
- it is used to target element in react .
- By the default it will be having key value pair of "current : undefined".
- ref will always uses Real dom.
- IN the functional component , we have to use useRef() hook to creat reference.
- e.g : const inputRef = useRef()

Ex:-
import React, { useRef } from 'react'

const Raference = () => {
    const reference=useRef()

    const handelClick=()=>{
        reference.current.style.color="blue"
        reference.current.style.backgroundColor="red"
        reference.current.style.marginButton="60px"


    }
  return (
    <div style={{textAlign:"center"}}>
       <h1 ref={reference}>Reference</h1>
       <button onClick={handelClick}>click me!</button>
    </div>
  )
}

export default Raference


# From Handling in React :
 1. Uncontrolled Froms 
 2. Controlled Froms

 ## Uncontrolled Froms 
 - It is a from where it is created using reference concept.
 - In functional component , we have to use useRef () hook to creat uncontroled from.
 - these froms are completely handeled by DOM it self.
 - Suppose if we have to take input from user , first the data will be taken by DOM and then we will be taking data from DOM .

 Example :-
 import React, { useRef } from 'react';

const UnControlledForm = () => {
  const nameRef = useRef();
  const emailRef = useRef();

  const handleSubmit = (e) => {
    e.preventDefault();

    console.log(nameRef.current.value);
    console.log(emailRef.current.value);

    
    nameRef.current.value = "";
    emailRef.current.value = "";
  };

  return (
    <div>
      <form className='container' >
        <label>Name:</label>
        <input type="text" ref={nameRef} />
        <label>Email:</label>
        <input type="text" ref={emailRef} /> <br />
        <button type="submit" onClick={handleSubmit}>Submit</button>
      </form>
    </div>
  );
};

export default UnControlledForm;




## Controled from

- these from are created using state in react .
- In functional component we use useState() to create controled froms.
- These froms are completly handeled by developers where we will be taking the data from the user by using "onChange" event.

example :-
import React, { useState } from 'react'

const   ControlledForm = () => {
    const [name,setName]=useState("")
    const [email,setEmail]=useState("")

    const getName=(e)=>{
       setName(e.target.value)  
    }

    const getEmail=(e)=>{
        setEmail(e.target.value)
     }

     const handelSubmit=(e)=>{
        e.preventDefault(); 
        console.log(name);
        console.log(email);
        
        
        setEmail("")
        setName("")
        
     }

  return (
    <div>
        <form className='conatiner'>
            <label> Name :</label>
            <input type="text" value={name}  onChange={getName}/>
            <label> Email :</label>
            <input type="text" value={email} onChange={getEmail} /> <br />
            <button onClick={handelSubmit}>Submit</button>
        </form>
    </div>
  )
}

export default ControlledForm


# useContext
- Context is a way to share data between components without having to pass props down the component tree.
- useContext() is a hook that allows you to consume context value in your foctional component.
- To creat a context , use the creatContext() method . This return a context object that can be used to provide and consume value .
- To provide value to a child component , use the "context.Provider" component . This component accepts a value prop that is passed down to chiled components.

- To consume a value in child component , use the UseContext() hook . This hooks takes a context object as its argument and return the current value of the context.

- WE can use multiple context values in a single component by nesting context.provider components.
- Overuse of context can make our code harder to understand and maintain .