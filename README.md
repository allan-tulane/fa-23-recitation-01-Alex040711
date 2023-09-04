[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11681067&assignment_repo_type=AssignmentRepo)

# CMPS 2200  Recitation 01

**Name (Team Member 1):**_________________________
**Name (Team Member 2):**_________________________

In this recitation, we will investigate asymptotic complexity. Additionally, we will get familiar with the various technologies we'dll use for collaborative coding.

To complete this recitation, follow the instructions in this document. Some of your answers will go in this file, and others will require you to edit `main.py`.

## Install Python Dependency

We need Python library of "tabulate" to visualize the results in a good shape. Please install it by running 'pip install tabulate' or 'pip install -r requirements.txt' in Shell Tab of Repl.

## Running and testing your code

- To run tests, from the command-line shell, you can run
  + `pytest test_main.py` will run all tests
  + `pytest test_main.py::test_one` will just run `test_one`
  + We recommend running one test at a time as you are debugging.

## Turning in your work

- Once complete, click on the "Git" icon in the left pane on repl.it.
- Enter a commit message in the "what did you change?" text box
- Click "commit and push." This will push your code to your github repository.
- Although you are working as a team, please have each team member submit the same code to their repository. One person can copy the code to their repl.it and submit it from there.

## Comparing search algorithms

We'll compare the running times of `linear_search` and `binary_search` empirically.

`Binary Search`: Search a sorted array by repeatedly dividing the search interval in half. Begin with an interval covering the whole array. If the value of the search key is less than the item in the middle of the interval, narrow the interval to the lower half. Otherwise, narrow it to the upper half. Repeatedly check until the value is found or the interval is empty.

- [ ]
- [ ]
- [ ]
- [ ]

**TODO: your answer goes here**

**The worst case input value of key for linear search and binary search would be the key that is not present in the list. In this case the algorithm have to search through the entire list to determine that the key is not there.**

- [ ]

**TODO: your answer goes here**

The best case input value of the key for linear search would be the key that is at the beginning of the list, which is at index 0. The best case input value of the key for binary search would be the key that is at exactly the middle of the list.

- [ ]
- [ ]
- [ ]

**TODO: add your timing results here**


| n        | linear  | binary |
| -------- | ------- | ------ |
| 10       | 0.001   | 0.001  |
| 100      | 0.001   | 0.001  |
| 1000     | 0.021   | 0.002  |
| 10000    | 0.246   | 0.002  |
| 100000   | 2.237   | 0.004  |
| 1000000  | 23.399  | 0.010  |
| 10000000 | 227.089 | 0.014  |

- [ ]

**TODO: your answer goes here**

Yes. As the input size (n) increases, the running time of linear search also increases linearly. The running time of the binary search grow much more slowly as n increases compared to linear search.

- [ ]
  + What is worst-case complexity of searching a list of $n$ elements $k$ times using linear search? 
    **TODO: your answer goes here

    O(nk)**
  + For binary search? 
    **TODO: your answer goes here

    O(k * log(n)).**
  + For what values of $k$ is it more efficient to first sort and then use binary search versus just using linear search without sorting? 
    **TODO: your answer goes here

    In general, for larger values of n where log n is relatively small compared to n, sorting and binary search will be more efficient for larger values of k. However, for very small values of n or when log n is close to n, linear search without sorting might be more efficient for most values of k.**
