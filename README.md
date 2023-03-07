AirBnB clone
Description
This repository contains the first version of the project to build a clone of the AirBnB website.

This version implements a back-end interface (the console) to manage the program's data, and currently only utilize a file for data storage.

airbnb


Console

The console is a command line interpreter that allows the manipulation of all classes utilized by the application by making calls on the storage object defined above.

Using the console
The command interpreter can be started by running ./console.py in your terminal.

$ ./console.py
(hbnb)
To quit the console, enter the command quit, or input an EOF signal (ctr-D)

$ ./console.py
(hbnb) quit
$
$ ./console.py
(hbnb) EOF


Testing
Unittest for this progrem are defined in the test folder. To run the entire test suite simultaneously, execute the following command:

$ python3 unittest -m discover tests
Alternatively, you can specify a single test file to run at a time:

$ python3 -m unittest tests/test_models/test_engine/test_file_storage.py

Authors ✒️
Chrisvy Kouabngou - https://github.com/AngeCk98
