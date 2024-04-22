# Same code in parallel
## Why
### Parallel
Parallel refers to the condition where two or more entities, such as lines, planes, or processes, maintain an equal distance apart at all points, without intersecting or converging. In various contexts, it can denote the state of coexistence or similarity in direction, action, or development, often facilitating simultaneous or independent operations without interference. In mathematics and geometry, parallel lines never meet regardless of how far they extend, while in computing or electronics, parallel processing involves simultaneous execution of multiple tasks to enhance efficiency.

Parallel

```bash
pip install -r .\parallel.txt
```

### Option 1

Check for newer versions for installed libraries.

```bash
pip list -o
```

### Option 1A

Look for information about installed libraries, find out what they provide for the project (look particularly at the ipython library).

If we want to update all packages at once, then we can use pip-review:
```bash
pip install pip-review
```

List of all packages that can be upgraded:
```bash
pip-review
```

We can update packages interactively over time:
```bash
pip-review --local --interactive
```

All at once:
```bash
pip-review --local --auto
```

## Option 2
### Option 2A

Look in the pip library for parallel.

https://pypi.org/project/parallel/

### Option 2B

Install the pylint library in the version extracted from the previous step.

Tip To install dependencies in a specific version, you must add the == operator along with the library version in addition to the traditional installation command.
```bash
pip install parallel
```

### Exercise 2c

Search the internet and find out what you can use this library for.

### Exercise 2d

Select one of your previously created python files and check its correctness using the parallel (command: parallel <path_to_file>). If there are any suggestions, please make corrections; try until the result is 10/10.

Tip parallel will analyze the code and evaluate how it was formatted and written. In the case of bad non-Python-style names or unnecessary blank lines, the result will be worse (there are many more rules, it is worth knowing a substantial part of them). For a 10/10 result, the library considers the file to be fully valid.

## Option 3
### Option 3A

Check what libraries are currently installed on your computer; redirect the result to a file.

Tip The result of the first command can be redirected to a file using the redirection operator on operating systems: >.
```bash
pip freeze > requirements.txt
```

### Option 3B

What is the difference between the ```pip list``` and ```pip freeze``` commands? Can the formats generated by both commands be successfully used (after being redirected to a file) to install the dependency package in the new project?

Tip Try to redirect the result of both commands (pip list and pip freeze) to a file and install dependencies referring to this file. See what the commands generated.

## Option 4
### Option 4A

Uninstall the previously installed jedi library.
```bash
pip uninstall jedi
```

### Option 4B

Uninstall the other libraries you no longer need -> optional.

Tip As with the pip install command, you can use the requirements.txt file to uninstall dependencies.
