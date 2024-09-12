# Elevator-Simulator-Java

## Elevator Challenge

-This project simulates the operation of an elevator system in a building using Core Java. The elevator operates based on user input and random requests. The elevator moves between floors, picks up passengers, and drops them off at their desired floors. The program demonstrates key object-oriented programming principles.
 
 ## Features
 
 This project implements a single-threaded elevator simulation. The elevator moves between floors and responds to both manual and automatic requests. The elevator is 
 designed to keep moving in the current direction (up or down) until all requests in that direction are processed. It changes direction when it reaches the top or 
 bottom floors, and it idles when no more requests exist.

 ## Prerequisites
 
 1. Java Development Kit (JDK) 8 or higher
 2. A Java IDE (IntelliJ, Eclipse, etc.) or command-line tools to compile and run Java programs

## usage

You can run the elevator simulation in two modes: manual and automatic.
Manual Mode: The user manually inputs the starting floor and the destination floor for the elevator.
Automatic Mode: The program automatically generates random floor requests for the elevator to process.

## Classes

Direction (Enum):Represents the direction of the elevator: UP, DOWN, or IDLE.
Elevator:The core class that manages the elevator’s behavior, including its current floor, direction and requests.
*Attributes*:
-currentFloor: Tracks the current floor.
-currentDirection: Tracks the elevator’s current direction.
-requestedPathsMap: A map that stores the floor requests.
-currentFloorDestinations: An array that tracks the floors where people need to deboard.
*Methods*:callElevator(): Adds a request for pickup and destination.
-processFloor(): Handles the current floor's onboarding and offboarding processes.
-moveElevator(): Moves the elevator up or down based on current requests.
-start(): Starts processing the elevator's movement based on requests.
ElevatorChallenge:The entry point of the program, where the simulation begins.
*Methods*:
-manualElevator(): Allows the user to manually input the floor requests.
-automaticElevator(): Automatically generates random floor requests.

## How it works

1.The Elevator starts at the ground floor (0) and initially moves in the UP direction.
2.The user can request the elevator from any floor to go to a destination floor.
3.The elevator processes all requests in its current direction. Once all requests are fulfilled, it changes direction (either UP or DOWN) if there are more requests in the opposite direction.
4.If no requests are left, the elevator becomes IDLE.The elevator handles onboarding and offboarding at each requested floor.
5.Manual and automatic mode allows either user controlled request or random request for the elevator.

## Future Improvements

1.Multiple Elevators: Implement support for multiple elevators
2.Weight Capacity: Add constraints to limit the number of passengers or the weight the elevator can handle at a time.
3.Priority Requests: Implement a priority system for certain floors (e.g. emergency floors or express service).

## author

Dibyani Debasmita Behera

