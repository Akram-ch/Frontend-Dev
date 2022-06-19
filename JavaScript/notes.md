# Notes for JavaScript course module

The simplest way to get started is to simply create an HTML file with the JavaScript code inside of it. Type the basic HTML skeleton into a file on your computer somewhere:
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Page Title</title>
</head>
<body>
  <script>
    // Your JavaScript goes here!
    console.log("Hello, World!")
  </script>
</body>
</html>
```

**<span style="color: pink">console.log()</span>** is the command to print something to the developer console in your browser.

Another way to include JavaScript in a webpage is through an external script. This is very similar to linking external CSS docs to your website.
```html
  <script src="javascript.js"></script>
  ```
  JavaScript files have the extension .js

___
## Variables
Until recently there was only one way to create a variable in JavaScript — the **var** statement. But in the newest JavaScript versions we have two more ways — **let** and **const**

## Strings
A **string** is simply a piece of text… and is a fundamental building block of the language.