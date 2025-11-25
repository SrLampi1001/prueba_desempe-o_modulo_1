# Aplication register for library
this is a console application, it DOES NOT have a database or any type of memory persistance, it starts with 5 registed products on the inventory variable, and allows the user to insert more.

## Functions
### add product 
-> asks the user for title (obligatory), author (optional), amount in stock (optional) and price (optional). Adds the book added to memory
### delete product 
-> asks the user for title (obligatory), and deletes the book with the title provided from memory
### update product
-> asks the user for title (obligatory), then, asks the user if update only the stock, or made a general update, if stock selected, only ask for an int number to add to the current stock, if general selected, allow the user to insert new_title(optional), new_price(optional), new_author(optional) and new_stock(optional), the ones the user insert valid data, are updated on memory
### search product
-> asks the user for a title (optional), if a title is provided, shows the book with a matching title, if no title is provided, prints on console all the books on memory
### sell product
-> asks the user for the title of the book to sell, if nothing is provided, does nothing, then asks for the amount to sell, the amount CAN be 0, but no negative, also asks for the client's name (optional) that if provided and does not exist, asks the user if it wish to create a new user with that name, if not, it does an anonymus sell or ask for valid name, finally, ask for the date, that MUST be on the dd/mm/yy format. It also shows the amount the client has spent on the library and asks the user if it desires to make a discount up to 80%.
### show 3 best seller
-> simply prints the 3 most sold books on the program, if there has not been any sell, it says it and returns to main menu
### generate sales repot
-> simply prints a sales report orded by author, the same book name may appear on the report if has been sold more than one time
### calculate profit and brute profit
-> print the profit made by the sells, and the profit if no discounts were applied
### Show all sales
-> simply prints all the sale, a sale has the book, the author of the book (In case the book is deleted from memory on the inventory, the author is keept on the sales list to get over error via trying to get an already deleted book from the inventory when creating sales report, instead, all the relevant information for a sale report is stored on the sales list), the client to which was sold, the amount sold of said book, the discount made to the sell, the total with the discount and the total without the discount.
### register a new client
-> asks the user for the name of the client, the ID which HAS to be an Integer, can be 0 but negative, and CAN be a repeated ID from other user, there's no a validation with user's ID. the clients are stored on the clients list in the program.
### show clients
-> prints all the clients, including name, ID and amount of money spent
### exit
-> allows the user to exit the program

## Observations
There may be grammatical errors on the program, also, it is imposible (unless the terminal process is interrupted by the user) to exit the program with out using the menu option. There are no error that interrupts the program execution. When selecting a print option on the menu, after the printing, it does not show the main menu again until the user press Enter (Anything the user may insert before pressing enter will not have an effect)