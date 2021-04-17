# Airport Security Simulator

- Author: Saahir Monowar (@SaahirM)
- Upload date: 16-Apr-2021

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

### Sample input explanation

1) First line: No. of Screening stations, followed by each station's (unique) ID number
1) Second line: No. of rounds "n" when a passenger is going to enter the Airport
1) n lines afterward: No. of passengers walking in, followed by a combo of 
	- Passenger name 
	- number of bags they're bringing 
	- true/false for each bag, explaining whether the bag has to be screened 
