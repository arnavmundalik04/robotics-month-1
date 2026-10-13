Day 14
Time: 2 hours
Start CS50P.
Focus on:
- Variables
- Conditions
- Loops
- Functions
- Lists
Append: Add items to a list.
Extend: Add items to the same list.
Remove: Remove items from a list.
Insert: takes the position where the item must be added in a list as its first argument. 
Reverse: flip the sequence of the list. 
- Dictionaries
Syntax
Spacecraft = {“Name”: “Voyager 1”, “Distance”: “163” }
If distance is not mentioned, use .get function to give out a value when distance is not mentioned. 
Link for tutorials: https://cs50.harvard.edu/python/shorts/
1. Make a csv file containing sensor data. 
2. Read it from python using the following code:
>>> import csv (This imports the built-in CSV module in python so it can work easily with csv files. 
>>> with open("Sensor Data.csv","r") as file: (This is the format to open files, “r” opens the file in read mode, “w” opens in write mode.)
...     contents = file.read() (file refers to the file that is just opened, .read() reads all the content from the file as a string. Contents: stores the data in the variable called contents.)
... print(contents): (Prints the contents)
