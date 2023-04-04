# Vulnerability Taxonomy CWE Homework

#### Name: Cody Southworth

 ## CWE Choosen: CWE-787: Out-of-bounds Write

- An Out-of-Bounds-write vulnerability occurs when a program writes data outside the boundaries of a specific memory area, potentially overwriting data in adjacent memory locations. This type of vulnerability can be exploited by attackers to execute malicious code or cause a program to crash. Out-of-bounds writes can happen due to programming errors such as buffer overflows, uninitialized variables, or incorrect calculations of memory size. These errors can cause the program to access memory locations that are not allocated for it, leading to unintended behavior.

- For example, let's consider a program that uses an array to store user input. If the program does not perform proper bounds checking on the input size, an attacker could provide input that exceeds the size of the array, causing an out-of-bounds write vulnerability. The attacker can then write arbitrary data into memory beyond the end of the array, potentially overwriting data in adjacent memory locations. This could lead to the program crashing or executing malicious code. 

- I have done this exact mistake when I was first here at Wright State when I was enrolled in CS 1180. Plenty of times I had created an array to store a user's input whether it be an array string of characters or a specific amount of numbers and I did not do proper bounds checking on the input size and each time it caused an Out-of-bounds error. One specific instance that I can recall it happening was, I believe it was the project where we had to store a user's deck of cards, the number on the card, and the suite of the cards. When creating that array to store the user's cards, number, and suite I had not implemented that bounds check. I did in fact implement a bounds check to make sure there was a very specific int, and char within those arrays to make sure no other data is stored and did not receive an Out-Of-Bounds-write. I do not remember specifically what I implemented but I did, however, was able to fix that error and not allow it to continue. 
