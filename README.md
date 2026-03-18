Netflix Hash Table (C++)
A C++ program that loads a Netflix dataset into a custom hash table using separate chaining for collision resolution. Users can search for any title by name and see the matching entry along with the number of comparisons required to find it.

Features

Loads a Netflix CSV dataset into a hash table at runtime
Custom hash function based on character sum of the title string
Separate chaining via linked list for collision resolution
Search by title with comparison counter to measure hash efficiency
Displays type, title, director, country, and year of release for any match


Concepts Demonstrated

Hash tables with separate chaining
Linked list node construction in C++
Dynamic memory allocation (new, NULL pointer handling)
CSV file parsing with istringstream
Structs and typedef in C++


How to Run
Online (easiest)
Paste Lab_9.cpp into onlinegdb.com, set language to C++, and upload netflix.csv as the input file.
Local (requires g++)
bashg++ -o netflix_search Lab_9.cpp
./netflix_search
Place netflix.csv in the same directory before running.

Usage
Read 6235 entries.

Enter a movie or show title (<return> to quit): Inception
Comparisons: 1
Type: Movie
Title: Inception
Director: Christopher Nolan
Country: USA
Year of Release: 2010
Press Enter on a blank line to quit.

Notes

Hash table size is set to 2089 (a prime number) to reduce clustering
The hash function sums the ASCII values of all characters in the title
Requires netflix.csv in the same directory to run
