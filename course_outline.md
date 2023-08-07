# Introduction to Python Programming for Earth Scientists

## High-level concepts

There are 3 areas: programming and computing concepts, skills, and scientific concepts that motivate the development of the other two.

### Computing concepts

1. Computers and programming in general
  - How data is represented
  - How programs work
  - Version control
2. Tools
  - Unix shell navigation
  - Jupyter notebooks
  - Organizing files and folders for projects
3. Python language
  - Operators, variables, and basic data types
  - More complex data types
  - Modules and libraries
  - Functions
  - Flow control
  - Classes and objects
  - Input and output
  - Exception handling
4. Scientific Python
  - Numpy
  - Matplotlib
  - Pandas
  - Xarray
  - Scipy
5. Working with data
  - Common file formats

### Computing skills

1. Write procedural programs to perform calculations
2. Read data from a file
3. Create plots of data
4. Analyze data by performing calculations on arrays

### Scientific concepts

1. Planetary surface temperature is controlled by solar radiation, albedo, and greenhouse gases


## Modules

1. Computers and computing environments
2. Python basics
3. Functions
4. Flow control
5. Data structures
6. Input and output
7. Classes and objects
8. Plotting with Matplotlib
9. Arrays and NumPy
10. Pandas and Xarray
11. Applications

### Computing Environments

#### Computing concept goals and level
- Identify that computers use binary to represent information 1
- Transform between decimal and binary numbers 1
- Describe how computers represent integers, floating point numbers, and alphanumeric characters 1
- Describe the difference between an interpreted and compiled programming language 1
(- Explain what a version control system does and why it is useful 3)

#### Computing skill goals and level
- Be able to log on to the JupyterHub and create, edit, save, and upload/download files. 1
- Create formatted text in notebook cells with markdown. 1
- Create basic equations with LaTeX in notebook cells. 1
- Navigate a unix file system using shell commands. 2
- Use the ! operator to execute shell commands from a notebook
- Stop and start notebook kernels
(- Create nd manage a git repo 3)
(- Manage own project w gh 3)
(- Collaborate w gh 4)
(- Be able to install and operate a scientific python distribution on your own computer. 4)

#### Scientific concept goals and level
- Define solar irradiance and albedo 1
- Identify the Stefan-Boltzmann law 1
- Use the Stefan-Boltzmann law to calculate the effective radiating temperature of earth or any other planet given S0 and albedo 2

#### Exercise and assignment notes
- First practice in notebook math and markdown writing formulas for surface area of circle and sphere
- Then have them take notes in the notebook using markdown and latex as I go over incoming solar radiation and Stefan-Boltzmann law
- Have them download a file of irradiance data, and upload it to the hub
- Have them make a folder and sub-folder for their data file, and inspect its contents with cat and more, and write down a "typical" value from the file in their notebooks
- For binary, have them calculate how many binary digits are needed to represent the (integer) values 1370 (Solar contant), 10000, 100000, etc. (turns out it's floor(log2(N))) - maybe have them import math and use log2 and floor.

### Python basics

#### Computing concept and skill goals

- Use the assignment operator to create or update a variable
- Define dynamicically typed programming language
- Identify the basic data types in Python
- Determine the type of a variable
- Convert between basic data types
- Execute Python commands in an interpreter
- Use %whos to list the variables stored in the memory of the python kernel
- Collect user input using the input() command
- Describe the list, dict, tuple, and set data types; apply lists and dicts; recognize tuples and sets
- Define immutable versus mutable objects

#### Scientific concept goals and level
- Define greenhouse gas and greenhouse effect 1
- Explain the faint young sun concept 1
- Combine the Stefan-Boltzmann law with incoming solar energy to solve for earth's equilibrium radiating temperature 2



## Schedule and Lesson Plans

### Module 1: Getting started with scientific computing

#### Class 1

- Introduction and mini-lecture on computing in geoscience (10 min)
- Intro to course and syllabus (10)
- Intro to notebooks (5)
- Ex: log on to J-hub; sort out any issues (5)
- Overview of the Lab environment: file browser, tools, tabs window (5)
- Overview of J notebooks (5)
- Open daily notebook and do exercise of name, date, note to self about the Python print() function, and hello world (5)
  - Directions: make a new notebook, give it a name that includes today's date.
  - Make a text cell that has a 1st-level heading "Getting started", name, and date
  - Make a new text cell, give it a 2nd-level heading "The Python print() function", then write a note to your future self about what the function does.
  - Make a new code cell with a print("Hello, world!") and run it
- Live guided exercise on LaTeX math, with inline ($g=9.8$ meters per second squared) ($\pi$), own line ($$A_c = \pi r^2$$, $$A_s = 4 \pi r^2$$) (10)
  - Make a new text cell with the 2nd-level header "LaTeX math"
  - Write some expressions or equations, including at least one subscript, one superscript, and Greek symbol, one fraction, and one square root. Include at least one example of an inline equation, and one example of an equation on a line by itself.
- Mini-lecture on geologic time by powers of ten (10)
- Wrap up and recap (5)

#### Class 2

- Motivating example and mini-lec on planetary temperature; take notes in a markdown cell(s) with latex math in today's notebook. Part 1: energy balance in words and formula for power input rate. (10)
  - Make a title, and a heading "power from the sun"
  - Use markdown text and latex math to take notes
- Intro to operators: Enter numbers for 3.1416 * 6370 ** 2; get someone to identify the units; explain what operators are. Show some basics: 1 + 1, 3 - 1, 2 * 3, 3 / 2, 3 ** 2. What if more than one?  (10)
  - Try the calc in a code cell and see what you get
  - Try it with parens around (6370 * 2)
  - Try to put parens that give you the WRONG answer
  - Guess what 2 + 3 * 4 is, then try it
  - Try (2 + 3) * 4
  - Guess what 4 / 2 * 3 is, then try it
  - Try 3 * 4 / 2
  - Try to get the right answer to (1 + 5) / (2 * 3) (but write it in standard math without parens)
  - Conclude talking about operator precedence.
- Part 2: blackbody radiation and S-B law (10)
- Solar irradiance: exercise in downloading data, uploading it to hub (5)
- Guided exercise on unix shell commands: introduce pwd, ls, cd , .. and ., mkdir, mv, cp, cat, more. (5)
- Then have them create a directory for the solar irradiance data, move the file into it, and use cat or more to look at the values. What's a typical value? (10)
  - Write a notebook cell that lists the unix commands we reviewed and briefly says what they do
  - Do a !ls in a code cell as an example of using ! to run shell commands from a notebook
- How computers represent data; RAM and storage; bits and bytes; binary numbers with example of earth radius in km; have them to pCO2 in ppm, and density of quartz. (10)
  - In a code cell, calculate and print the 0-11 powers of 2
  - In a markdown cell, write the binary for pCO2 ppm and density of quartz; test by adding up the 1's
- Guided live ex: how many binary digits needed for 100 ky, 10 my, 1 Gy? (5)
- Guided exercise: python import statement, and use of math log2 and floor functions (5)
  - Try math.log2(2650)
  - Try math.floor(2650)
- Wrap up and assignment (5)

#### Materials

- Slides and/or notes and/or Jbook
  - Intro to course
  - Geologic time by powers of 10
  - Planetary temperature & bb rad
  - Binary representation
- In-class workbooks
  - Day 1 - they create their own
  - Day 2


### Module 2: Python Basics

#### Class 3

- Science opener: earth radiating temperature. Greenhouse effect. Radiating temperature on Mars, Venus, Mercury. (10)
- Variables. Notice that we're having to re-type numbers. Useful if you could store values for later reuse. That's what variables are. Demo: define sigma in a variable then reuse. (5)
- Assignment operator as an instruction to the computer. (5)
  - nbex: define vars for each factor in the temperature equation and use them to calculate the temperature and print it. (5)
- How does Python know whether float or int or something else? Automatic typing. type() function. (5)
- Integer, string.
  - nbex: pick one of the planets we looked at. Define a string var for the planet's name, an integer for the number (Mercury=1), and a float for the solar irradiance. Use type() to verify that each var is of the type you intended. (5)
  - Try casting S0 to an int. What happens? Cast to str, what happens? Try planet number to float. What happens?  (5)
  - Try 2 = (1 + 1). Then 2 == (1 + 1). Then result = 2 == (1 + 1). type(result) (5)
- Comparison operations and bool variables. (5)
  - Try: result == True, result is True, result is False, result is not False. Which expression evaluates to False? (5)
- Redefining. Try reusing a variable, eg sigma, so sigma = "I forgot". type(sigma). Previous contents are discarded and variable is redefined (in general, avoid doing this!). (5)
- Discovering variables in your notebook with %whos.
  - nbex: run %whos in a code cell; make a note to yourself that this is a notebook command not a Python function. (5)


#### Class 4

- String indexing.
  - nbex: epoch = "Anthropocene". len(epoch). epoch[0]. Use brackets to print the "ro" in "Anthropocene" (5)
  - try epoch[12]. Lesson: 0-based indexing. (5)
  - ranges with colon. Ex: epoch[2:7]. epoch[:2]. epoch[7:]. (5)
  - try period = "Cretaceous". Use slicing to print out the phrase 'Creta' means 'chalk'. (5)
- Recap






  


