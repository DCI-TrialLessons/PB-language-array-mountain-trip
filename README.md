# The Mountain Trip

You are collecting reservations for a bus trip to the mountains.

You have a list of people interested in the trip and a list of available seats on the bus.

```javascript
const people = [
  "Dawn Greenfield",
  "Wait Lindegard",
  "Lucia Timoney",
  "Rock Thom",
  "Courtney Haryngton",
  "Afton Meugens",
  "Mata Lydiard",
  "Gene Castanie",
  "Owen Satcher",
  "Langston Benne",
  "Derk Pavlishchev",
  "Guinna Shovelbottom",
  "Clemmie Skeermor",
  "Rich Worley",
  "Isa Featherstonhaugh",
];

const seatsAvailable = ["A1", "A2", "B1", "C1", "C2", "D2", "E1", "F1", "F2"];
```

## Task 1

You have to make sure that there are enough available seats.

You have 2 arrays:
- the array `people` contains the names of the people that want to reserve a seat on the bus
- the array `seatsAvailable` contains the remaining available seats

Your first task is to:

1. get the number of people interested in the trip and assign it to a variable called `numberOfPeople`
2. get the total of available seats and assign it to a variable called `numberOfSeatsAvailable`
3. print a message to the console saying:
    - `there are X people interested in the trip and 9 available seats`
    - replace X and Y with the correct values
4. compare the 2 variables and print a message like:
    - `there are enough available seats for everyone`
    - `there are not enough available seats for everyone`

Expected output with the data provided:

```plaintext
There are 15 people interested in the trip and Y available seats
There are not enough available seats for everyone
```

## Task 2

Now that you realised that there are not enough available seats for everyone, you need to communicate to everyone whether they can join the trip or not.

You need to:
- update the list of people leaving only the ones that can join the trip
- create a second list called `peopleRejected` containing only the people that can not join the trip, due to lack of seats

Your task is:

1. calculate the difference between the number of people and the number of available seats, to know how many people won't be able to join. Assign this value to a variable called `numberOfPeopleRejected`
2. using the variable you just created, remove the number of people that can't join the trip from the original `people` array and assign this to a new array
3. assign the right values to the variables `peopleConfirmedList` and `peopleRejectedList`
    - they should contain a string with all the names in the 2 respective arrays, with each name separated by the `\n` (new line) special character

Expected output:

```plaintext
The list of people that can go on the trip is:
Dawn Greenfield
Wait Lindegard
Lucia Timoney
Rock Thom
Courtney Haryngton
Afton Meugens
Mata Lydiard
Gene Castanie
Owen Satcher

The list of people that can not go on the trip is:
Langston Benne
Derk Pavlishchev
Guinna Shovelbottom
Clemmie Skeermor
Rich Worley
Isa Featherstonhaugh
```



## Task 3

There is an extra seat available which you want to assign to a random person from the list of rejected people.

Your task is to:

1. randomly choose a name from the array `peopleRejected` and assign it to 
a variable called `luckyWinner`
2. print a message to the console saying: `PERSON will be able to join the trip`
   - replace PERSON with the name of the chosen person
