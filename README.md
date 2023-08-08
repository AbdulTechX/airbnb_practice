## Airbnb Clone Project

![airnnb](https://github.com/AbdulTechX/airbnb_practice/assets/125444167/774d34f7-2668-4645-8934-1a3d75f2972d)

## Project description
The AirBnB is Web Application, integrating database storage, a back-end API, and front-end interfacing in a clone of AirBnB.

AirBnB clone - The Console project is the first part of the AirBnB clone project where we will work on the backend of the project while interfacing it with a console application with the help of the cmd module in python.

# Console(command interpreter)

The console is a command line interpreter just like the bash shell except that it has a limited number of accepted commands that were solely defined for the usage of the AirBnB website. The console(Cammand line interpreter) serves as the frontend of the web app where users can interact with the backend which was developed wit the OOB(obejct oriented programming)

# How to start it

These instructions will get you a copy of the project up and running on your local machine for development and testing purpose

 You will need to clone the repository of the project from Github. This will contain the simple shell program and all of its dependencies.

    git clone repository

After cloning the repository you will have a folder called AirBnB_clone. In here there will be several files that allow the program to work.

* console.py: The main executable of the project, the command interpreter.

* models/engine/file_storage.py: Class that serializes instances to a JSON file and deserializes JSON file to instances

* models/engine/__init__.py: A unique FileStorage instance for the application
* models/base_model.py: Class that defines all common attributes/methods for other classes.
* models/user.py: User class that inherits from BaseModel

* models/state.py: State class that inherits from BaseModel

* models/city.py: City class that inherits from BaseModel

* models/amenity.py: Amenity class that inherits from BaseModel

* models/place.py: Place class that inherits from BaseModel

* models/review.py: Review class that inherits from BaseModel

## How to use it

The AirBnB console can run in both interactively and non interactively.

in the interactive mode the console will display a prompt (hbnb) indicating that the user can write and execute a command. After command is run, the prompt will appear again and wait for new command.it can go indefininetly as long as the user does not exit the program.


    $ ./console.py
    (hbnb) help

    Documented commands (type help <topic>):
    ========================================
    EOF  help  quit

    (hbnb) 
    (hbnb) 
    (hbnb) quit
    $

in Non-interactive mode: the console will run by piping any command  into execution of the file console.py at the command line.

    $ echo "help" | ./console.py
    (hbnb) 
    Documented commands (type help <topic>):
    ========================================
    EOF  all  count  create  destroy  help  quit  show  update

    (hbnb) 
    $

## Console Commands
The AirBnB console support the following commands:

* create
    *  Usage: create <class>

Creates a new instance of a given class. The class' ID is printed and the instance is saved to the file file.json.

* show
    * Usage: show <class> <id> or <class>.show(<id>)

Prints the string representation of a class instance based on a given id.


* destroy
    * Usage: destroy <class> <id> or <class>.destroy(<id>)

Deletes a class instance based on a given id. The storage file file.json is updated accordingly.


* all
  * Usage: all or all <class> or <class>.all()

Prints the string representations of all instances of a given class. If no class name is provided, the command prints all instances of every class.


* count
    * Usage: count <class> or <class>.count()

Retrieves the number of instances of a given class.


* update
    * Usage: update <class> <id> <attribute name> "<attribute value>" or <class>.update(<id>, <attribute name>, <attribute value>) or <class>.update( <id>, <attribute dictionary>).

Updates a class instance based on a given id with a given key/value attribute pair or dictionary of attribute pairs. If update is called with a single key/value attribute pair, only "simple" attributes can be updated (ie. not id, created_at, and updated_at). However, any attribute can be updated by providing a dictionary.

# Authors 

* AbdulAzeez Buhari <AbdulTechX>
* Khadijat Abubakar <github username>
