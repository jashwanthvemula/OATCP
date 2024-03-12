Algorithm Description: Dice Rolling Problem
Problem Statement:

Given a target number NN, you need to find the number of ways to reach NN by rolling a dice. The dice has 6 faces numbered from 1 to 6.
Approach:

The provided C++ code solves the Dice Rolling Problem using dynamic programming and recursion.

    Function Explanation:
        The countWays function recursively calculates the number of ways to reach the target sum by rolling a dice.
        It maintains a memoization array (memo) to store the number of ways for each possible sum.
        If the current sum equals the target sum, it returns 1 (a valid way).
        If the number of ways for the current sum is already calculated and stored in the memoization array, it returns the precomputed result.
        Otherwise, it recursively explores all possible dice rolls from 1 to 6 and sums up the number of ways for each possible next sum.

    Main Function:
        The main function reads the number of test cases from the input file input.txt.
        For each test case, it reads the target number from the input file.
        It initializes the memoization array with -1 for each test case.
        It then calls the countWays function to calculate the number of ways to reach the target sum.
        Finally, it writes the result to the output file output.txt.
