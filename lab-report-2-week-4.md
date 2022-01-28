# ~Week 4 Lab Report~

## Commit #1 ##

### Code Change #1 ###
![image](https://user-images.githubusercontent.com/97643301/151611664-f60b6861-584f-4c05-8ace-7b3e425ae476.png)
==

### Link to the test file for a failure-inducing input that prompted a change ###
[Link to Test File](https://github.com/k3alvare/markdown-parse/blob/main/test-file.md)
==

### Symptom of failure-inducing input at the command line for the version where it was failing ###
![image](https://user-images.githubusercontent.com/97643301/151612113-f1839181-f7ec-466e-8ee2-7a12b706d15f.png)
==

### Relationship between the bug, the symptom, and the failure-inducing input ###
In this case there was no bug, as there were no problems with the computer itself, however there was symptoms when the program was ran, which had nothing to do with a failure-inducing input as the test-file contained inputs that were of legal argument. The symptom in this case was a problem in the code in which it threw a `Java heap space` error which was resolved by indicated where the `currentIndex` should be after adding a link. 


## Code Change #2 ##

### Code Change #2 ###
![image](https://user-images.githubusercontent.com/97643301/151614606-520d7fab-afe3-4f35-9c91-ba82d830010a.png)
==

### Link to the test file for a failuire-inducing input that prompted a change ###
[Link to test file](https://github.com/k3alvare/markdown-parse/blob/main/test-file2.md)
==

### Symptom of failure-inducing input at the command line for the version where it was failing
![image](https://user-images.githubusercontent.com/97643301/151614807-c91006d7-18be-4fc4-8c17-80005401b635.png)
==

### Relationship between the bug, the symptom, and the failure-inducing input
In this case there was no bug either, as there were no hardware/computer problems, however there was symptoms when the program ran. This was cause as the failure-inducing input were characters that weren't a link, and the code didn't know when to break as a result of this failure-inducing input which cause the symptoms to show. Once the code was fixed, the symptoms were relieved.


