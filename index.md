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
The second for loop in your ```inOrder``` method seems to end right as your outer loop iterates.  
Additionally, your ```median``` method works because your tester uses an arraywith odd length.  I suggest you 
implement code to work for even length as well.  

# Student's response
Thank you for the helpful advice.  With your help, I found out that in the ```inOrder``` I started and ended at the 
condition which is why the array did not change in the test methods, and it iterated the wrong variable.  To fix 
this, I fixed the inner loop to start at the beginning of the index.  Moreover, I changed the iterating variable 
from i to x in order to fix the iteration problem.  In order to fix the ```median``` method, I added a scenario
where the array length was even where it adds both the middle values and divide them by two.  Also, I added
a test case that properly tests the median method.

```
Code After Changes
```
![Image](https://github.com/DatGuy84/CSE-15L-Lab-Report-5/blob/main/ArrayAFter.png?raw=true)

```
Test Output From Terminal
```
![Image](https://github.com/DatGuy84/CSE-15L-Lab-Report-5/blob/main/bash%20and%20tests.png?raw=true)

# Part 2
Something I learned from my lab experience in the second half of this quarter that I did not know before 
was the uses of keys.  I thought it was interesting how other people could access files on my computer as 
well as others.  The uses of Vim is also what intrigues me because I like the value of remotely editing files.
