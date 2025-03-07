# lumel_technologies-on-campus-interview-coding-question
 The  question that has been asked in lumel technologies oncampus drive process round 2 coding question
 Given encoded string str such that ‘a’ is written 1 time, ‘b’ is written 2 times, and so on, until ‘z’ is written 26 times, the task is to decode the given string str. 

Note: The letter may contain spaces and punctuation marks, so don’t ignore those.

Examples:


Input: str = “bbadddd”
Output: bad
Explanation:
As each letter is written corresponding to the number of appearances in the English Alphabets. Therefore, the resultant string is “bad”.


Input: str = “abbbbacccdddd”
Output: abbacd


Approach: The given problem can be solved by iterating the given string str, and for each character and push that character in an output string and move that respective position ahead to check for the other character. Follow the steps below to solve the problem:

Initialize a variable, say output as an empty string that stores the resultant string.
Define a function findRepetition(char c) and perform the following steps:
If the value of c is in the range from a to z, then return the value of c-‘a’.
Otherwise, if the value of c is in the range from A to Z, then return the value of c-‘Z’.
Otherwise, return 0.
Iterate over a range [0, N] using the variable i and perform the following steps:
Push the ith character of the string str into the string output.
Call the function findRepetition(str[i]) to count the number of steps ith index has to move ahead.
After performing the above steps, print the string output as the resultant string.
