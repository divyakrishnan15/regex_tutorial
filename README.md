
 
<h1 align="center">REGEX (regular expression) Tutorial👋</h1>

<p align="center">
    <img src="https://img.shields.io/github/repo-size/divyakrishnan15/regex_tutorial" />
    <img src="https://img.shields.io/github/languages/top/divyakrishnan15/regex_tutorial"  />
    <img src="https://img.shields.io/github/issues/divyakrishnan15/regex_tutorial" />
    <img src="https://img.shields.io/github/last-commit/divyakrishnan15/regex_tutorial" >
    <a href="https://github.com/divyakrishnan15"><img src="https://img.shields.io/github/followers/divyakrishnan15?style=social" target="_blank" /></a
</p>
  
<p align="center">
    <img src="https://img.shields.io/badge/regex"  />
</p>

 ## Table Of Contents : 
 1.  [Documentation](#documentation) 

        1.  [Title](#Title) 

        2.  [Description](#Description) 

        3.  [Questions](#Questions) 

        4.  [Installation](#Installation) 

        5.  [Usage](#Usage) 

        6.  [Video](#Video) 

        7.  [License](#License) 

        8. [Tests](#Tests) 

        9. [Screenshot](#screenshot) 
 
 ## Character Classes: :  
 <a name="Description"></a>
asdas

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |



 ## 1. Using String search() With a String :  
 <a name="Installation"></a> 
```shell
<!DOCTYPE html>
<html>
<body>

<p>Search a string for "divya", and display the position of the match:</p>

<p id="demo"></p>

<script>
let text = "hi divya!"; 
let n = text.search("divya");
document.getElementById("demo").innerHTML = n;
</script>

</body>
</html>
```

Output:
Search a string for "divya", and display the position of the match:

6


 ## 2. Using String search() With a Regular Expression :  
 <a name="Installation"></a> 
```shell
<!DOCTYPE html>
<html>
<body>

<p>Search a string for "divya", and display the position of the match:</p>

<p id="demo"></p>

<script>
let text = "hi divya!"; 
let n = text.search(/w3Schools/i);
document.getElementById("demo").innerHTML = n;
</script>

</body>
</html>
```

Output:
Search a string for "divya", and display the position of the match:

6
