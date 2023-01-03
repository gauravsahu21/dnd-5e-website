# Fatespinner: A D&D 5e Character Creator

### Getting Started:

Check under the "projects" tab to view the list of tasks that need to be complete. If you are working on a task, change it to "In Progress", and once it is complete change it to "Done". Feel free to add tasks you think need to be done, just be kind and include a short description of it.

Review my (Frank's) wireframe pdf in the *wireframes* folder for how the website should generally look and be organized. If you feel like you have an idea that works better, try it out! Nothing right now is set in stone, so experimentation is encouraged!

Follow the **Coding Style & Conventions** section below for how to make your code neat and readable.

Currently, all work should be done within the "Stage 2" folder. We will not be using React until all current tasks are complete.

Before working, please pull from "main" branch, then create your own local branch and switch to it for whatever work you want to do. Do not merge with "main" without permission.

For more information on using Git branches: https://info201.github.io/git-branches.html

### Coding Style & Conventions:

Use camelCase for naming variables/functions!

With that out of the way, these are my big 3 rules for this project:
 
 1. **Indent and space out your code so it is readable!**
 
 Generally, every time you use an opening curly brace "{", you should indent subsequent lines of code by 1 tab's worth of space. Every time you use a closing curly brace "}", you should remove 1 tab's worth of indentation for subsequent lines of code.
 ```
 function getExponentValue(num, exponent) {
     if (exponent == 0) {
         return 1;
     }
    
     let exponentValue = num;
    
     for (int i = 1; i < exponent; i++) {
         value *= num;
     } 
    
     return value
 }
 ```
 
 Additionally, space out mathematical operators so that your code isn't so squished together.
 
 ```
 GOOD:
 int index = nameArray.length - 1;
 
 BAD:
 int index=nameArray.length-1;
 ```
 
 Lastly, do not create multiple variables on the same line. Put them on different lines!
 
 ```
 GOOD:
 let index = 0;
 let pointer = 1;
 let pointer2 = 2;
 
 BAD:
 int index = 0;int pointer = 1; int pointer2 = 2;
 ```
 
 **2. Use descriptive variable & function names.**
 
 DO NOT use single-letter variable names! Put in the extra effort to make something a little more descriptive. Even a three-letter name is much better. The only exception is the "i" variable in for loops!
 
 ```
 GOOD:
 let index = 0;
 let currentClass = "Ranger"
 let classArray = [];
 
 BAD:
 let x = 0;
 let c = "Ranger"
 let array = [];
 
 ```
 
 **3. Use comments to describe funtions, complex lines of code, and important variables!**
 
 When commenting on functions, always describe:
 - What the inputs are.
 - What the function does. (Do not describe HOW it does it, just tell readers WHAT it does!)
 - If it returns a value, what it is returning.
 - If there are any important exceptions, such as special input values and fail cases.
 
  ```
 // Takes in an integer value and exponent, and returns the value of the calculated
 // exponent. If the exponent is 0, returns 1.
 function getExponentValue(num, exponent) {
     
     // Any value with a 0th exponent has a value of zero. 
     if (exponent == 0) {
         return 1;
     }
    
     let exponentValue = num;
     
     for (int i = 1; i < exponent; i++) {
         value *= num;
     } 
    
     return value
 }
 ```
 Also, if there are any important variables that you feel the variable name is not descriptive enough, add a comment above it!
 
 ```
 // Keeps track of the user's selected class.
 int currentClass = "Rogue"
 ```

 There are many more coding conventions that I'd like to touch on, but these are the ones I care about the most right now. If problems arise, I will address them as they come.
 
### Stage 1:
Contains test code for developing basic functionality of website (i.e. parsing .json files)

### Stage 2:
Contains html/css/js code for the overall look and feel of website.

### Resources:

[5etools GitHub](https://github.com/5etools-mirror-1/5etools-mirror-1.github.io/releases/tag/v1.174.1): This is where I got all the .json files from, as well as some images.

UW CSE 142/143 Guides on Good Coding Practices [1](https://courses.cs.washington.edu/courses/cse143/17su/handouts/style-guide.pdf) [2](https://courses.cs.washington.edu/courses/cse143/22wi/homework/commenting-guide.pdf) [3](https://courses.cs.washington.edu/courses/cse142/21au/quality.html#indentation): Very comprehensive guides on good coding practices using Java, applicable in any coding environment.

[W3Schools](https://www.w3schools.com/): Fantastic online reference for all things HTML/CSS/JS that everyone I've ever encountered has used. 

[UW INFO 340 Client-Side Programming Textbook](https://info340.github.io/): Public, free-to-use guide for HTML/CSS/JS, React, and Firebase. If you need a guide on more complex operations, check here.
