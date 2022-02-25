# Introduction

In this lab report, I will observe the output of my markdown-parse and one that I reviewed under certain cases and either provide a fix for each if the fix is trivial, or explain why the fix must be non-trivial.

## Snippet 1

### Expected output

![image](ExpectSnip1.png)

according to the markdown preview in vsCode, the expected output should be links 2, 3, and 4.  (\`google.com, google.com, ucsd.edu) 

### Output of my markdown-parse

![image](MySnip1TO.png)

My markdown-parse fails to exclude the first link because there are no checks for backticks inside the brackets.  A three line fix for this is to make a string that is the substring of markdown between nextOpenBracket and nextCloseBracket, check if charAt(\`) !=-1 in an if statement on a second line, and set current index to nextCloseParen if that was true.
