# Car Rental System

This project is a console-based Car Rental System implemented in Java. It allows users to rent and return cars, as well as view the available cars. The system keeps track of car availability and rental transactions.

## Features

- Add cars to the rental system
- Add customers to the rental system
- Rent a car to a customer
- Return a rented car
- Display all available cars
- Simple console-based menu for user interaction

## Class Descriptions

### Car

Represents a car in the rental system.

#### Properties

- `carId`: Unique identifier for the car
- `brand`: Brand of the car
- `model`: Model of the car
- `basePricePerDay`: Base price for renting the car per day
- `isAvailable`: Availability status of the car

#### Methods

- `Car(String carId, String brand, String model, double basePricePerDay)`: Constructor to initialize car details
- `String getCarId()`: Returns the car ID
- `String getBrand()`: Returns the car brand
- `String getModel()`: Returns the car model
- `double getPrice()`: Returns the base price per day
- `double calculatePrice(int rentalDays)`: Calculates the rental price based on the number of rental days
- `boolean isAvailable()`: Checks if the car is available for rent
- `void rent()`: Marks the car as rented
- `void returnCar()`: Marks the car as returned

### Customer

Represents a customer in the rental system.

#### Properties

- `customerId`: Unique identifier for the customer
- `name`: Name of the customer

#### Methods

- `Customer(String customerId, String name)`: Constructor to initialize customer details
- `String getCustomerId()`: Returns the customer ID
- `String getName()`: Returns the customer name

### Rental

Represents a rental transaction.

#### Properties

- `car`: The car being rented
- `customer`: The customer renting the car
- `days`: The number of days for which the car is rented

#### Methods

- `Rental(Car car, Customer customer, int days)`: Constructor to initialize rental details
- `Car getCar()`: Returns the rented car
- `Customer getCustomer()`: Returns the customer who rented the car
- `int getDays()`: Returns the number of rental days

### CarRentalSystem

Manages the car rental operations.

#### Properties

- `cars`: List of cars in the system
- `customers`: List of customers in the system
- `rentals`: List of rental transactions

#### Methods

- `CarRentalSystem()`: Constructor to initialize the rental system
- `void addCar(Car car)`: Adds a car to the system
- `void addCustomer(Customer customer)`: Adds a customer to the system
- `void rentCar(Car car, Customer customer, int days)`: Rents a car to a customer
- `void returnCar(Car car)`: Returns a rented car
- `void showAvailableCars()`: Displays all available cars
- `void menu()`: Displays the main menu for the car rental system

## How to Run

1. Clone the repository or download the source code.
2. Open the project in your preferred IDE (e.g., VS Code, Eclipse, IntelliJ IDEA, NetBeans).
3. Run the `Main` class to start the car rental system.
4. Follow the on-screen instructions to interact with the system.

## Example Usage

1. **Show Available Cars**: View all cars that are currently available for rent.
2. **Rent a Car**: Enter your name, select a car by its ID, and specify the number of rental days.
3. **Return a Car**: Enter the car ID to return the rented car.
4. **Exit**: Exit the car rental system.

## Author

- Created by Gourab Roy
