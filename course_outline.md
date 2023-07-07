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
- Explain what a version control system does and why it is useful 3

#### Computing skill goals and level
- Be able to log on to the JupyterHub and create, edit, save, and upload/download files. 1
- Create formatted text in notebook cells with markdown. 1
- Create basic equations with LaTeX in notebook cells. 1
- Navigate a unix file system using shell commands. 2
- Create nd manage a git repo 3
- Manage own project w gh 3
- Collaborate w gh 4
- Be able to install and operate a scientific python distribution on your own computer. 4

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

#### Lesson Plans

##### Class 1

- Introduction and mini-lecture on computing in geoscience (10 min)
- Intro to course and syllabus (10)
- Intro to notebooks (5)
- Ex: log on to J-hub; sort out any issues (5)
- Overview of the Lab environment: file browser, tools, tabs window (5)
- Overview of J notebooks (5)
- Open daily notebook and do exercise of name, date, note to self about the Python print() function, and hello world (5)
- Live guided exercise on LaTeX math, with inline ($g=9.8$ meters per second squared) ($\pi$), own line ($$A_c = \pi r^2$$, $$A_s = 4 \pi r^2$$) (10)
- Mini-lecture on geologic time by powers of ten (10)
- Wrap up and recap (5)

##### Class 2

- Motivating example and mini-lec on planetary temperature; take notes in a markdown cell(s) with latex math in today's notebook. Part 1: energy balance in words and formula for power input rate. (10)
- Intro to operators: enter numbers for 3.1416 * 6370 ** 2; get someone to identify the units; explain what operators are, and operator precedence; little ex on use of parens; interpreted versus compiled (10)
- Part 2: blackbody radiation and S-B law (10)
- Solar irradiance: exercise in downloading data, uploading it to hub (5)
- Guided exercise on unix shell commands: introduce pwd, ls, cd , .. and ., mkdir, mv, cp, cat, more. (5)
- Then have them create a directory for the solar irradiance data, move the file into it, and use cat or more to look at the values. What's a typical value? (10)
- How computers represent data; RAM and storage; bits and bytes; binary numbers with example of earth radius in km, pCO2 in ppm, density of quartz. (10)
- Guided live ex: how many binary digits needed for 100 ky, 10 my, 1 Gy? (5)
- Guided exercise: python import statement, and use of math log2 and floor functions (5)
- Wrap up and assignment (5)

#### Materials

- Slides and/or notes and/or Jbook
  - Intro to course
  - Geologic time by powers of 10
  - Planetary temperature & bb rad
  - Binary representation
- In-class workbooks
  - Day 1
  - Day 2
- Assignment 1


### Python basics

#### Scientific concept goals and level
- Define greenhouse gas and greenhouse effect 1
- Explain the faint young sun concept 1
- Combine the Stefan-Boltzmann law with incoming solar energy to solve for earth's equilibrium radiating temperature 2