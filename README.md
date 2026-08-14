MAJORITY ELEMENT
Explanation

The Majority Element problem requires finding the element that appears more than n / 2 times in an array.

The program uses the Boyer-Moore Voting Algorithm to find the majority element efficiently.

Problem Statement

Given an array nums of size n, return the majority element.

The majority element is the element that appears more than n / 2 times.

Features
Finds the majority element
Uses Boyer-Moore Voting Algorithm
Traverses the array only once
Does not require an additional data structure
Uses constant extra space
How It Works

The program maintains two variables:

candidate
count

The candidate represents the current possible majority element.

The count represents its current voting strength.

When the current element matches the candidate, the count increases.

When it is different, the count decreases.

If the count becomes zero, the current element becomes the new candidate.

Because the majority element appears more than half the time, it remains as the final candidate.

Technologies Used
Arrays
Loops
Conditional statements
Methods
Boyer-Moore Voting Algorithm
Data Structure Used

The program uses an integer array.

No additional data structure is required.

Methods Used
majorityElement()

Uses the Boyer-Moore Voting Algorithm to find and return the majority element.

main()

Creates the sample input, calls majorityElement(), and displays the result.

Program Flow
Start
↓
Read array
↓
Set candidate
↓
Set count to 0
↓
Traverse array
↓
Check count
↓
Update candidate if required
↓
Increase or decrease count
↓
Continue traversal
↓
Return candidate
↓
Display result
↓
End
Sample Input
nums = [2, 2, 1, 1, 1, 2, 2]
Sample Output
Majority Element: 2
Time Complexity
O(n)

The array is traversed once.

Space Complexity
O(1)

Only two variables are used.

Key Learning

This problem teaches the Boyer-Moore Voting Algorithm, which efficiently finds the majority element using constant extra space.

File Location
Arrays/MajorityElement.java
Repository Structure
Majority-Element/
├── README.md
└── Arrays/
    └── MajorityElement.java
Author

V.Harini
