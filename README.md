Parking Lot Application
This is a simple command-line project written in Kotlin that simulates a parking lot management system. The application allows you to create a parking lot, park cars, remove them, and perform various queries on the lot's status.

🌟 Features
The application supports the following commands, which can be entered in the command line:

create <size>: Creates a parking lot with the specified number of spots.

park <reg_number> <color>: Parks a car with a specific registration number and color in the first available spot.

leave <spot_number>: Removes the car from the specified parking spot, making it free.

status: Displays the current status of the parking lot, listing parked cars by spot number.

reg_by_color <color>: Returns all registration numbers of cars of a specific color, separated by commas. The search is case-insensitive.

spot_by_color <color>: Returns all spot numbers of cars of a specific color, separated by commas.

spot_by_reg <reg_number>: Returns the spot number where a car with a specific registration number is located.

exit: Shuts down the application.

🚀 How to Run
To run this project, you need to have the Kotlin compiler installed.

Compile the code:

kotlinc Main.kt -include-runtime -d parking-lot.jar

Execute the JAR file:

java -jar parking-lot.jar

After execution, the program will enter a command loop, waiting for your input.

💻 Example Usage
Here is an example of an interaction with the application:

> create 6
Created a parking lot with 6 spots.

> park KA-01-HH-1234 White
White car parked in spot 1.

> park KA-01-HH-9999 Black
Black car parked in spot 2.

> park KA-01-BB-0001 Red
Red car parked in spot 3.

> status
1 KA-01-HH-1234 White
2 KA-01-HH-9999 Black
3 KA-01-BB-0001 Red

> spot_by_color black
2

> leave 2
Spot 2 is free.

> status
1 KA-01-HH-1234 White
3 KA-01-BB-0001 Red

> exit

🛠️ Technologies Used
Kotlin: The main programming language.

JVM: The platform on which the code is executed.
