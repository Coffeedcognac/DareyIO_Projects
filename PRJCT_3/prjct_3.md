# Introduction to Shell Scripting and user input
## Notes
#### What are Bash Scripts? These are a series of command like instructions that are executed in a sequenntial manner. its basically like arranging numbers in a descending or ascending order and calling them as they are arranged . The .sh extension signifies the file type for a bash script also noting to make this file executable with the `chmod +x` command (Never forget the almighty SUDO).

## Shell Scripting Syntax Elements
#### 1. Variables: We can assign or define variables using the `equal to  sign (=) ` and also Print a value using the `echo` command in a shell script.
#### 2. Control flow: These are basically like conditional statements to control the flow in your scripts. Example of these are 

#### `if [ condition ]; then`
    # commands to be executed if the condition is true
#### `elif [ another_condition ]; then`
    # commands to be executed if another_condition is true
#### `else`
    # commands to be executed if none of the conditions are true
#### `fi`

#### 3 . Command Substitution: This is like assigning a variable to a command with a specific output. lets say, we will like to include in our script to datestamp a file with a particular date format. we know the command to print the present date on our terminal to be `date`.
#### See this sample; curent_date = `date %Y-%m-%d`  or `curent_date = $date (%Y-%m-%d)`
The above is asking the value for  `date` command with its format specifier to be assigned to the variable `current_date`.
Note : this can be don with backticks`` or $()

#### 4. Input and Output : In shell |Scripting we often have to make provision for human input and system output. We use the `read` command to specify that human input is required and `echo` to out put a required response which ould usually be a text . We also can input froma file using `<` and output from a file using `>`. 

#### 5. Functions: We could modularise our code in bash scripts to make it more reusable. This means you can define the  a function by grouping a set of commands and creating it as a module to be used in another scripts when needed.

#### See samples of writen scripts below



## Writing our first Shell script (commented each line)

![test first script](img/intro_commt.JPG)
![test first script](img/intro.JPG)

This script interacts with the user by prompting them to enter their name, reading the input, and then displaying a greeting message using the entered name.

## Directory Manipulation and Navigation
![test first script](img/twocommt.JPG)
![test first script](img/two.JPG)

This script creates three files, displays their initial order, sorts them alphabetically, displays the sorted order, removes the original files, renames the sorted file, and then displays the final sorted file

## File Operations and sorting
![test first script](img/3r33comt.JPG)
![test first script](img/3r33.JPG)

These comments explain each line of the script and provide context for the actions being performed.

## Working with Numbers and Calculations
![test first script](img/4ourcommt.JPG)
![test first script](img/4our.JPG)

This script demonstrates basic arithmetic operations, including addition, subtraction, multiplication, division, and modulo. Additionally, it performs more complex calculations such as raising a number to the power of 2 and finding the square root using the bc calculator. Finally, the script displays the results of all calculations.

## File Backup and Timestamping
![test first script](img/five2commt.JPG)
![test first script](img/five2.JPG)

This Script runs kepps a backup of a specified path and saves it with a name similar to the timestamp as at the time the backup was taken.
