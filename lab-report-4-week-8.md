## [Index](https://asandoval2313.github.io/cse15l-lab-reports/index.html)

### My Implementation 
[Link to Repo](https://github.com/asandoval2313/markdown-parser)

### Implementation I reviewed
[Link to Repo](https://github.com/leahkuruvila/markdown-parser)

## Snippet 1:

### Expected Output
[\`google.com, google.com, ucsd.edu]

### <u>Junit Test</u>
![image](s1test.png)

### <u>My Results</u>
![image](sn1result.png) 

### <u>Other Results</u>
![image](otheres1.png)

Both my implementation and the implementation I reviewed failed test 1.
## Snippet 2:

### Expected Output
[a.com, a.com(()), example.com]

### <u>Junit Test</u>
![image](snip2.png)

### <u>My Results</u>
![image](snip2result.png)

### <u>Other Results</u>
![image](otherresult2.png)

For this snippet my implementation failed but the implementation I reviewed passed. 

## Snippet 3:

### Expected Output
[(https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule)]

### <u>Junit Test</u>
![image](snip3test.png)

### <u>Results</u>
![image](snip3result.png)

### <u>Other Results</u>
![image](otherTest.png)

For this snippet my implementation failed but the implementation I reviewed passed. For some reson make test was being buggy so I just ended up running it manually.

## Follow up Questions

1. I'm not sure if there's a small code change I can make to fix the first snippet because it would involve parsing the text between brackets and making sure it avoids the bakc ticks. 

2. I think for the secod snippet I could implement some code that only uses the right most parenparenthesis for a link, to avoid the link ending prematurely. 

3. I also don't know if there's an easy fix for snippet 3 because you would have to implement some sort of new logic for looking at line breaks. 
