# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?

Some things that I learned through this assignment was the way that we can benefit from certain search algorithims and how we can appropriently use them when needed. Backtracking was one of the hardest things that I had to figure out because it can be a lot of work since you have to think about what number is going to be placed in a certain location and then you have to worry about whether it does belong there or if you need to go back and change it. I also struggled on determining how to prevent the same number from being used and how to let the user know when they are placing an invalid number somewhere.


2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?

When you have to explore through a specific website to find one set solution that you are looking for, DFS would be a better choice because it would just get you to the answer that you are looking for rather than bringing to you all the extra information. If someone uses DFS then that means that they are looking for the fastest and shortest option/route to their solution. They only care about having one working solution rather than BFS which explores through all the possible solutions before coming down to one final solution. BFS takes up more storage and time which sometimes might not be convienient in some cases.



3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?

The stack class allows for new operations to be pushed to the top rather than be left behind at the bootom. So wehnever the most recent item gets added, it goes straight to the top rather than going in the bottom like the queue. The queue class allows for the newest addition to be put behind like in a line where it will go in the back after all the past items. So it will do kind of the opposite of what the stack class does. The difference between LIFO with stack is that the newest number/item/operation will get explored next, and it will complete that exploration before moving on to the next. With FIFO in queue, the oldest number/item/operation will be explored first and it wil explore all the possiblities in depth before it moves on to a new path.

