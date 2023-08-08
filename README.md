
 
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

        3.  [Modifiers](#Modifiers) 

        4.  [Metacharacters](#Metacharacters) 

        5.  [Quantifiers](#Quantifiers) 

        6.  [Sets](#Sets) 

        7.  [Groups](#Groups) 

        8. [Assertions](#Assertions) 

        9. [Screenshot](#screenshot) 
 


## Regular Expression Modifiers / flags
<a id="Modifiers"></a>
| Modifier      | Description |
| ----------- | ----------- |
| i   | Case-insensitive matching |
| g   | Global match |
| m   | ^ and $ start and end of the multi line matching  |
| a   | Matched ASCII only  |
| L   | Locale character classes   |
| s   | Matches evrything including newline as well    |
| u   | Matches unicode character classes   |
| x   | Allow spaces and comments    |





## Metacharacters
<a id="Metacharacters"></a>
| Metacharacter      | Description |
| ----------- | ----------- |
| \w     | Match alphanumeric (a-z, A-Z, 0-9 and underscore(_))   |
| \W     | Match NON alphanumerc other than (not a-z, notA-Z, not0-9, not underscore)   |
| \d     | Match a digit (0-9)  |
| \D     | Match non digit (not 0-9)  |
| \s     | Match whitespace characters with \t, \n, \r and space characters  |
| \S     | Match non-whitespace characters  |
| \A     | Match string to right at absolute start of string whether in single / multiline |
| \Z     | Match string to left at absolute end of string whether in single / multiline |
| \n     | Match a newline character |
| \t     | Match a tab character |
| \b     | Find a match at beginning of word \bdivya or Find a match at end of word divya\b       |
| \B     | Find a match that is non-boundary  |







## Quantifiers 
<a id="Quantifiers"></a>
| Quantifier      | Description |
| ----------- | ----------- |
| n+     | Match a string with atleast one n  |
| n*   | Match a string with 0 or more occurances of n  |
| n?   | Match a string with 0 or 1 occurance of n   |



## Sets
<a id="Sets"></a>
| Modifier      | Description |
| ----------- | ----------- |
| [abc]   | Matches any of a (or) b (or) c. It does not match abc |<pre><p id="demo"></p>
 ```<script>
let text = "Is this all there is?";
let result = text.match(/[h]/g);
document.getElementById("demo").innerHTML = result;
</script> </pre>```|
| [a-z]   | Matches any alphabet from a-z |
| [A-Z]   | Matches any alphabet in Capital from A-Z  |
| [a\-p]  | Matches a, -, or p. It matches – because \ escapes it.  |
| [-z]   | Matches – or z   |
| [a-z0-9]   | 	Matches characters from a to z or from 0 to 9.   |
| [(+*)]   | Special characters become literal inside a set, so this matches (, +, *, or )   |
| [^ab5]  | Adding ^ excludes any character in the set. Here, it matches characters that are not a, b, or 5    |
| \[a\]   | 	Matches [a] because both parentheses [ ] are escaped  |



## Groups:
<a id="Groups"></a>
| Expresions      | Description |
| ----------- | ----------- |
| ( )   | 	Matches the expression inside the parentheses and groups it which we can capture as required |
| (?#…)   | Read a comment |
| (?PAB)   | Matches the expression AB, which can be retrieved with the group name.  |
| (?:A)   | 	Matches the expression as represented by A, but cannot be retrieved afterwards.  |
| (?P=group)   | Matches the expression matched by an earlier group named “group”   |





## Assertions:
<a id="Assertions"></a>
| Expression      | Description |
| ----------- | ----------- |
| A(?=B)   | This matches the expression A only if it is followed by B. (Positive look ahead assertion) |
| A(?!B)   | 	This matches the expression A only if it is not followed by B. (Negative look ahead assertion) |
| (?<=B)A   | 	This matches the expression A only if B is immediate to its left.  (Positive look behind assertion)  |
| (?<!B)A   | This matches the expression A only if B is not immediately to its left. (Negative look behind assertion)  |
| (?()|)   | 	If else conditional   |





 ## 1. search() without regex:  
 <a id="Installation"></a> 
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


 ## 2. search() With a Regular Expression :  
 <a id="Installation"></a> 
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


 ## 3. replace() With a Regular Expression :  
 <a id="Installation"></a> 
```shell
<!DOCTYPE html>
<html>
<body>

<p>Replace "car" with "bus" in the paragraph below:</p>
<button onclick="myFunction()">Try it</button>
<p id="demo">This is a car</p>

<script>
let text = document.getElementById("demo").innerHTML;
  document.getElementById("demo").innerHTML =
  text.replace(/car/i, "bus");
</script>

</body>
</html>
```

Output:
Replace "car" with "bus" in the paragraph below:

Try it
Please visit bus!

 ## 4. test() With a Regular Expression :  
 <a id="Installation"></a> 
```shell
<!DOCTYPE html>
<html>
<body>

<p>Search for an "i" in the next paragraph:</p>
<p id="p01">This is a car!</p>
<p id="demo"></p>

<script>
let text = document.getElementById("p01").innerHTML;
const pattern = /i/;
document.getElementById("demo").innerHTML = pattern.test(text);
</script>

</body>
</html>
```

Output:
Search for an "i" in the next paragraph:

This is a car!

true


 ## 5. exec() With a Regular Expression :  
 <a id="Installation"></a> 
```shell
<!DOCTYPE html>
<html>
<body>

<p id="demo"></p>

<script>
const obj = /i/.exec("This is a car!");
document.getElementById("demo").innerHTML =
"Found " + obj[0] + " in position " + obj.index + " in the text: " + obj.input;
</script>

</body>
</html>
```

Output:
Found i in position 2 in the text: This is a car!
