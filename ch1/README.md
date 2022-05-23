# Chapter 1 Notes

## Code Hygiene
The [Style Guide for Python Code](https://peps.python.org/pep-0008/) is an important reference to keep handy.

There are a couple of things to point out with regard to code hygiene:

- List imports in alphabetical order
- After imports, define functions, followed by class definitions
- Use classes when you're either
  1. trying to maintain state with global variables
  2. passing the same data structures to several functions

Here's an example of how the above applies:

![](/ch1/img/code1.png)

The main block at the bottom is used in two different ways:
1. For use from the command line: ```python scan.py```
    - The module's internal name is \_\_main__, and the main block is executed.
    - This loads functions and classes and executes the main block.
2. For use when imorting code into another program: ```import scan```
    - Doesn't execute the \_\_main__ block

## Setting Up a Python Virtual Environment
Run the following command to install the Python virtual environment:  
  ```shell
  sudo apt install python3-venv
  ```
