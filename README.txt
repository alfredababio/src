Ticket Seller User Input:
Written by Alfred Ababio

	To use the user input:
	Remove the comments around the entire class, in Eclipse it is done easily, but pressing Ctrl + A to highlight the class, and then pressing Ctrl + / or Ctrl + 7 to remove the "//" characters.
	Afterwards run the main method in the ConsoleInput class.
	
	It requires Viera's Java Power Tools Jar
	It can be acquired at (http://www.ccs.neu.edu/home/vkp/2510-sp13/jpt.jar)

** The assignment is not clear whether or not you should initialize the Console TicketSales with the files given. I put them in to be safe. If you would like to test my Console without reading them in, don't be afraid to edit the main method and comment them out. You'll find it still works.

-------------------------------------------------------------
-----------------------PLEASE READ---------------------------
-------------------------------------------------------------
Also, I lose two style points for indentation on lines that are correctly indented. I changed the indentation to the one webcat tells me to, and it still won't give the points and say that the previous indentation was correct.
--------------------------------------------------------------
--------------------------------------------------------------

The Console will prompt you with four options as to where you must choose one of those numbers, otherwise it will prompt you again after outputting a gentle error message.

1 - Buy a ticket
	If you attempt to buy a ticket, the system will first check if there are shows. If there are shows, then it will display all of the shows and then prompt to buy  one of them. After you select a show, it will run through each ticket and ask how many you would like to buy. At the end of the tickets, it will then check if there are enough tickets to fill the order. If there are, it will print your receipt, if there is not, it will print that the theater was not able to fulfill the order because the customer requested x more tickets than are left.
	Successfully purchasing a ticket will also save the order

2 - Request a sales report
	If you request a sales report, it will print out in the correct format all of the orders and their total revenue since the initialization of the cinema.

3 - Request a manager report
	If you request a manager report, it will print out in the correct format and update the number of reports requested and add the newly generated report to the log in the TicketSales class, so it can be read after a new report is requested.

4 - Initialize Data
	1: Movie
		-Will prompt you for a Movie name and use that name.
		-Will prompt you for a Movie length (must be a natural number)
		Note: Will add duplicate movies, because in real life we could possibly have
		a movie with the same name and coincidently same length, although unlikely, it 			could happen.
	2: Theater
		-Will prompt you for a Theater name and use that name.
		-Will prompt you for a Theater maximum capacity (must be a natural number)
		Note: Will add duplicate theaters, because in real life we could possibly have
		a theater with the same name and coincidently same theater capacity, although 
		unlikely and confusing, it could happen.
	3: Showing
		-Will display a list of the movies in the database and prompt the user to choose 			one. (Number must be one displayed or it will prompt you again for one that is)
		-Will display a list of the theaters in the database and prompt the user to choose
		one. (Number must be one displayed or it will prompt you again for one that is)
		-Asks for a start time in hours (0 - 23) will enforce the range
		-Asks for a start time in minutes (0 -59) will enforce the range
		This will then create the Showing that corresponds to the user's choices and check 		if it already exists. (Can't have duplicate showingss.) If it already exists it won't add 		it, otherwise it will add it with no problems.
	4: Ticket
		-Will prompt for a ticket name
		-Will prompt for a ticket price (must be a positive number) we can have $0 tickets, 	
		they're called "free"
		Also, will not add a duplicate Ticket as this may confuse the user.

0 - Exit
	Will send a system call to exit the program.