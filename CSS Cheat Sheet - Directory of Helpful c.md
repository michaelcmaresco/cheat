CSS Cheat Sheet - Directory of Helpful commands





CSS Syntax is important for giving us different style for a used on a given HTML page.





Module 1:

EXAMPLE:

body{
    color: #39a6b2;
    font-family: Helvetica, Arial, sand-serif;
}

1. body : Selector
2. font-family: :Property name
3. Helvetica, Arial : Property Value
4. ; : Declaration terminator
5. sans-serif; : Declaration


        1. Selector: This is the part that says "let's find this matching HTML element (in this case, the "body" element) so 
        we can tell it what it should look like
        - This is the most basic of selectors where we select the HTML by name. 
            - we COULD use a CSS selector to be vague and apply all <a> elements 
                                        OR
            - we COULD use a CSS selector to specifically target <a> elements in a <header> and to ignore others that aren't. 

        2. Property name: CSS has an extensive list of possible style properties. 
            - All we need to do is list one between the selectors {}
                - now we can change how this element looks. 
                    - EXAMPLE : a popular one is "color, background-iamge and font-family" 
                        - If we use one that isn't predefined, then the browser will ignore the style. 

        3. Property Value: Where we get to provide a desired look to an element.
            - EXAMPLE: we can provide a value of "#39a6b2" to the color property
            - EXAMPLE: we can provide "font-size: 3meters" it WOULDN'T BE UNDERSTOOD AND APPLIED.
                WE WOULD HAVE TO SAY "font-size: 24px;" because CSS can understand "24px" as a size. 

        4. Declaration: a property: property-value pairing like we see with "font-family": Helvetica is what's known as a declaration.

        5. Declaration Terminator: ;, whenever CSS see's this semicolon, it says that this style is done and to stop it right then and there. 
            - Everything after that is apart of a different declaration. 
                -It's extremely important to terminate your declarations. 
        
        6. CSS Rule : The entire block shown in the preceding image. 
            - It is a combination of the selector and all of the declarations. 

        7. <link rel="stylesheet" href="./assets/css/style.css" /> : Link a CSS sheet to an HTML page

        8. header h1 {

        }
            - This ensures we are only effecting the <h1> parts that are within the header element.

        9. header nav ul li {

        }
            - This effects all of the nav elements (ul, li, and ol)

        10. header nav ul li a{

        }
            - This effects all of the nav elements associated with all the anchored elements. 

        11. *{

        }
            - This tells every element on the page to not have any margin or border unless we explicitly tell it to. 

        12. * : this is the Universal selector in CSS. 

        13. line-height : how much vertical space should be between lines of text content. 
            EXAMPLE: 1.5 = we want the spacing to be 1.5 times the size of the font. 
                - 1.5 is a good baseline. 

        14. box-sizing : content-size : calculates the height and width of the element by only counting the content box of the CSS box model. 

        15. box-sizing : border-box : calculates the height and width of the element by including the border and padding addition to the content box. 

        16. images : insert image into style.

        17. background-image: url("../images/hero-bg.jpg);

        18. class : **atribute** 
            EXAMPLE: <section class="hero">

        19. background-position: initial position of the background image.
            EXAMPLE: background-position: center;
        
        20.  background-color: property sets background color to the element selected

        21. padding : property that creates an inner margin within the border. 

            .title-name {
                padding: 20px;
            ...

        22. border-style: Different type of border.
            EXAMPLE: 

            .title-name {
            ...border-style: solid;
            }

        23. border-width: width of border
            EXAMPLE: 

            .title-name {
            ...
            border-width: 3px;
            }

        24. color: #024e76
            EXAMPLE:
            .title-name {
            ...
            color: #024e76;
            }

        25. border: solid 3px #024e76;
            EXAMPLE:
            .text-name {
            ...
            border: solid 3px #024e76;
            }

        26. ... : syntax placeholder, this assumes there is other content here. 

        27. static : is the default value and maintains the order of the natural flow of the elements on the page/ 
            EXAMPLE: order created in the HTML.
                - The static positioning isn't affected by the top, bottom, left and right properties. 

        28. relative : a form of positioning that uses the "top" and "bottom" properties to vertically offset the "left" and "right" properties to horizontally offset the element from the "static" position. 

        29. absolute : a form of positioning that removes the element from the natural flow of the page elements and uses the top, bottom, left and right. 

        EXAMPLE:
        - Enabling absolute positioning of the form container to be taken relative to the hero section, we need to make the hero's section's position "relative" . To do this, go to the CSS rule for the hero and add a declaration that sets the position to "relative". This is how the CSS should look. 

        /* Hero Style Start */
        .hero {
        background-image: url("../images/hero-bg.jpg");
        height: 600px;
        background-size: cover;
        background-position: center;
        position: relative;
        }
        /* Hero Style End */

        30. fixed : a form of positioning that removes the element from the natural flow of the page elements and positions it relative to the viewport or browser window so that it isn't affected by scrolling. 
            - The "fixed" position value uses the "top", "bottom", "left"  and "right" properties to offset the element from the viewport's margins. 

        28,29 and 30 Code example
        EXAMPLE: 

        .hero-form {
        border: 3px solid #024e76;
        background-color: #fce138;
        padding: 20px;
        width: 500px;
        color: #024e76;
        position: absolute;
        bottom: 0px;
        right: 0px;
        }

        31. bottom : moves the current box 

        32. right : moves the current box 

        31 & 32 EXAMPLE CODE: 

        .hero-form {
        border: 3px solid #024e76;
        background-color: #fce138;
        padding: 20px;
        width: 500px;
        color: #024e76;
        position: absolute;
        bottom: 120px;
        right: 140px;
        }

        33. Chrome DevTools 
        - To access, click the small menu button at the top right of chrome
            - This button will look like three vertical circles. 
                - Then click "More tools" 
                    -Then click "Developer Tools" 
                        - Then click the "Elements" tab to reveal the HTML code. 
        ** DEVTOOLS is a big assets to front-end developers because it allows you to do the following
            * Change HTML elements and attributes
                * Manipuilate CSS style properties
                    * Change the text content
                        * and much more, which we'll continuously learn throughout this class. 
        ** Look at the "box-sizing" property to observe the width of the elements. 

        34. margin : text spacing and word wrapping 
            EXAMPLE 
            .hero-form p {
                margin: 5px 0 15px 0;
            }

        35. font-size : helps with font of text in the input fields. 

        36. display : aid in help with elements sitting in a row or column 

        37. <img> : display graphical content

        38. <span> : elements to highlight inline content. 

        39. div : each div wrapping in it's own section to keep the step title and description coupled together. 

        40. id : attribute 


In index.html, add the following id attributes to the appropriate sections:





TIP FOR THE CSS BOX MODEL:

    Content: The innermost box that contains the text. as well as any nested elements. The size is determined by the height and width.

    Padding: inside margi within the CSS box, each of the four sides of the padding size can be specified. 

    Border: sits on the outside edge of the padding and the inside edge of the margin. This layer's sides, size, and styles can be specified
    similarly to the padding and margin. Such border-bottom or border-style or even border-top-color. This property needs a weight of the line,
    style and color to render. 

    Margin: behaves alot like padding, except whereas padding creates sapce inside the box, margin creates space outside the box and pushes any 
    other HTML elements before and after it away. It also behaves like padding in the way its values are provided ( top, right, bottom and left.)


