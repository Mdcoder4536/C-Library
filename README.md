# C-Library
A fully functional online library that allows users to view the book collection and check a book in or out of the library.


Author: Mohamed Dahir

Purpose: This program allows a user to print all the books in the libary to the screen, check a book in our out, or close the program. 
Through a sever the user is able to send requests to the server to get the needed information. 
The server then handles the requests, then sends a response that allows
client to follow through with whatever the user requested


Header files: 
defs.h contains all forward refrences, structure definitions and libraries used

Source files:
books.c contains all book manipulation functions

lib.c contains the library manipulation functions

server.c contains all server functionality 

client.c contains all client functionality

connect.c contains all the basic TCP/IP socket communication functions needed for this program

booksData.txt contains all the book data that will be copied to the book list

Makefile contains the compilation and linking commands



Compilation and Launching instructions:
To compile the program, untar the tar file and type the command
"make". This handles both the compiling and linking of the source files to create two executables.

To run the program, first run the executable server by typing "./server" in 
the terminal. The server will load the book list and then wait for a connection from a client.
Next, open another terminal and type "./client" to run a client program that will take in the user input.
Once the client executable is run, the server will establish a connection, and the client will give the user
menu options to interact with the library.
