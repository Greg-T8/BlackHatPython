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

Issue the following command to create a new virtual environment in the directory **venv3**:
```shell
python3 -m venv venv3
```
The **-m** option specifies the module name.

Issue the following comamnd to activate the environment:
```
source venv3/bin/activate
```

The **source** command executes the command from the current shell.

You can use the **deactivate** command to deactivate the environment.

Here's a look at the directory structure when creating a new environment:

![](/ch1/img/tree.png)

Note that VS Code picks up the virtual environment and automatically activates it for you:

![](/ch1/img/codeactivation.png)


## Installing a Package
The book uses the example of installing the **lxml** pacakge. This package is used for processing XML and HTML. 
- [Python xlxml Package Info](https://pypi.org/project/lxml/)
- [lxml Project Homepage](https://lxml.de/)

Here's an example showing packaging install:

![](/ch1/img/lxmlinstall.png)

And how to verify the package installation:

![](/ch1/img/lxmlverify.png)
