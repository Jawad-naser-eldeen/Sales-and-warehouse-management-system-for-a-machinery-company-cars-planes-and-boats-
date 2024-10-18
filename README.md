Vehicle Management System
This Python script defines a set of classes for managing vehicles (cars, planes, jetskis), customers, and their purchase history. The main components are as follows:

Vehicle Class
Represents a general vehicle with attributes:

name: Name of the vehicle.

brand: Brand of the vehicle.

model: Model of the vehicle.

year: Manufacturing year of the vehicle.

color: Color of the vehicle.

available: Availability status (True if available, False if sold).

Methods:

buy(): Marks the vehicle as sold and updates the availability status.

\\str\\(): Returns a string representation of the vehicle’s details and status.

Plans Class (inherits from Vehicle)
Specific for planes, with additional attribute:

capacity: Passenger capacity of the plane.

Overrides the \\str\\() method to include capacity.

Jetski Class (inherits from Vehicle)
Specific for jetskis, with additional attribute:

engine_type: Type of engine used in the jetski.

Overrides the \\str\\() method to include engine type.

Customer Class
Represents a customer with attributes:

name: Customer’s name.

email: Customer’s email address.

phone: Customer’s phone number.

salary: Customer’s salary.

Purchase Class
Represents a purchase transaction with attributes:

customer: The customer making the purchase.

vehicle: The vehicle being purchased.

Methods:

process_purchase(): Processes the purchase by calling the buy method on the vehicle.

\\str\\(): Returns a string representation of the purchase details.

PurchaseHistory Class
Manages the history of purchases.

history: A list to store purchase records.

Methods:

add_purchase(purchase): Adds a purchase to the history.

print_history(): Prints all purchases in the history.

Example Usage
The script creates instances of vehicles (cars, planes, jetskis) and customers, processes purchase transactions, and prints the status of all vehicles and the purchase history.
