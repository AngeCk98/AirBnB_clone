AirBnB clone
Description
This repository contains the first version of the project to build a clone of the AirBnB website.

This version implements a back-end interface (the console) to manage the program's data, and currently only utilize a file for data storage.

airbnb

Classes
This program utilizes the following classes:

BaseModel	FileStorage	User	State	City	Amenity	Place	Review
PUBLIC INSTANCE ATTRIBUTES	id
created_at
updated_at		Inherits from BaseModel	Inherits from BaseModel	Inherits from BaseModel	Inherits from BaseModel	Inherits from BaseModel	Inherits from BaseModel
PUBLIC INSTANCE METHODS	save
to_dict	all
new
save
reload	""	""	""	""	""	""
PUBLIC CLASS ATTRIBUTES			email
password
first_name
last_name	name	state_id
name	name	city_id
user_id
name
description
number_rooms
number_bathrooms
max_guest
price_by_night
latitude
longitude
amenity_ids	place_id
user_id
text
PRIVATE CLASS ATTRIBUTES		file_path
objects						
Storage
This project supports the serialization and deserialization of simple data sets using a simple file storage mechanism. The data sets are serialized to a JSON file format for the purpose of simplicity. The program initializes an instance of FileStorage called storage every time the backend is initialized. As class instances are created, updated, or deleted, the storage object is used to register corresponding changes in the file.json.

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
