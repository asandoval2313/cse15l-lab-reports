# Week 3-4 Lab Report

### If you'd like to read my first lab report, please head [here](https://asandoval2313.github.io/cse15l-lab-reports/lab-report-1-week-2.html)

# Code Change #1

## Commit Message
![Image](codechange1.PNG)

[Test File that Prompted Fix](https://github.com/leahkuruvila/markdown-parser/blob/6938e7d578994dbde1da1c611c9ee5034838fcc9/test-file.md)

## Symptom/Error
![Image](symptom1.PNG)


## Explanation
 Whenever there was anything after the link in the markdown file, it would infinetely search for the next open bracket. To fix this, we set a criteria where if it didn't find an opening bracket, aka ```openBracket == -1```, then it would break out of the for loop. This indicated that it had reached the end of the markdown file without finding an open bracket. 

# Code Change #2

## Commit Message
![Image](codechange3.PNG)

[Test File that Prompted Fix](https://github.com/asandoval2313/markdown-parser/blob/main/test1.md)

## Symptom/Error
![Image](symptom2.PNG)


## Explanation
 In the test file you can see that there is an open bracket, closing bracket, open parentheses, and closing parentheses, all in the order that the code is searching for. However, the open parentheses is not directly next to the closing bracket, meaning that it is not a link and therefore should not be printed. To fix this, we made a check to see if the index of the open paren is right next to the index of the closing bracket. If it's not, it starts looking for the next open bracket starting at the index of the closing bracket + 1.

# Code Change #3

## Commit Message
![Image](codechange2.PNG)

[Test File that Prompted Fix](https://github.com/asandoval2313/markdown-parser/blob/main/test2.md)

## Symptom/Error
![Image](symptom3.PNG)


## Explanation
This tet file prompted another heap error, meaning that it was going on infiitely. This happened because there was a lone open curly bracket. This error is very similar to the first bug I mentioned, which is my partner and I were confused at first since we thought we had fixed it. We ended up having to add a conditional to each index variable to make sure that when looking for any character you wouldn't reach the end of the file. 
