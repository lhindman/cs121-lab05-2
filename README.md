# Module 5 Lab Guide (part 2)

## Lab Activity 2 - HousingCrunch (Required)
### Problem Description
For this lab activity, the HousingCrunch activity in part 1 will be modified to load housing data from a CSV file instead of having the options manually added to the houseList (also known has hard-coded). In addition to prompting the user for name and a seed value, the program should also prompt for the filename containing the housing data. The data file will contain more data fields than will be used in this application as we are only interested in the housing data stored in the 1st field. The screenshot below shows a spreadsheet view of the provided CSV data with the first field of each row outlined in red.

<img src="images/MASHDatabase.png" alt="MASH Database Spreadsheet" width="653">

***It will be extremely helpful to review the CSVParser Deeper Look Video and Guided Experimentation examples before starting on this activity.***

NOTE:  In Computer Science we teach students to begin counting at zero because zero is the first index value of arrays, strings and many other programming related things.  When working with data from muggles (non-programmer folk), the first data element is often referred to as *record 1* or *row 1* or *column A* or *field 1*. Just open a spreadsheet and look at the column and row identifiers.  As programmers it is our responsibility to be aware of this difference and make certain our programbs behave accordingly.

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
