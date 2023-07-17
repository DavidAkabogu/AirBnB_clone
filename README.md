# 0x00. AirBnB clone - The console

## Description
This is the AirBnB clone team project.
In this project, we worked on the backend of the project while interfacing it with a console application with the help of the cmd module in python.
Data (python objects) generated are stored in a json file and can be accessed with the help of the json module.

[The Command Interpreter]()
The command interpreter serves as the frontend of the web app where users can interact with the backend which was developed with python OOP programming.
The command interpreter also known as `Console` manage objects abstraction between objects and how they are stored.
The following tasks will be performed by the console:
	* Create a new object
	* Retrieve an object from a file
	* Do operations on objects
	* Destroy an object

[Storage]()
All the classes are handled by the Storage engine in the `FileStorage` Class.

## How to start it

[Installation]()
You will need to clone the repository of the project from Github. This will contain the simple shell program and all its dependencies.

`git clone https://github.com/Famous3262/AirBnB_clone.git`
After cloning the repository, change to the AirBnb directory and run the command:

`./console.py`

[Execution]()
It can work in two different modes:

Interactive and Non-interactive.

In Interactive mode, the console will display a prompt (hbnb) indicating that the user can write and execute a command. After the command is run, the prompt will appear again and wait for a new command. This can go indefinitely as long as the user does not exit the program.

`$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$`

In Non-interactive mode, no prompt will appear, and no further input will be expected from the user.

`$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$`

## Testing
All the tests are defined in the test folder.

[Documentation]()
	* Modules:
`python3 -c 'print(__import__("my_module").__doc__)'`
	* Classes:
`python3 -c 'print(__import__("my_module").MyClass.__doc__)'`
	* Functions (inside and outside a class):
`python3 -c 'print(__import__("my_module").my_function.__doc__)'`

and

`python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'`

[Python Unit Tests]()
* unittest module
* File extension `.py`
* Files and folders star with `test_`
* Organization: `models/base.py`, unit tests in: `tests/test_models/test_base.py`
* Execution command: `python3 -m unittest discover tests`
* or: `python3 -m unittest tests/test_models/test_base.py`

* To run test in interactive mode
`echo "python3 -m unittest discover tests" | bash`

* To run test in non-interactive mode

`python3 -m unittest discover tests`

## Commands
Some of the commands are:

* show
* create
* update
* destroy
* count
* all
