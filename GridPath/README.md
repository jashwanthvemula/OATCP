Algorithm Description: Grid Path Counting
Problem Statement:

Given a grid of size N×NN×N, where each cell of the grid can either be empty or blocked by an obstacle represented by '*', you need to find the number of unique paths from the top-left corner to the bottom-right corner, considering only right and down movements.

    Function Explanation:
        The f function recursively calculates the number of unique paths from a given cell to the bottom-right corner.
        It traverses the grid from the top-left corner and explores two possible movements: moving right or moving down.
        Base Cases:
            If the current cell is out of bounds or blocked by an obstacle, it returns 0 (no possible paths).
            If the current cell is the bottom-right corner, it returns 1 (a valid path is found).
        Memoization:
            It uses a memoization table (dp) to store the number of paths from each cell to the bottom-right corner.
            If the number of paths from the current cell is already computed and stored in the memoization table, it returns the precomputed result.
        Recursion:
            It recursively explores the number of paths by moving right and down from the current cell.
            The number of paths from the current cell is the sum of paths obtained by moving right and down.
        Finally, it stores the result in the memoization table for future reference and returns the total number of paths from the current cell to the bottom-right corner.

    Main Function:
        The main function reads the number of test cases from the input file input2.txt.
        For each test case, it reads the size of the grid NN and the grid itself.
        It initializes the memoization table with -1 for each test case.
        It then calls the f function to calculate the number of unique paths.
        Finally, it writes the result to the output file output2.txt.
