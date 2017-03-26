# Module 1 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

## HTML

### Questions

1. What is HTML and what is it used for?
Answer: **HTML is Hypertext Markup Language, which is used to create pages which can link to other pages.**
2. What is the difference between an ID and a class?
Answer: **An ID is more specific, and should only be used once in a document, whereas a class can be used as a part of many different objects to group them together with identical stylings.**
3. What does it mean to write "semantic" HTML?
Answer: **It means to write easily readable, efficient, and organized code so that anyone can look at it and find what they need to find.**

### Exercises

1. Write a paragraph tag with a class of "highlight" and content "Watch out!".
    `<p class="highlight">Watch out!</p>`
2. Write an HTML image tag to show an image called `profile-picture.jpg`.
    `<img src="profile-picture.jpg" alt="Profile Picture" />`
3. Write a link tag that links to http://google.com.
    `<a href="http://google.com/">http://google.com</a>`
5. Write a complete standard HTML document outline (including a DOCTYPE, and `<html>`, `<head>`, and `<body>` tags).
    ```html
     <!DOCTYPE html>
     <html>
     <head>
     <script src="main.js"></script>
     <link rel="stylesheet" href="main.css">
     </head>
     <body>
      <ol>
        <li>The Jungle Book</li>
        <li>Treasure Island</li>
        <li>The Scarlet Pimpernel</li>
      </ol>
     </body>
     </html>
     ```
6. Inside of the code for the previous exercise, write the appropriate tag to link to a script file called `main.js`.
7. Inside of the code for the previous exercise, write the appropriate tag to link to a stylesheet file called `main.css`.
8. Write a numbered list in HTML and list three of your favorite books.
9. Fix the indentation of the following HTML sample:

  ```html
  <div>
    <ul>
      <li>The Jungle Book</li>
      <li>Treasure Island</li>
      <li>The Scarlet Pimpernel</li>
    </ul>
  </div>
  ```

## CSS

### Questions

1. What is CSS and what is it used for?
  **Cascading Style Sheets, and it is used for styling HTML to give it color, a layout, and every other design-related feature.**
2. What is the CSS box model?
  **A guideline representing the size of the actual content, padding, border, and margin.**
3. What's the difference between margin and padding?
  **Padding is the space between the content and the border, and the margin is the space between the border and other content on the page.**

### Exercises

1. Write a CSS rule to make the text of all `h1` tags red.
  `h1 {
    color: red;
    }`
2. Write a CSS rule to make the background color of the link with `class="btn"` blue:
   `.btn a {
    backround-color: blue;
    }`

  ```html
  <a href="#" class="btn">Learn more</a>
  ```

3. Write a CSS rule to give the first paragraph in the following HTML a font size of `20px`, but not the second paragraph.
   `.jumbotron p {
    font-size: 20px;
    }`
  ```html
  <header class="jumbotron">
    <p>Hello, World!</p>
  </header>

  <p>Welcome to this awesome website!</p>
  ```

## JavaScript

### Questions

1. What is a function? What are they used for?
 **A function executes a string of commands.**
2. What is the difference between `==` and `===`?
  **The == will try and interpret two values (even if one is a string and one is a number or boolean value, etc) to see if they are even, and if they are, it will evaluate to "true". The === will evaluate to "false" if the two values are not of the same type, even if they contain the same value.**
3. What is the difference between global and local scope variables?
  **Global scope variables apply to every function within the script. Local scope variables only exist within the function they are declared in.**
4. What is a boolean value?
  **A boolean value declares whether something is true, or false.**
5. What is an array?
  **An array is a group of strings, numbers, other arrays, boolean values, etc. all grouped together in order between two brackets.**

### Exercises

1. Write a line that declares a variable called `myName` and set its value to your name.
   `var myName = "Ryan";`
2. Write a loop that logs the numbers 1 through 10 to the console.
   `for (var i = 1; i <= 10; i++){
      console.log(i);
      }`
3. Translate the following pseudocode into JavaScript: if `score` is greater than `3` and `lives` is greater than `0`, alert "You win!".
 `function testFunction (score, lives){
 if (score > 3 && lives > 3){
 alert("You win!");
  }
 }
testFunction (5, 5);`
  
  

4. Write a function `sayHello` that takes one argument, a name, and logs "Hello, <name>!" to the console. Then, call the function below the function definition and pass in your name as the argument.
`function sayHello (name){
console.log("Hello, " + name + "!");
};
sayHello ("Ryan");`

5. What would the following script log to the console?

  ```javascript
  var currentSong = "Call Me Maybe";

  function setSong(song) {
    currentSong = song;
  }

  setSong("Friday, Friday");

  console.log(currentSong);
  ```
  Answer: **Friday, Friday**

6. What would the following script log to the console?

  ```javascript
  var add = function(a, b) {
    return a + b;
  }

  var result = add(3, 7);

  console.log(result);
  ```
Answer: **10**

7. What would the following script log to the console?

  ```javascript
  var helloGoodbye = function(name) {
    return sayHello(name) + " " + sayGoodbye(name);
  }

  var sayHello = function(name) {
    return "Hello " + name " !";
  }

  var sayGoodbye = function(name) {
    return "Goodbye " + name " !";
  }

  console.log(helloGoodbye("Sarah"));
  ```
Answer: ----

8. Write a function `findLongestWord()` that takes an array of words and returns the length of the longest one.
9. Define a function `sum()` that sums all the numbers in an array of numbers. For example, `sum([1,2,3,4])` should return 10.
10. Write a function that takes a character (i.e. a string of length 1) and returns true if it is a vowel, false otherwise.
11. Write the correct line to make `"Woof!"` show up in the console based on this script:

  ```javascript
  var pet = {
    name: "Charles",
    goodDog: true,
    speak: function() {
      console.log("Woof!");
    }
  };
  ```
  
  Answer: **I don't know.**

12. Using the same script as above, write the correct line to log the dog's name to the console.

Answer: **Kevin, please help.**

## Command Line

### Questions

1. What is the command line and what is it used for?
 - Command line enables the user to directly communicate to the computer through the terminal and execute commands to do virtually anything the computer is capable of doing without the use of a user interface.
2. What does the command `ls` do?
 - ls lists files and folders in the current directory.
3. What does the command `pwd` do?
 - It prints the working directory-- i.e. "
4. What does the following command do: `cd my-cool-project`
 - It would change the current directory to my-cool-project.

### Exercises

1. Write the command to make a new directory called "my-cool-project".
 - `mkdir my-cool-project`
2. Write the command to create a file called "index.html".
 - `touch index.html`
3. Write the command to delete a file called "main.css".
 - `rm main.css`

## Git

### Questions

1. What is Git and what is it used for?
 - Git is an organization and collaboration system developed to save revisions of code, merge different revisions of the same code, and help people collaborate on a single project more effectively.
2. What's the difference between a local repository and a remote repository?
 - A local repository is a repository stored on a local machine, whereas a remote repository is one which is saved in a remote location (i.e. GitHub)

### Exercises

1. Write the command that you would use to create a new local Git repository.
`git init`
2. Write the command to stage a file called `index.html` to be committed.
`git add index.html`
3. Write the command to view the current status of the git repository.
`git status`
