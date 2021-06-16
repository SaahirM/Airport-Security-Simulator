# Airport Security Simulator

- Author: Saahir Monowar (@SaahirM)
- Upload date: 17-Apr-2021

## Desc

AirportSecuritySim.java is the main program that uses the Passenger, Bag and ScreeningStation objects. Program takes specific console input with information about how many screening stations there are, how many passengers are coming, when they're coming, how many bags they're bringing and whether these bags need to be screened (which delays the screening stations). The program then simulates the rounds, and prints key events to the console.

## Input format details

Program assumes valid input, and doesnt verify anything

### Sample input

Input looks like this:

```
5	1 2 3 4 5
4
1 FirstPerson 1 false
3 SecondPerson 0 ThirdPerson 0 FourthPerson 1 true
0
1 FifthPerson 2 true false
```

[Click here](https://github.com/SaahirM/Airport-Security-Simulator/blob/main/README.md#output-for-sample-input) for its corresponding output

### Sample input explanation

1) First line: No. of Screening stations, followed by each station's (unique) ID number
1) Second line: No. of rounds "n" when a passenger is going to enter the Airport
1) n lines afterward: No. of passengers walking in, followed by a combo of 
	- Passenger name 
	- number of bags they're bringing 
	- true/false for each bag, explaining whether the bag has to be screened. 		For every bag that needs to be screened, the passenger is delayed 		one round

## Output information

Program prints to console when an event occurs. Events are:
- When a passenger enters a station
- When a passenger leaves a station

### Output format

When a passenger leaves or enters a station, the following is print to the console:

```
PassengerName(#Bag) enters/leaves station St# in round Rn#
```

Where:
- **PassengerName** is the name of the passenger the event is focused on
- **#Bag** is the number of bags the passenger has
- **St#** is the Station number
- **Rn#** is the round in which the event occured

### Output for Sample Input

Here's the output for the [sample input](https://github.com/SaahirM/Airport-Security-Simulator/blob/main/README.md#sample-input) introduced earlier:

```
FirstPerson(1) enters station 1 in round 1
FirstPerson(1) leaves station 1 in round 1
SecondPerson(0) enters station 1 in round 2
ThirdPerson(0) enters station 2 in round 2
FourthPerson(1) enters station 3 in round 2
SecondPerson(0) leaves station 1 in round 2
ThirdPerson(0) leaves station 2 in round 2
FourthPerson(1) leaves station 3 in round 3
FifthPerson(2) enters station 1 in round 4
FifthPerson(2) leaves station 1 in round 5

```
