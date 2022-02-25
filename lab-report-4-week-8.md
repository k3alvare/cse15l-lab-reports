# Week 8 Lab Report 4
## What should each Snippet produce?

---

**Snippet 1:** 

_Links:_ [%60google.com, google.com, ucsd.edu]

<img width="557" alt="image" src="https://user-images.githubusercontent.com/97643301/155625862-d459322d-de2f-44c8-b897-2eae385aa6b4.png">

---

**Snippet 2:** 

_Links:_ [a.com, a.com(()), example.com]

<img width="559" alt="image" src="https://user-images.githubusercontent.com/97643301/155625937-d2128de3-a589-4a7a-be6c-96f2b4b46dcc.png">

---

**Snippet 3:** 

_Links:_ [https://ucsd-cse15l-w22.github.io/]

<img width="561" alt="image" src="https://user-images.githubusercontent.com/97643301/155626041-adeaf063-f5ed-4fd7-baba-d2ce74233d71.png">
 
 ---
## Code for MarkdownParseTest.java  

<img width="471" alt="image" src="https://user-images.githubusercontent.com/97643301/155626534-6710ea2a-4d2f-44cf-8ce7-e4432bf3e504.png">



## Own Implementation of MarkdownParse
[Link To Own Implementation](https://github.com/k3alvare/markdown-parse)

---

### Result for Snippet #1

<img width="782" alt="image" src="https://user-images.githubusercontent.com/97643301/155626712-b25cd399-c901-4a65-bc61-0712f560b8e3.png">

---

### Result for Snippet #2

<img width="655" alt="image" src="https://user-images.githubusercontent.com/97643301/155626745-6743d740-ca16-4702-9990-a9703cc289a1.png">

---

### Result for Snippet #3

<img width="524" alt="image" src="https://user-images.githubusercontent.com/97643301/155626778-3178984c-53ae-47dc-8e0b-22a40c4deab6.png">

---

## Review Implementation of MarkdownParse
[Link To Review Implementation](https://github.com/annakkin/markdown-parse)

---

### Result for Snippet #1

<img width="722" alt="image" src="https://user-images.githubusercontent.com/97643301/155627450-05ed8fc2-fc53-4289-9713-7908f1e2f239.png">

---

### Result for Snippet #2

<img width="580" alt="image" src="https://user-images.githubusercontent.com/97643301/155627478-9f3c192c-ca0e-4af0-80dd-dc62c805027f.png">

---

### Result for Snippet #3

<img width="489" alt="image" src="https://user-images.githubusercontent.com/97643301/155627526-d923e4bf-5a7f-411e-939f-f319f0ed23b3.png">

---

## Answering the Following Questions 
### Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.
 Yes, I do believe there is a small change of code the will make the program work and thats adding a variable that checks and holds the positions of the back ticks.
 Then adding another part within a if statement to check if those both back ticks are found within the open and close brackets, to still take it in as a link, and if the back ticks (either one or both) are found within the paranthesis, to still take it in as a link. In the case where the back tick is found in the open and closed bracket, and another is found outside of it, then it shouldn't count as a link.
 
 ---

 
### Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.
Yes there is a small change that will be able to make the program work, and thats including a line of code similar to lecture where there anything before the last closed parantheses, to hold that text after the first open parantheses and consider that the "markdown link" as a way to be able to include those closed parantheses. For the other cases, the code already made holds that change.

---

### Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.
No, there is no small code change that will make the program work as it has to check for a lot of things such as new lines, and if there's any text in those new lines. It also has to check for the correct parantheses and brackets in order to be considered a link. It is a bit nuanced to as this has many variability and many cases that will not be able to be solved with less than 10 lines of code.
