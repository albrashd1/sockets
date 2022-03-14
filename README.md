# sockets
COMMANDS:
The commands that implemented is LOGIN, SOLVE, LIST, LOGOUT, and SHUTDOWN.

INSTRUCTIONS:
To run the program correctly, we should run the server first then run the client to avoid causing any crash. Then the user should enter LOGIN with the username and password separated with a space to log in. The server will check if the user is allowed to log in or not. If the user logged in correctly, then the user can enter the other commands including the LOGIN which will return that the user is already logged in. To use the solve command, the  user enter SOLVE with either (-c) with a radius separated with a space for a circle and (-r) with the two sides separated with a space for a rectangle. If the user input one space, the server will consider it as a square. For LIST command, the user can type LIST to list all the problems the user asked. The root is allowed to type LIST and LIST -all, to list the users’ information including the user. If any user is not a root try to ask for all users’ information, it will return that the user is not allowed to. For the LOGOUT, it will logout the client only, without terminating the server. For the SHUTDOWN, it will terminate the server and client as well. 

PROBLEMS AND BUGS:
There is one bug that I know so far, when the user type for example: SOLVE -c 4 5 3 1, it will not crash but the server will consider the first one as the radius and will ignore the rest. 
