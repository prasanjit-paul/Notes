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