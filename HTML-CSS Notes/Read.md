Working Flow ->

These are used for frontend part ->>

1. HTML -> It is used for building satructure of a web page
2. CSS -> It is used to styling our web page.
    a. Bootstrap 
    b. Tailwind CSS
    c. MUI(Materialistic User Interface)
    d. Chakra UI
    from the above we have to learn Tailwind CSS for the responsiveness of the website and it now most used for the bilding of the website.
3. JavaScript -> It is used for building logics or functinality of a web page
    a. React JS(It's a frontend library)  -> Here we can modify the rule taking a partikular thing
        i. Next JS(It's a framework)  -> Here some certain Rule Are there 

Back-End -->>
4. Node JS(It's a Run-time Environment - tool) --->> its a tool for JS 
    a. Express JS (It's a framework of Node JS)

Database ->>
5. MongoDB (Un-Structured DB / non relational DB)
    a. Mongoose (It's Framework of Mongo DB)

-------------------------------------------------------------------------------------------
6. API (Application Programming Interface) ->> 
    - Used to make connection between frontend & backend

============================================================================================

HTML :-
    - Hyper Text Markup Language
    - It is used for building structrue of a web page
    - We called HTML as hyper text markup language because html creates a skeleton structrue of a web page
    - HTML works on the basis of tags
    - The main tag of html is <html>
    - Inside <html> tag we have our 2 important tag - <head> & <body>

Head tag :-
    - In head tag we have <title> tag for, give the website title in the title bar
    - In head tag we have some meta tags for holding responsiveness of the page & some other style sheet links

Body Tag :-
    - In body tag, we have all the elements in that tag

heading tag :- 

    - In html heading is a most important element.
    - there are 6 types of heading are there in html(h1 - h6)
    - <h1> is the bigger heading, <h6> is the small heading

Paragraph :-
    - paragraph is a most important element for showcasing our text in a web page
    - It is denoted by <p>

Break tag :-
    - It is used to break the line and starting a new line
    - It is denoted by <br>
    - It is a single tag

HR tag :-
    - It is used to create a horizontal line
    - It is denoted by <hr>
    - It is also a single tag

Image tag :-
    - When we put the image in our website we need <img> tag for inserting the image,
    - in <img> tag we have some attributes to showcasing our image in a proper form...
    - src -> for store the image link
    - alt -> for alternative text for a image
    - height -> for giving image height
    - width -> for giving image width
    - src,alt,height,width are the attributes of <img> tag
    <!-- FOR ONLINE PHOTO
    <img src="https://static.vecteezy.com/system/resources/thumbnails/021/746/785/small/holding-a-tree-in-a-ball-ecology-and-environment-concept-with-generative-ai-photo.jpg"
        alt="image"> -->

    <!-- FOR OFFLINE PHOTO IN SAME FOLDER  We use ./  and access  -->
    <img src="./image1.jpg" alt="image1"> 

    <!-- FOR OFFLINE PHOTO IN OTHER FOLDER  We use ../ and access -->
    <img src="../image2.jpg" alt="image2">


Text Formating :-
    - We use html formatting for properlly format our text inside paragraph or heading
    - There are 10 types of html formatting tag are there :
    1.    <i>Italic Tag</i>
    2.    <b>Bold Tag</b>
    3.    <small>Small Tag</small>
    4.    <strong>Strong Tag</strong>
    5.    <em>Emphasise</em>
    6.    <ins>Inseted Text - Underline</ins>
    7.    <del>Delete Tag</del>
    8.    <mark>Mark tag</mark>
    9.    <sup>Superscript</sup>
    10.   <sub>Subscript</sub>
    
Ancher Tag:- 
    FOR link clicked to the ANOTHER Page
    <a href="https://www.geeksforgeeks.org/" target="_blank">Click me</a>

    FOR link clicked to the SAME Page
    <a href="https://www.geeksforgeeks.org/" target="_self">Click me</a>

HTML Table:-
    - As per the normal table we have a table like structure in html
    - in HTML, Our table is row wise structure
    - The main tag of html is <table>
    - In the table we have 
        <td> -> table data
        <tr> -> table row
        <th> -> table heading
        
        Ex:- 

    sl.     name      designation       salary
    1	    rishi	    HR	            12000
    2   	ridhi	    Manager	        20000
    3	    Ram	        Developer   	34000


HTML List:-
    - We used html list for storing data in a sequential data
    - Basically list are 3 types:- 
        1. Ordered List ( <ol> for storing data - <li> -> list item)
        2. Unordered List ( <ul> for storing data - <li> -> list item)
        3. Description List ( <dl>for storing data - <dd> -> description data, <dt> -> descriptionn Term)


HTML Form:-
    - In HTML we have a form like structure to create in web page
    - The main tag of html form is  <form>
    - Inside the <form> tag we have 2 more field like labels fields & input fields

    - Input Types
<input type="button">
<input type="checkbox">For selecting multiple options from a group.
<input type="radio">For selecting one option from a group.
<input type="color">
<input type="date">
<input type="datetime-local">
<input type="email">
<input type="file">
<input type="hidden">
<input type="image">
<input type="month">
<input type="number">
<input type="password"> For entering passwords; the input is masked
<input type="search">
<input type="range">
<input type="reset">Creates a button to reset the form fields.
<input type="submit">Creates a button to submit the form data.
<input type="tel">
<input type="text">For single-line text input.
<input type="time">
<input type="url">
<input type="week">


HTML Block Structure element:- 
    - We have some html block level element for separate the block in different part.
    - Ex:- <address>    <article>   <aside> <blockquote>    <canvas>    <dd>    <div>   <dl>    <dt>    <fieldset>  <figcaption>    <figure>    <footer>    <form>  <h1>-<h6>   <header>    <hr>    <li>    <main>  <nav>   <noscript>  <ol>    <p> <pre>   <section>   <table> <tfoot> <ul>    <video>

HTML inline element:-
 
 -we have our html element for structuring our inline text.
 -it means there will be no specific width in that element, it is situated inside a block levle element.
 -ex.<span>

CSS :-
    - we can use CSS for the propose of designing & styleing our web page.

-Syntax :- 

    h1{
     color:red;
    }
    - in this above code h1 is the selector, color is the property & red is the value of that porporty.
 - there are three types of CSS are present..

1. inline CSS :-
- we used inline CSS inside a tag.
- inline CSS is heighest peiority by compair with other types of css.
- we can put our styling by creating a "style" attribute inside the tag.

2. internal CSS :-
- we us internal CSS inside head tag, by creating a <style> tag inside it.
- internal CSS use many cases for small codebase.

3. External CSS :-
- we used external CSS by creating a separate CSS file and link that in our html page.
- we can link the external cSS file by <link> tag.
- it is most popularlly used because everyon wants to see clean code so all files have to be separated.

Selector in CSS :- 

- we used selector for selecting an html element for the shake of desighing.
- there are 5 types of css selector are there.

1. ID selector :-
- id selector is a type of selector that used for unique design.
- it is denoted by the symbol "#".

2. class selector :-
- class selector is a type of selector that used for similar design in multiple elements.
- class selector is denoted by the symbol "."

3. Group selector :-
- group selector is a type of selector that can used to design more then one element by creating a group.
 
4. Universal selector :-
- Universal selector is a type of selector where we can design whole html element by single styling.
- it is denoted by the symbol "*"

5. Element selector :-
-  element selector is a type of selector where we can design one by one element by tag wise.


Text Properties:-
    - text-align: left/right/center
    - text-decoration: overline/underline/line-through
    - font-weight: 100 - 900
    - font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif   -> we have multiple font family
    - line-height: normal/2px/3
    - text-transform: capitalize/uppercase/lowercase/normal
    - font-size: 10px

Units in CSS:-
    96px = 1 inch

Question Practice:-
    1. Crreate a heading centered on the page with all of its text capitalized by default
    2. Set the font family of all the content in the document to "Times New Roman"
    3. Create one div inside another div Set the outer div text size to 25px  & inner text size to 10px
    4. Create a simple div with an ID box. Add some text content inside the div Set its background color to blue
    5. Create 3 heading with h1,h2 and h3 Give them all a class "heading and set color

Properties in CSS:-
There are lots of properties are there in css
    - color:
    - background-color:
    - text-line:
    - text-decoration:
    - font-family:
    - font-weight:
    - line-height:
    - text-transform:

Box Model in CSS:-
    - Box model is used for properlly placed the element in right direction.
    - It major all the size of that particular of that element and place them into a right place
    - There are 5 types of box-model element are there
        1. Height
        2. Width
        3. Padding -  Padding-left, Padding-right, Padding-top, Padding-buttom 
        4. Border -(Border-radius)
        5. Margin -  Margin-left, Margin-right, Margin-top, Margin-buttom


display properties in CSS:-
    - We use display properties to showcase our elemrnt in proper form to display.
    - Basically we have 4 type of properties are present....
        1. display-inline ---->it takes only the space required by the element
        2. display-block ----->it takes full space available iin width
        3. display-inline-block ----> similar to inline but we can put padding & margin here
        4. display-none  ----> nothing(remove element from the document flow)


Flex-Box in CSS:-
    - We can use css flex-box to create 1D designs in  single page
    - flex box have some properties like  
        1. Display: flex;
        2. flex-direction : row / row-reverse / column-column / reverse
        3. justify-content: center /start /end / space-evenlly / space-between / space-around
        4. align-items:  center/top/buttomm;
        5. flex-wrap: wrap/no wrap;
        6. Gap

Question Practice:-
 1. Create a navbar with 4 options in the form of anchor tag inside list items. Now use flexbox to place them all spaced eually in a single line.
 2. Use flexbox to center one div inside another div.
 3. Which has higher Property-align items or align- self?


Transform Property:-
    - It helps us to transform an element from one form to another form.
    1. Rotate:-
        it ortates an element in terms of degree.
    2. Skew :-
        It distort each point of an element by a certain angle in horizontal or vertical directions.
            Horizontal ----> SkewX()
            Vertical ------> SkewY()
    3. Scale :-
        It allows us to resize an element
        Scale > 1 will increase the size and scale < 1 will decrease the size of an element
    4. Translate :-
        - It allows us to transfer an element from one place to another along the X-axis and the Y-axis.
        - Translate values will be given in pixel
    5. Transition :-
        It helps us to change the property values smoothly or a given direction of time.

Position Proerties:-
    - We will use Position property to place the element in proper position.
    - There are 5 types of position proporty 
    1. Static --> Default position(The top, bottom,left,right properties are no effect)

    2. Relative --> Element is relative to it self(The top, bottom,left,right properties will work)

    3. Absolute ---> position relative to its closest ancester (remove from the document flow)(The top, bottom,left,right properties will work)

    4. Fixed --> Position relative to its browser (remove from the document flow )(The top, bottom,left,right properties will work)
    
    5. Sticky --> position based on user's scroll position.(The top, bottom,left,right properties will work)

Animation in CSS :-

    @keyframe myName{
        from{ Font-size: 20px; }
        to{ Font-size: 40px; }
    }

    Animation properties:-
        - animation-name
        - animation-duration
        - animation-timing-function
        - animation-delay
        - animation-iteration-count
        - animation-direction
        

    Transition -->  to change the state 
        - transition enable to define the transition between two state.
        - Some important transition properties are :-
            1. transition: all
            2. transition-delay: 3s etc
            3. transition-duration: 3s etc
            4. transition-timing-function: step(2/3/4 etc), ease-in, ease-out, ease-in-out

    Transform --> transform the position
        - Used to apply 2D & 3D transformation to an element.
            1. transform: rotate --> rotate(45deg), rotateX(45deg), rotateY(45deg), rotateZ(45deg)
            2. transform: scale --> scale(2), scaleX(2), scaleY(2)
            3. transform: skew --> skew(45deg), skewX(45deg), skewY(45deg)

    Media-Query --> 
        - Create a responnsive website in today's world everyone has a different device with thousands of of different screen sizes.
        - If you  built a website people will use it on laptop, big screen computers, an iphone, a big screen andrion phone or small screen one, an ipad
        - Even orientation is different like landscape or portrait so its important that layout looks good on also we need design to be reponsive, respond to different screen size or orientation.

            Syntax:- 

                media not only type and (media feature) and (media feature)
                {
                    css-code
                }

            example:-

                @media(width:600px){
                    div{
                        background-color: red;
                    }
                }
                @media(min-width:600px){
                    div{
                        background-color: red;
                    }
                }
                @media(max-width:600px){
                    div{
                        background-color: red;
                    }
                }
                @media(max-width:600px)and (max-width:800px) {
                    div{
                        background-color: red;
                    }
                }

Grid in CSS:-
    - CSS Grid is a 2D layout system gor the web.
    - A gid is a collection of horizontal and vertical lines creating a patterns against which we can line up our design element
    - They helps us to create designs where element don't jump around or change width as we move from page to page
    - Some important properties of grid layout :-
        1. display: grid;
        2. grid-template-colomn: repate(4.1f)/3 4 5;
        3. gid-gap: 20px;
        4. grid-auto-rows: 100px;
        5. grid-lines: 

Q1:Create a webpage layout with a header, a footer & a content area containing 3 divs.
    Set the height & width of divs to 100px.
    (add the previous navbar in the header)
Q2: Add borders to all the divs.
Q3: Add a different background color to each div with an opacity of 0.5
Q4: Give the content area an appropriate height.
Q5. Give the div a height, width and some background image.
Q6. Use the appropriate position property for the div element to place it at the right end of the page. (The div should not move on scroll).
Q7. Create a navbar with 4 options in the form of anchor tags inside list items.Now, use flexbox to place them all spaced equally in a single line.
Q8. Use flexbox to center one div inside another div.
Q9. Which has higher priority - align-items or align-self?
Q10. Create a simple loader using Css 

Step1: Create a div width circular shape & a thick border from one end (top/bottom/left).
Step2: To make it spin create an animation which transforms it forms 0deg to 360deg.
Step3: Add the animation to the loader with infinite duration.


Table properties:-
