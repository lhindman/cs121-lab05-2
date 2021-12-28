# Lab05 Guide
## Getting Started
[Lab Introduction Video](https://youtu.be/4m5AwuwMg6E)  

- Please clone the [Mod05 Code Examples](https://github.com/lhindman/cs121-mod05-examples.git).
- Please watch the [M.A.S.H. and Gradebook Activity Overview Videos](https://www.youtube.com/playlist?list=PLbxWwkW_BhyBcxkgU0tQpIh_YdCUVFC52).  


### Code Style Requirements
Please review the [CS121 Style Guide](https://docs.google.com/document/d/1LWbGQBKkApnNAzzgwOSvRM03DmhYWx5yEfecT2WXfjI/edit?usp=sharing) and apply it in all lab activities and projects this semester. Coding Style will assessed as part of your lab and project grades.

### Code Quality Requirements
- Code must compile without warnings using openjdk11
- Code must run without errors or warnings on safe-path and edge test cases
- More to come as we learn about input validation and exception handling

## Activity 1 - CoinFlip
### Problem Description

Write a program that simulates flipping a coin to make decisions. The input is how many decisions are needed, and the output is either heads or tails. Assume the input is a value greater than 0.

Ex: If the input is:
```
3
```
the output is:

```
tails
heads
tails
```
For reproducibility needed for auto-grading, seed the program with a value of 2. In a real program, you would seed with the current time. In that case, every program's output would be different, which is what is desired but can't be auto-graded. 

Note: A common student mistake is to create an instance of Random before each call to rand.nextInt(). But seeding should only be done once, at the start of the program, after which rand.nextInt() can be called any number of times. 

The program must implement a method named *headsOrTails* that will perform the random selection. The javadoc comment below provides details on the expected behavior of this method as well as the required header (signature) of the *headsOrTails* method.
```
/**
 * Randomly pick 0 or 1 using the specified Random object and use them to 
 *    represent "heads" or "tails" respectively. Assume the value 0 represents
 *    "heads" and the value 1 represents "tails."  Return a String that 
 *    contains the randomly selected word.
 *
 * @param rand Reference to Random object to use for calls to nextInt()
 * @return String containing the randomly selected "heads" or "tails"
 */

 public static String headsOrTails(Random rand)
 ``` 


### Implementation Guide
1. Expand the folder named A1-CoinFlip and create a new file named CoinFlip.java
2. Design a program to satisfy the requirements in the Problem Description and enter the program code in CoinFlip.java
3. Test the program using the run link above the main method. Carefully think about each of the different cases you'll need to test for to verify that the application is functioning properly.
4. Commit the changes to your local repository with a message stating that Activity 1 is completed.
5. Push the changes from your local repository to the github classroom repository.

## Activity 2 - CoinFlip (revisited)
### Problem Description

Write a program that simulates flipping a coin to make decisions. The input is how many decisions are needed, and the output is either "heads" (true) or "tails" (false). Assume the input is a value greater than 0. The behavior and expected output of this program (from the user's perspective) should be identical to that of Activity 1.

Ex: If the input is:
```
3
```
the output is:

```
tails
heads
tails
```
For reproducibility needed for auto-grading, seed the program with a value of 2. In a real program, you would seed with the current time. In that case, every program's output would be different, which is what is desired but can't be auto-graded. 

Note: A common student mistake is to create an instance of Random before each call to rand.nextInt(). But seeding should only be done once, at the start of the program, after which rand.nextInt() can be called any number of times. 

The program must implement a method named *truesOrFalse* that will perform the random selection. The javadoc comment below provides details on the expected behavior of this method as well as the required header (signature) of the *truesOrFalse* method. Please **DO NOT** use the *nextBoolean()* method from the Random object to implement this method.
```
/**
 * Randomly pick 0 or 1 using the specified Random object and the *nextInt()* method to 
 *    represent **true** or false **respectively**. Assume the value 0 represents
 *    true and the value 1 represents false.  Return a String that 
 *    contains the randomly selected word.
 *
 * @param rand Reference to Random object to use for calls to *nextInt()*
 * @return boolean containing the randomly selected true or false
 */

 public static boolean trueOrFalse(Random rand)
 ```

### Implementation Guide
1. Expand the folder named A2-CoinFlipV2 and create a new file named CoinFlipV2.java
2. Design a program to satisfy the requirements in the Problem Description and enter the program code in CoinFlipV2.java
3. Test the program using the run link above the main method. Carefully think about each of the different cases you'll need to test for to verify that the application is functioning properly.
4. Commit the changes to your local repository with a message stating that Activity 2 is completed.
5. Push the changes from your local repository to the github classroom repository.

## Activity 3 - Counting Characters
### Problem Description

Write a program whose input is a character and a string, and whose output indicates the number of times the character appears in the string.

Ex: If the input is: 
```
n Monday
```
the output is:
```
1
```

Ex: If the input is: 
```
z Today is Monday
```
the output is:
```
0
```

Ex: If the input is: 
```
n It's a sunny day
```
the output is:
```
2
``` 

Case matters. n is different than N. 

Ex: If the input is: 
```
n Nobody
```
the output is:
```
0
```

The program must implement a method named *countCharacters* that will perform the counting. The javadoc comment below provides details on the expected behavior of this method as well as the required header (signature) of the *countCharacters* method.   

```
/**
 * Count the number of times that the specified character, userChar, occurrs in 
 *  the specified String, userString.  Return that number to the caller as an integer.
 * 
 * @param userChar character to count occurrences of in String
 * @param userString text to scan for occurrences of userChar
 * @return the number of times userChar is found in userString
 */

public static int countCharacters(char userChar, String userString)
```

### Implementation Guide
1. Expand the folder named A3-CharacterCounter and create a new file named CharacterCounter.java
2. Design a program to satisfy the requirements in the Problem Description and enter the program code in CharacterCounter.java
3. Test the program using the run link above the main method. Carefully think about each of the different cases you'll need to test for to verify that the application is functioning properly.
4. Commit the changes to your local repository with a message stating that Activity 3 is completed.
5. Push the changes from your local repository to the github classroom repository.


## Activity 4 - M.A.S.H. Game
### Problem Description
M.A.S.H. is a text-based game that will predict your future!  M.A.S.H. is an abbreviation for the potential future places of residence: Mansion, Apartment, Shack, House. :)  

The details for this activity are in the guide below: 

[M.A.S.H. Activity Guide](https://docs.google.com/document/d/1-xPfyvufVYh6HVFAUjgjeazvw8aZEHjHK0gXFKKRa4Q/edit?usp=sharing)


### Impementation Guide
1. Expand the folder named A4-MASHGame and open the file named MASHGame.java
2. Modify the existing MASHGame.java program as specified in the M.A.S.H. Activity Guide
3. Test the program using the run link above the main method
4. Commit the changes to your local repository with a message stating that Activity 4 is completed.
5. Push the changes from your local repository to the github classroom repository.

## Activity 5 - Gradebook
### Problem Description
This activity demonstrates how to handle File I/O and Exception handling in Java by creating a simple Gradebook application. The details for this activity are in the guide below:

[Gradebook Activity Guide](https://docs.google.com/document/d/133y2yFQUiQxowdil4mygw4jl01NunzAJwTCxC2YfB2A/edit?usp=sharing)

### Impementation Guide
1. Expand the folder named A5-Gradebook and open the file named Gradebook.java
2. Modify the existing Gradebook.java program as specified in the Gradebook Activity Guide
3. Test the program using the run link above the main method
4. Commit the changes to your local repository with a message stating that Activity 5 is completed.
5. Push the changes from your local repository to the github classroom repository.
