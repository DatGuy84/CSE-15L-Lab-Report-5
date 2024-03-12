## Lab Report 5 - Putting It All Together

# Part 1

# Student's post

Hello.  I tried creating a method that would return the median of an array in ```ArrayExamples.java```.  In order to check if my 
methods were correct, I created another java file, ```ArrayTests.java ``` that would test each method and a bash script, ```test.sh```
that would compile the java files, and run the tester file.  While the median method seem to have worked,
it seems that the ```inOrder``` method failed which makes me believe that the ```median``` method is also wrong.  I
would appreciate help on this problem.

```
Array Methods
```
![Image](https://github.com/DatGuy84/CSE-15L-Lab-Report-5/blob/main/pre-code.png?raw=true)

```
Java Test File
```
![Image](https://github.com/DatGuy84/CSE-15L-Lab-Report-5/blob/main/pre-tests.png?raw=true) 

```
Bash Script
```
![Image](https://github.com/DatGuy84/CSE-15L-Lab-Report-5/blob/main/bash%20script.png?raw=true)
```
Errors produced
```
![Image](https://github.com/DatGuy84/CSE-15L-Lab-Report-5/blob/main/bash%20error.png?raw=true) 

# TA's response
Hello.  It seems like your bash script and works fine, however, there are some errors I have spotted in your code.
The second for loop in your ```inOrder``` method seems to end right as your outer loop iterates, and it the method
iterates the wrong variable.  Additionally, the reason why your 
