Cheat Sheet - Directory of Helpful commands & tips for HTML Coding




Prework Overview



Module 0 - Welcome to the Course



Module 1 - 

    1. CLI: command-line interface or Terminal ( A way to interact with the computer " Black Screen " )

    2. pwd: print working directory ( aka the "folder" that the CLI is currently in.)
        - This is pretty much like asking "WHERE AM I?" in the terminal 
            EXAMPLE: " /c/Users/michaelcmaresco/desktop " 
    
    3. ls: list files/folders in current directory. 
        - This is pretty much like asking "WHAT'S HERE?"

    4. cd <directory-name> : Change Directory
        - This allows you to move in and out of directories. 
    
    5. cd .. : Took us back a level or "up a directory"

    6. mkdir <directory-name> : Create a new folder
        - Make directory
            EXAMPLE: " mkdir projects " this will make a folder "projects" in the current directory. 

    7. touch <file-name> : Command used to create files. 
        EXAMPLE: touch hello.txt | This will create a new file "hello.txt"

    8. rm <file-name>: Remove Command
        EXAMPLE: rm hello.txt | This removes the "hello.txt" file or whatever file you input.

    9. . : This syntax means directory 

    10. code . : type this in a current directory to open VS Code.

    11. <title> </title> : Opening tag and a closing tag.
        - This is the name that will be displayed on the Tab name 
            - Anything between these tags is affected by what the element signifies. 

    12. <h1> : level 1 heading. 
        - This text will be the largest, biggest and boldest of the headings. 
    
    13. <h2> : level 2 heading will be slightly smaller than <h1>.
        - As you go up in the numbers, the headings will become smaller than the other headings. 

    14. <h3> : level 3 heading will be slightly smaller than <h2>.
        - As you go up in the numbers, the headings will become smaller than the other headings. 

    15. <html> : Placed at the top of and bottom of an HTML document.
        - Everything within the HTML document EXCEPT THE <!DOCTYPE html> needs to be within this opening and closing tag.

    16. <!DOCTYPE html> 
        - The only acception for what should be outside of the HTML opening and closing tags. 

    17. <head> : one of the two elements of a webpage. 
        - This is where we provide any information that the browser may need to know about the page

    18. <body> : this is where all of the content for the page should go. 

    19. <html lang="en"> : Usually the opening HTML tag. This specifies what language the html is in. 

    20. <meta charset="UTF-8" /> : This is a META TAG.
        - This gives the browser extra information about the page. 
            - Sometimes for display purposes and sometimes for search engine optimization. 
    
    21. charset : the tag important to include because it specifies the range of characters (letters, numbers, symbol, etc.)
        - UTF-8 accomodates just about any character from foreign symbols to emojis. 

    22. main : aka master.

    23. ls -a: display hidden files/etc. 

    24. . : any folder starting with a "." is hidden. 

    25. .git : folder that is marked as hidden because we shouldn't be entering it/ or messing around with it. 

    26. git status: helps us track our codebase in the current directory.
        - The following code should look something like this. 
            
            " $ git status
            On branch main

            No commits yet

            Untracked files: 
                (use "git add <file>..." to include in what will be committed)

                    index.html (**this would be red**)

                nothing added to commit but untracked files present (use "git add" to track)"
    
    27. .DS_Store : will later learn about in the course

    28. Untracked files: files that we have told the computer to never specifically worry about. 

    29. git add <file-name> : Adding a file to Git's tracking
        - usually followed by "git status" 
        - telling Git to "pick up" any new, edited, or removed files in the current project


    30. COMMIT - **EVERYTHING** **VERY IMPORTANT**
        Changes to be committed : a page that needs to be committed. 
            "git commit -m "page template" 
                - Telling Git what you added or changes 
                - Takes everything in staging and commits it. 
                    - the "-m "message" is part of the command that contains a short description of the commit. 
                        -ON YOUR FIRST COMMIT: GIT MIGHT ASK YOU TO IDENTIFY YOURSELF AS SHOWN BELOW.
                                "$ git commit -m "page template"

                                ** Please tell me who you are.

                                Run

                                    git config --global user.email "you@example.com"
                                    git config --global user.name "Your Name" 

                                to set your accounts default identity.
                                Omit --global to set the identity only in this repository
                                "

                        - This is normal, just run the commands the terminal is suggesting 
                            
                                "git config --global user.name "Your Name" "

                        - If you needed to do this step, you need to run the 
                           
                                "git commit -m"page template" command again

                        -You'll know you were successful if this following code appears. 
                           
                                "$git commit -m "page template"
                                [main (root-commit) 414d57f] page template
                                1 file changed, 11 insertion(+)
                                create mode 100644 index.html"

                        - This will ensure you made your commit!
    
    31. git add <file-name> : commit a change to Git
        "git add <file-name>
        git commit -m "add more link text"
        "
    
    32. git log : shows you the log of different commits on the current file

    33. q : how to quit out of the git log and other things. 

    34. <div> : content division  *SEMANTIC ELEMENT*
        - this can basically be different boxes of content 
            <div> hello </div>
            <div> this is a different box of content </div>

    35. div soup : a term describing TOO MUCH <div> in a page of code. 

    36. <header> </header> : opening and closing tags for a heading of a page. *SEMANTIC ELEMENT*
        - This is better than putting a heading in <div> </div>

    37. <footer> </footer> : this has the same function as <div> amd <header> but is dedicated to being the ending of a page. *SEMANTIC ELEMENT*

    38. <jumbotron> : the large image at the top of the element in HTML. *SEMANTIC ELEMENT*

    39. <section> </section> : An element used to divide into sections. *SEMANTIC ELEMENT*

    40. touch .gitignore : create a gitignore file. 
        - This is used to specifiy any files we dont want Git to track. 
            - On MacOS there is a .DS_Store which stores files that would be wasteful to expose to Git. 

    41. git add . : adds any untracked or modified files in the current directory ( the currnet directory is represented by .) and all subdirectories. 

    42. git add -A : adds any files in the entire project. 

    43. git commit -m "html outline and gitignore"

    44. git remote add origin git@githubblahblahblahblahblah.git
        git remote -v
            - this is for linking a remote repository on GitHub. We are linking it to a local project. 

    45. git remote -v : this shows us the remote link, if we've established any.

    46. git push origin main
        - this updates the origin's "main" branch 
        - Push all of the code and file edits from your recent "commit" to GitHub

    47. SSH Passphrase
        - The first time doing this, the computer will ask you if you trust this website. Click yes first. 
            - type "yes" if you trust. Then following any remaining steps. 
    
    48. GitHub username & GitHub password
        - it will ask you this everytime, which is why SSH is more convenient. 

    49. git push - ensures that changes are always make it to GitHub. 
        "git add -A
         git commit -m "<message-that-describes-the-commit>"
         git push origin main

    50. website/contact.html : anytype of website you visit that has this /contact.html will know to send this information back.

    51. <nav> </nav> : navigation

        EXAMPLE: 
            <header>
                <h1>RUN BUDDY</h1>
                <nav></nav>
            </header>

    52. <ol> : ordered lists 
        - tell the browser to interpret any nested list item( denoted with the <li> element) in numeric order (1,2,3,etc.)

    53. <ul> : unordered lists
        - allows for more loosely formatted list by marking each nested list item with a symbol (such as a bullet point or square)

        Ordered lists and unordered lists have a Parent/child relationship 
            <li> = child
            <ol> & <ul> = parent

    54. <li> : anything can be nested in this element. 

    55. <a> : anchor element : used to create links that take us to other destination when clicked. 
            - This destinations when clicked can be within the same page and on another page in the website. OR another website entirely. 
                EXAMPLE: 

                "<!-- When you click "Go to Google," it will take you to Google -->
                <a href="https://google.com">Go to Google</a>

                <!-- This will take us to our own site's privacy policy HTML page -->
                <a href="./privacy-policy.html">View Our Privacy Policy</a>

                <!-- This does nothing at all -->
                <a>This does nothing</a>"

    56. href= : this is an attribute that give an HTML element a unique identity. 
        - They create relationships with other elements and provide design changes using CSS. 
            - They give functionality, meaning and context to HTML elements. 
                - Attributes aren't necessary for every element, but some do require them.
                    - One of them is <a> element. - If we were to omit the href attribute, the links wouldn't work. 


                        Popular attributes:

                            1. id : a unique identifier for an HTML element. 
                                - The value of this c an only be used once per HTML document. 
                            
                            2. class : another way of identifying an HTML element, but it's value is 
                            expected to be mor general and can be reused across multiple HTML elements on a page

                            3. title : not to be mistaken with <title> , holds a value that appears as a small pop-up 
                            (known as a tool tip) when the cursor is pointed at an element for a period of time. 

                        The Value of href - a forward slash "/" : always represents a oath to the topmost directory of an application or project.

                            1. When clicking <a> the user will likely be taken to the topmost directory. 

    57. <link rel="stylesheet" href="./assets/css/style.css" /> : Link a CSS sheet to an HTML page 

    58. <link> : the link to an external file (like a CSS stylesheet)
        - This goes between the opening and closing of <head>

    59. inline style : <h1 style="color: blue; font-size: 100px;">Run Buddy </h1>

    60. rel="stylesheet" : providing information on the nature of the relationship of the linked document. 
        - The one specfied with the href- to the HTML.

    61. /* */ : CSS comments

    62. <!-- --> : HTML comments

    63. <br /> : break element to create a line break between the ___ and ___ 

    64. &copy : copyright symbol

    65. &gt is greater than < or > : but will create a >

    66. href="#what-we-do" : hashtag : helps to navigate between different sections on the same page. 

    67. <p> : paragraph : used to render the text in the page's body. 
        - By default, the browser declares a <p> to be block-level element, but- unlike a heading element - wont assign any changes to font size or weight. 

    68. <label> : offers a visual directive to the associated <input> when a user has a visual impairment. 
        - Links the displayed values to their respective inputs.
            - This enhances accessibility by allowing users to click on a labels text

    69. <input> : where the user inputs text. 

    70. CTA : "Call to action" : a way to encourage visitors via a story, advertiser, dazzling piece of content to do something. 
        - These play a vital role in converting a visitor into a sales lead.
            - That why we want it at the top of the page!

    71. for : **(ATTRIBUTE FOR <label> and <input>)** : ** <label> element ** 
        - This programatically links to the "id" attribute in the <input> element.
            - EXAMPLE: This can reference a radio button to which the label belongs.
            - The value for the "for" attribute must match the value of the "id" attribute of the "<input>" element. 

    72. type : **(ATTRIBUTE FOR <label> and <input>)** : 
        - This relates to the type of input element we're using .
            - In the example below, we want a text field
                - The text field is also the DEFAULT VALUE.

    73. placeholder : **(ATTRIBUTE FOR <label> and <input>)** : 
        - offers a hint or label within the text field, but will not be submitted if this field is left blank.

    74. name : **(ATTRIBUTE FOR <label> and <input>)** : 
        - identifies the element so the response can be referenced after the form is submitted. 
            - EXAMPLE: Radio button elements must have the same "name" attribute in order to be associated with the same radio group. 
            - This is how the browser odentifies that a group of choices can have an exclusive singular answer.
            - In the example below for "radio-button" the radio group in "name" is "trainer-confirm".

    75. </ <label> > : FORWARD SLASH : this forward slash is known as a "self closing tag" and is extremely commmon in HTML. 
        - It is necessary to use when closing a tag. 
            - They dont contain any content or child elements.
                - This is why when you close the tag, it is immediately folloed by the opening tag. 
                    - This shortcut was created to "self-close" the opening tag. 

    76. radio : a type of input element
        - A.k.a "radio button"
            - This is typically used in groups using the "name" attribute as the group reference.
                - EACH RADIO BUTTON MUST HAVE THE SAME "name" VALUE TO BE CONSIDERED IN THE SAME GROUP. 

    77. email & tel : special inputs for browsers
        - These inputs get treated differently than traditional "text"
            - When entering "email" as an input, after submitting ,the browser automatically validates the value. 
            -If the value doesn't look like an email address, the browser won't validate it. 
            -The browser will likely warn you that it is not validated. 
        - When entering "tel" as an input, it is treated like traditional "text". 
            - it wont be validated but on a browser, a numeric keyboard will pop up instead of a regular keyboard. 




Setting up Git Repository

    For Mac:
        1. run this command
            "brew install git"

        2. Set the default branch to "main" through this command.
            "git config --global init.defaultBranch main" 

        3. If successful, no confirmation message will appear. It will simply return back to the command prompt. 

        4. Make sure you're in the correct directory. 

        5. Next, type the following command
            "git init"
                - The command line should print something along the lines of "Initialized empty Git Repository"
                    - If you're computer doesnt recommend the Git command, make sur Git was installed correctly. 

        6. After success, we've create a hidden ".git" file. 
            - To verfiy run the command
                "ls -a"
                    - This will list any hidden files and folders as well as normal files in the current directory.



TIPS: 

    1. When creating a new file always remember to create it in all lowercase. 

    2. When you want to open VS Code from a command line, type this code "code ." in the <file-name> directory.

    3. EVERY PAGE NEEDS A 
        DOCTYPE
        <html> element
        <head> element
            This can be copy and pasted into a future project once it becomes like 2nd nature. 





Example of Module 1 HTML Page Knowledge:

    <!DOCTYPE html>
        <HTML> 
            <head>
                <meta charset="UTF-8 />
                <title>RUN BUDDY</title>

                <style>
                    body {
                        background-color: tomato;
                    }h1 {
                        font-size: 100px;
                    } </style>
            </head>
                <header> 
                <body>
                    <div>
                        <h1> Howdy. </h1>
                    </div>
                    <div>
                        <h2> Welcome to the website of world famous Texan, Michael C. Maresco </h2>

                        <h3> Here you can learn about my portfolio, lifestory and how I rose to being one of the most prominent cowboys </h3>
                    </div>
                <body>
                </header>
            <HTML>



 *SEMANTIC ELEMENTS*
 <div>
 <section>
 <header>
 <footer>
 <nav>






 Tips for Creating a form: 

    1. build a <section> element right below the closing </header> : this will act as a parent element that contains the chidren elements, the heading and sign up form .
    
    2. add a <div> element nested entirely inside the <section> element.
        -ONE IMPORTANT HTML RULE IS THAT BOTH THE OPENING AND CLOSING TAGS OF AN ELEMENT MUST BE COMPLETELY CONTAINED INSIDE THE PARENT ELEMENT. 

    EXAMPLE: 

        <section>
            <div> </div>
        </section>
  
    3. Now that we have the child element, let's insert it's child elements, including a heading for this section and some text. 
    - Add the following elements and content for the heading and paragraph text inside the <div> element 

    EXAMPLE: 

        <section>
            <div>
                <h3> Get started today! </h3>
                <p> fill out this form and one of our trainers will schedule... <p>
            </div>
        </section>

    4. Now insert the <form> </form> into the HTML code.

    NEXT STEP:

    <section>
        <div>
            <h3> Get Started today! </h3>
            <p> if you sign up, a personal trainer will reach out to you..</p>

            <!-- Add form element -->
            <form></form>
        </div>
    </section>

    5. Now insert the <input> and <label>

    EXAMPLE:

    <section>
        <div>
            <h3> Sign up! <h3>
            <p> a trainer will reach out to you.. </p>

            <form>
                <label for="name>Enter full name:</label>
                <input type="text placeholder="Your Name" name="name" id="name>
            </form>

        </div>
    </section>

** It's very important to look at how closely we pair the <input> and the corresponding <label> elements and their attributes, which are shown above (in step 5). 

** The <label> text not onle offers a visual directive of what to enter but also programatically links to the associated <input>.

****THIS IS CRUCIAL WHEN WRITING CODE THAT MAY BE READ ALOUD TO SOMEONE THAT MAY HAVE A VISUAL IMPAIRMENT****
    - Through this, the label will be read out loud when they focus on an input field. 
        - This also makes it easier to fill out forms on mobile devices. Which is a very practical thing for people with visual impairments. Their phone may be their lifeline for medical appointments,etc. 
            - Clicking on the label will target the focus to the associated input field. (Which can be hard to do manually on a small screen).

** To see how the different attributes withing <label> and <input> are broken down, read the elements starting at # 71. above.

    6. Code the fields for email and phone number, also include the attributes for "name", "for", "type", "id" and "placeholder".

    <label for="email">Enter Email Address:</label>
    <input type="text" placeholder="Email Address" name="email" id="email />
    <label for="phone">Enter Phone Number:</label>
    <input type="text" placeholder="Phone Number" name="phone" id="phone" />

Then you should be good to :)




Radio Button Input : How to add it to an HTML Page.
    1. We will begin this by typing this beneath our form code from above. 

        <form>
            <label for="name>Enter Full Name:</label>
            <input type="text" placeholder="Your Name" name="Name" id="Name" />
            <label for="email">Enter Email address:</label>
            <input type="text placeholder="Your Email address" name="email id="email" />
            <label for="phone">Enter Full Phone number: </label>
            <input type="text placeholder=">Your phone" name="phone" id="phone" />
            <p>
                Have you worked out with a trainer before?
                <input type="radio" name="trainer-confirm" id="trainer-yes" />
                <label for="trainer-yes>Yes</label>
                <input type="radio" name="trainer-confirm" id="trainer-no" />
                <label for="trainer-no>No</label>
            </p>
        </form>


    2. Add the checkbox input. 
<section>
    <div>
        <form>
            <label for="name>Enter Full Name:</label>
            <input type="text" placeholder="Your Name" name="Name" id="Name" />
            <label for="email">Enter Email address:</label>
            <input type="text placeholder="Your Email address" name="email id="email" />
            <label for="phone">Enter Full Phone number: </label>
            <input type="text placeholder=">Your phone" name="phone" id="phone" />
            <p>
                Have you worked out with a trainer before?
                <input type="radio" name="trainer-confirm" id="trainer-yes" />
                <label for="trainer-yes>Yes</label>
                <input type="radio" name="trainer-confirm" id="trainer-no" />
                <label for="trainer-no>No</label>
            </p>
            <p>
        <label for="checkbox" >
          I acknowledge that I am at least 18 years of age.
        </label>
        <input type="checkbox" name="age-confirm" id="checkbox" />
      </p>
      <button type="submit">
        Get running!
      </button>
        </form>
    </div>
</section>

    3. Change the specific inputs to "email" and "tel"
<section>
    <div>
        <form>
            <label for="name>Enter Full Name:</label>
            <input type="text" placeholder="Your Name" name="Name" id="Name" />
            <label for="email">Enter Email address:</label>
            <input type="email"Your Email address" name="email id="email" />
            <label for="phone">Enter Full Phone number: </label>
            <input type="tel">Your phone" name="phone" id="phone" />
            <p>
                Have you worked out with a trainer before?
                <input type="radio" name="trainer-confirm" id="trainer-yes" />
                <label for="trainer-yes>Yes</label>
                <input type="radio" name="trainer-confirm" id="trainer-no" />
                <label for="trainer-no>No</label>
            </p>
            <p>
        <label for="checkbox" >
          I acknowledge that I am at least 18 years of age.
        </label>
        <input type="checkbox" name="age-confirm" id="checkbox" />
      </p>
      <button type="submit">
        Get running!
      </button>
        </form>
    </div>
</section>