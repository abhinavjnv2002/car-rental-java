<h1>Car Rental System</h1>

## Description

This Car Rental System allows users to rent and return cars. The system keeps track of available cars, customer details, and rental transactions. It provides an interactive menu for users to perform these operations.

## Features

- Rent a car
- Return a car
- Display available cars
- Calculate total rental price based on the number of rental days

## Usage

### Initialize System:

1. Create an instance of `CarRentalSystem`.
2. Add predefined `Car` objects to the system.

### Menu Display:

Display the main menu with options to:
- Rent a Car
- Return a Car
- Exit

### Handle User Choice:

#### If the user chooses to Rent a Car:

1. Prompt the user to enter their name.
2. Display a list of available cars.
3. Prompt the user to enter the ID of the car they want to rent.
4. Prompt the user to enter the number of days for the rental.
5. Create a new `Customer` object with a unique ID and the provided name.
6. Add the customer to the system.
7. Find the selected car by ID and check if it's available.
8. If the car is available:
   - Calculate the total rental price.
   - Display the rental information:
     - Customer ID
     - Customer Name
     - Car details
     - Rental Days
     - Total Price
   - Ask the user to confirm the rental.
   - If confirmed, mark the car as rented and add a new `Rental` to the system.
9. If the car is not available or the ID is invalid, display an error message.

#### If the user chooses to Return a Car:

1. Prompt the user to enter the ID of the car they want to return.
2. Find the car by ID and check if it's rented.
3. If the car is rented:
   - Find the corresponding rental and customer.
   - Mark the car as available.
   - Remove the rental from the system.
   - Display a success message.
4. If the car is not rented or the ID is invalid, display an error message.

#### If the user chooses to Exit:

Terminate the program.

### Repeat Menu:

Continue displaying the menu and handling user choices until the user chooses to exit.
