
 
 # HTML
- ### What Is HTML ?
  - HTML stands for hyper text markup language .
  - HTML is the code that is used to structure a web page and its content.
  - The component used to design the structure of websites are called HTML tags.

- ### First HTML File
  - index.html
  - It is the default name for a website's homepage. 

- ### HTML Tags
     One of the main parts of HTML is HTML tags – HTML tags are like keywords that define how a web browser will format and display content.
           
     A container for some content or other HTML tags.
           
          < !DOCTYPE html> -> is a tag used to tell the browser the version of html that you are using.
         
          < html>                   -> root of an html document
          < head>                 -> container for metadata 
          < title>My First Page</title>     -> page Title
          < /head> 
          < body>        -> contains all data rendered by the browser 
          < p>hello world</p>      -> paragraph tag 
          < /body> 
          < /html>

     
     <strong>< !DOCTYPE html ></string> is a tag used to tell the browser the version of html that you are using.
     
   HTML tags contain three main parts:
     - opening tag
     - content
     - closing tag
     
   Opening tag
     - Begins the section of a page
     - All opening tags are enclosed in <>
     
   Content
     - The matter written in between the opening and closing tags.
     - <> content </>.
     
   Closing tag
     - It ends the section of a page.
     - All closing tags are enclosed with, </>.
     
   Most HTML tags are paired tags, very few tags are unpaired. 


- ### Paired tags
   <strong>Paired tags</strong> have both opening and closing tags.
          
   Example:
          
          <html>  </html>
          <p> </p>
          <b> </b>

- ### Unpaired tags  
          
     <strong>Unpaired tags</strong> have no ending or closing tags.
          
      Example:
          
          <br>
          <hr>
          <img>
 
- ### HTML Basic ElementsHTML tags case sensitive ?

     All the HTML elements/tags are case-insensitive. Case-insensitive means the tags/elements which are used in the code are understandable by the browser irrespective of the letters being the upper case or lower case classes.
          
      Example:
          
          <!DOCTYPE html>
          <html>
          <body>
               <h2>Welcome To AD</h2>
               <p>AppsDeployer</p>
               <p>The code has lowercase body tags</p>
          </body>
          </html>
          
- ### Anchor Tag
          
Used to add links to your page.
          
    < a href="https://google.com"> Google </a>

- ### Image Tag
Used to add images to your page
          
    < img src="/image.png" alt="Random Image">
          
- ### Br Tag
          
Used to add next line(line breaks) to your page
          
    < br>
          
- ### Bold, Italic & Underline Tags
Used to highlight text in your page 
          
    <b> Bold </b> 
    <i> Italic </i> 
    <u> Underline </u>
          
- ### Big & Small Tags
Used to display big & small text on your page
          
    <big> Big </big>
    <small> Small </small>

- ### Hr Tag
Used to display a horizontal ruler, used to separate content
          
    < hr>
          
- ### iframe Tag
website inside website
          
    < iframe src="link"> Link </option>



- ### Video Tag

    < video src="myVid.mp4">	My Video </video>

Attributes

-controls
-height
-width
-loop
-autoplay



- ### HTML Basic Elements
          
     The basic elements of an HTML page are: 
          
     A text header, denoted using the <strong>< h1>, < h2>, < h3>, < h4>, < h5>, < h6> tags.</strong>
          
     A paragraph, denoted using the <strong>< p></strong> tag.
          
     A horizontal ruler, denoted using the <strong>< hr></strong> tag.
          
     A link, denoted using the <strong>< a></strong> (anchor) tag.
          
     A list, denoted using the <strong>< ul></strong> (unordered list), <strong>< ol></strong> (ordered list) and <strong>< li></strong> (list element) tags.
          
     An image, denoted using the <strong>< img></strong> tag.
          
     A divider, denoted using the <strong>< div></strong> tag.
          
     A text span, denoted using the <strong>< span></strong> tag.
         
 - ### Lists
     HTML provides a way to create both an 
1. <strong>ordered list</strong> (with elements counting up, 1, 2, 3...) and an 
2. <strong>unordered list</strong> with bullets instead of numbers.

 - ### Images
     To add an image, use the <strong>< img></strong> tag along with the <strong>src</strong> attribute to specify the location of the image.
          
     Example:  
          
       <img src="img/code.jpg">
   
- ### Comment in html     
     The comment tag is used to insert comments in the source code. Comments are not displayed in the browsers.
          
       <!--This is a comment. Comments are not displayed in the browser-->
     
- ### HTML Attributes
     HTML attributes are the special words placed inside the opening tags and used to define the characteristics of an HTML element. 
        
       <html lang="en">
          
     The four core attributes that can be used on the majority of HTML elements
          
     <strong>Id =><strong> The id attribute of an HTML tag can be used to uniquely identify any element within an HTML page.
           
     <strong>Title =><strong> The title attribute gives a suggested title for the element.
           
     <strong>Class =><strong> The class attribute is used to associate an element with a style sheet, and specifies the class of element. 
           
     <strong>Style =><strong> The style attribute allows you to specify Cascading Style Sheet (CSS) rules within the element.
   
- ### HTML Table     
     HTML table tag is used to display data in tabular form (row * column). There can be many columns in a row. 
     - #### HTML Table Tags 
       < table>=> It defines a table.
            
       < tr>=> used to display table row
            
       < th>=> used to display table header
            
       < td>=> used to display table data
            
       < caption>=> It defines the table caption.
            
       < colgroup>=> It specifies a group of one or more columns in a table for formatting.
            
       < col>=> It is used with <colgroup> element to specify column properties for each column.
            
       < tbody>=> to wrap table body
            
       < thead>	 => to wrap table head
            
       < tfooter>	=> It is used to group the footer content in a table.

- ### HTML Form
     An HTML form is a section of a document which contains controls such as text fields, password fields, checkboxes, radio buttons, submit button, menus etc.
            
       <form>
       form content
       </form>

     <strong>Why use HTML Form</strong>
            
     HTML forms are required if you want to collect some data from of the site visitor.
     HTML Form Syntax
            
       < form action="server url" method="get|post">  
       //input controls e.g. textfield, textarea, radiobutton, button  
       < /form>  

- ### HTML Form Tags
     < form>         =>     It defines an HTML form to enter inputs by the used side.
          
     < input>        =>     It defines an input control.
          
     < textarea>     =>     It defines a multi-line input control.
          
     < label>        =>     It defines a label for an input element.
          
     < fieldset>     =>   It groups the related element in a form.
          
     < legend>       =>   It defines a caption for a < fieldset> element.
          
     < select>       =>   It defines a drop-down list.
          
     < optgroup>	 =>  It defines a group of related options in a drop-down list.
          
     < option>	      =>  It defines an option in a drop-down list.
          
     < button>	      =>  It defines a clickable button.
          
- ### Action in Form
Action attribute is used to define what action needs to be
performed when a form is submitted 

     <form action="/action.php" > 

- Form Element : 
Input
     <input type="text" placeholder="Enter Name">
 
-Label
          
     <label for="id1">
     <input type="radio" value="class X" name="class" id="id1">
     </label>

     <label for="id2">
     <input type="radio" value="class X" name="class” id="id2">
     </label>

- ### Page Layout Techniques
     using Semantic tags for layout using the Right Tags 

       <header>
       <main>
       <footer> 

     Inside Main Tag 

     Section Tag   -> For a section on your page

       <section>

     Article Tag  -> For an article on your page

       <article> 

     Aside Tag  -> For content aside main content(ads)

       <aside>

- ### Div Tag

     Div is a container used for other HTML elements 
     Block Element (takes full width) 


# CSS - (Cascading Style Sheets)
            
CSS (Cascading Style Sheets) allows you to create great-looking web pages.
            
It provides an additional feature to HTML. It is generally used with HTML to change the style of web pages and user interfaces.

CSS syntax

       h1 {
       color: red;
       font-size: 5em;
       }
__
            
- There are 3 ways to add CSS to HTML:
            
     1.<style> tag : Adding <style> … </style> to HTML
     
     2.Inline CSS : Adding CSS using style attribute
            -> An inline style will override external and internal styles
            
     3.External CSS : Adding a stylesheet(.css) to HTML using <link> tag.

     - HTML id  attributes
     When an HTML element is given an id, it serves as a unique identifier for that element.

     - HTML class attributes
     HTML element is given a class, it now belongs to that class. More than one element can belong to a single class 

     Example:

       <div id = ‘first’ class = ‘C1 C2 C3’>
       …
       </div>


- CSS selectors
CSS selectors define the pattern to select elements to which a set of CSS rules are then applied.

- Universal selectors
The CSS universal selector (*) matches elements of any type.

example :
            
       * {
       color: green;
       margin: 0;
       padding: 0;
       }

- Id Selector
It is used to select an element with a given id
            
Syntax:    `#idname`

example: 
            
       #first {
       color: white;
       background: black;
       }
                               
‘#’ is used to target by id

- Class Selector
It is used to select an element with a given class.
            
Syntax:  `.classname`

example:

       .red {
       background: red;
       }


- Type selectors
The CSS type selector matches elements by node name. In other words, it selects all elements of the given type within a document.
            
Syntax:   `element { style properties }`
            
example:

       a {
       color: red;
       }

- Group selectors
When multiple selectors share the same declarations, they can be grouped together into a comma-separated list.
            
example:

       h1,h2,h3,div {
       color:blue;
       }

- color property
The CSS color property can be used to set the text color inside an element

       p{
       color: red;       /*Text color will be changed to red*/
       }

- background-color property
The CSS background-color property specifies the background color of a container.
            
example:
            
       .brown {
       background-color: brown;
       }

The background-image property
Used to set an image as the background

       body {
       background-image: url(“image.jpg”)
       }
       /*The image is by default repeated in X & Y directions*/

- background-repeat property 
     - repeat-x : => repeat in the horizontal direction
     - repeat-y :  => repeat in the vertical direction
     - no-repeat : =>  image not repeat 

- background-size property
     - cover :  => fits & no empty space remains
     - contain :  => fits & image is fully visible
     - auto :  => display in original size
     - {{width}} : =>  set width & height will be set automatically
     - {{width}} {{height}} :  => set width & height

- background-position property
Sets the starting position of a background image

       .div1{
       background-position: left top;
       }

- background-attachment property
Defines a scrollable/non-scrollable character of a background image

       .div2{
       background-attachment: fixed
       }

- background shorthand
A single property to set multiple background properties

       .div3{
       background: red url(‘img.png’) no-repeat fixed right top;
       } 

- display property
The CSS display property is used to determine whether an element is treated as a block/inline element & the layout used for its children (flexbox/grid/etc.)

- display: `inline`
Takes only the space required by the element. No line breaks before and after. Setting width/height (or margin/padding) not allowed.

- display: `block`
Takes full space available in width and leaves a newline before and after the element

- display: `inline-block`
Similar to inline but setting height, width, margin, and padding is allowed. Elements can sit next to each other

- display: `none`
With display: none, the element is removed from the document flow. Its space is not blocked.

- visibility: `hidden`
With visibility: hidden, the element is hidden but its space is reserved.

- text-align property
Used to set the horizontal alignment of a text

       .div1{
       text-align: center;
       }

- text-decoration property Used to decorate the text
> Can be overline, line-through, underline, none

- text-transform property
Used to specify uppercase and lowercase letters in a text

       p.uppercase{
       text-transform: uppercase;
       }

- line-height property
Used to specify the space between lines

       .Small{
       line-height: 0.7;
       }

- Font
Font plays a very important role in the look and feel of a website

`Font-family : =>Font family specifies the font of a text.`

       p{
       font-family: “Times new Roman”, monospace;
       } 

- Other Font Properties 
     - `font-size`: Sets the size of the font
     - `font-style`: Sets the font style
     - `font-variant`: Sets whether the text is displayed in small-caps
     - `font-weight`: sets the weight of the font

- How to add Google Fonts 
     - In order to use custom google fonts, 
     - go to google fonts then select a style, 
     - and finally paste it to the style.css of your page.

- What’s wrong with pixels?
     - Pixels (px) are relative to the viewing device.
     - For a device with the size 1920x1080, 1px is 1unit out of 1080/1920.

- Relative lengths
     - These units are relative to the other length property. 
     - 4.	em – unit relative to the parent font size
     - 5.	em means “my parent element’s font-size”
     - 6.	rem – unit relative to the root font size (<html> tag)
     - 7.	vw – unit relative to 1% viewport width
     - 8.	vh – unit relative to 1% viewport height
     - 9.	% - unit relative to the parent element

-Min/max- height/width property
     - CSS has a min-height, max-height, and min-width, max-width property.
     - If the content is smaller than the minimum height, minimum height will be applied

- position property 
Used to manipulate the location of an element  
     - `static`: The default position. top/bottom/left/right/z-index has no effect
     - `relative` : The top/bottom/left/right/z-index will now work. Otherwise, the element is in the flow of the document like static.
     - `absolute`: The element is removed from the flow and is relatively positioned to its first non-static ancestor. top/bottom etc. works
     - `fixed`: Just like absolute except the element is positioned relative to the browser window
     - `sticky`: The element is positioned based on the user’s scroll position

- list-style property
The list-style property is a shorthand for type, position, and image 
            
       ul{
       list-style: square inside url(‘image.jpg’)
       }
            
- '# square’ in the above code is the list-style-type, ‘inside’ is the list-style-position and ‘image.jpg’ is the list-style-image. 

- z-index property 
     - The z-index property specifies the stack order of an element.
     - It defines which layer will be above which in case of overlapping elements.
            
- float property
     - float property is simple. It just flows the element towards left/right 

- CSS Flexbox
Aims at providing a better way to layout, align, and distribute space among items in a container.
            
       .container{
       display: flex;                  /*Initialize a flexbox*/
       }

- flex-direction property 
Defines the direction towards which items are laid.
Can be row (default), row-reverse, column and column-reverse  

- Flex properties for parent (flex container) 
     - `flex-wrap`: Can be wrap, nowrap, wrap-reverse. Wrap items as needed with this property
     - `justify-content`: Defines alignment along the main axis
     - ``align-items`: Defines alignment along the cross axis
     - align-content`: Aligns a flex container’s lines when there is extra space in the cross axis 

- Flex properties for the children (flex items) 
     - `order`: Controls the order in which the items appear in the flex container.
     - `align-self`: Allows default alignment to be overridden for the individual flex items.
     - `flex-grow`: Defines the ability for a flex item to grow.
     - `flex-shrink`: Specifies how much a flex item will shrink relative to the rest of the flex items.

- CSS grid can be initialized using:

       .container {
       display: grid;
       }
            
All direct children automatically become grid items

- grid-column-gap property
Used to adjust the space between the columns of a CSS grid
 
- grid-row-gap property
Used to adjust the space between the rows of a CSS grid

- grid-gap property
Shorthand property for grid-row-gap & grid-column-gap 

       .container {
       display: grid;
       grid-gap: 40px 100px;            /*40px for row and 100px for column*/
       }
        /* For a single value of grid-gap, both row and column gaps can be set in one value.*/

- Following are the properties for grid container: 
The grid-template-columns property can be used to specify the width of columns

        .container {
        display: grid;
        grid-template-columns: 80px 120px auto;
        }
            
The grid-template-rows property can be used to specify the height of each row

        .container {
        display: grid;
        grid-template-rows: 70px 150px;
        }
            
The justify-content property is used to align the whole grid inside the container.
The align-content property is used to vertically align the whole grid inside the container.

- Transforms are used to rotate, move, skew or scale elements. They are used to create a 3-D effect.

- transform property  
Used to apply a 2-D or 3-D transformation to an element

- The transform-origin property
     Allows to change the position of transformed elements
     2D transforms – can change x & y-axis
     3D transforms – can change Z-axis as well

- CSS 2D transform methods
            
translate()
            
rotate()
            
scaleX()
            
scaleY()
            
skew()
            
matrix()
            
scale()
 
- CSS 3D transform methods
rotateX()
            
rotateY()
            
rotateZ()


- CSS Transitions
Used to change property values smoothly, over a given duration.
            
transition property 
            
`transition-property`: The property you want to transition
            
`transition-duration`: Time for which you want the transition to apply
            
`transition-timing-function`: How you want the property to transition
            
`transition-delay`: Specifies the delay for the transition 

            
- Syntax:      transition: property duration timing-function delay;
                    transition: width 35 ease-in 25;
 
Transitioning multiple properties 
transition: opacity 15 ease-out 15, transform 25 ease-in;

- CSS Animations
Used to animate CSS properties with more control.
We can use the @keyframes rule to change the animation from a given style to a new style.

        @keyframes text{
        from { width: 20px; }              /*Can change multiple properties*/
        to { width: 31px; }
        } 

- Properties to add Animations 
`animation-name`: name of the animation
            
`animation-duration`: how long does the animation run?
            
`animation-timing-function`: determines speed curve of the animation
            
`animation-delay`: delay for the start of an animation
            
`animation-iteration-count`: number of times an animation should run
            
`animation-direction`: specifies the direction of the animation
 
- Animation  
            
All the animation properties from 1-6 can be applied like this 
            
animation: text 65 linear 15 infinite reverse; 

Using percentage value states with animation 
            
We can use % values to indicate what should happen when a certain percent of animation is completed 
            
        @keyframes text{
        0% {
        width: 20px;
        }
        50% {
        width: 80px;
        }
        100% {
        width: 200px;
        }
        }
   
