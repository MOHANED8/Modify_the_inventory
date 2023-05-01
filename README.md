#Modify_the_inventory
This is a C program that maintains an inventory database of parts for a store. The program allows users to insert new parts into the inventory, search for a specific part, update the quantity of a part, and print a listing of all parts in the inventory.

The program uses an array of structures to store information about the parts, with each structure containing the part number, part name, quantity on hand, and price. The maximum number of parts that can be stored is defined as a constant called MAX_PARTS, which is set to 100.

The program starts by prompting the user to enter an operation code, which can be one of the following:

'i': insert a new part into the inventory
's': search for a specific part in the inventory
'u': update the quantity of a specific part in the inventory
'p': print a listing of all parts in the inventory
'q': quit the program
The program uses a switch statement to determine which operation to perform based on the user's input. Each operation is implemented as a separate function.

The insert function prompts the user for information about a new part and then adds it to the inventory if it doesn't already exist and the database is not full.

The search function prompts the user for a part number and then looks it up in the inventory. If the part exists, the function prints its name, price, and quantity on hand. Otherwise, it prints an error message.

The update function prompts the user for a part number and then updates the quantity on hand for that part in the inventory. If the part exists, the function prompts the user for a change in quantity and updates the database. Otherwise, it prints an error message.

The print function sorts the parts in the inventory by price and then prints a listing of all parts, including their part number, name, price, and quantity on hand.

The find_part function is a helper function used by the insert, search, and update functions to look up a part number in the inventory array. If the part is found, it returns the index of the part in the array. Otherwise, it returns -1.

The compare_parts function is used by the print function to sort the parts in the inventory by price. It takes two parts as arguments and returns -1, 0, or 1 depending on whether the first part is less than, equal to, or greater than the second part in terms of price.

The program uses the sort function from the standard library to sort the parts in the inventory based on the compare_parts function.
