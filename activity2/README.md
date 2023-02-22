# Activities

> The [modulo-calculator](#links) might be handy in these exercises.

## Task 1

- Refer to the following link. Discuss how open hashing works.
  https://www.cs.usfca.edu/~galles/visualization/OpenHash.html

  Answer: 
      - The simplest form of open hashing defines each slot in the hash table to be the head of a linked list. All records that hash to a particular slot are placed on that slot's linked list. The following figure illustrates a hash table where each slot points to a linked list to hold the records associated with that slot.

- Open Hashing Practice. Refer to the following link. Move each record on the left to the appropriate bin on the right.

  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Hashing/OpenHashPRO.html
- Given the following input (`4322, 1334, 1471, 9679, 1989, 6171, 6173, 4199`) and the hash function `x mod 10`, which of the following statements are true?
- [T] `9679, 1989, 4199` hash to the same value
- [T] `1471, 6171` hash to the same value
- [F] All elements hash to the same value
- [F] Each element hashes to a different value

## Task 2

- Bucket Hashing Practice. Refer to the following [link](https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Hashing/HashBucketPRO.html).
- The keys `12, 18, 13, 2, 3, 23, 5 and 15` are inserted into an initially empty hash table of length `10` using open addressing with hash function `h(k) = k mod 10` and **linear probing**. What is the resultant hash table?

Ans:
  0
  1    
  2 --- 12
  3 --- 13
  4 --- 2
  5 --- 3
  6 --- 23
  7 --- 5
  8 --- 18
  9 --- 15

  

## Task 3:

- What is the [Birthday Paradox](http://en.wikipedia.org/wiki/Birthday_problem)?

Ans: 
  - The birthday paradox refers to the counterintuitive fact that only 23 people are needed for that probability to exceed 50%.
  - In probability theory, the birthday problem asks for the probability that, in a set of n randomly chosen people, at least two will share a birthday.

- Why is it generally discussed with hashing?
Ans: 
  - Hashing algorithms can be used to authenticate data.

- In a hash table of 9658 slots, what is the smallest number of records that must be inserted for the probability of a collision to be 61% or more? Use the calculator at this [link](https://opendsa-server.cs.vt.edu/ODSA/AV/Hashing/Birthday.html)
- Discuss in groups how the following program works `./src/birthday.cpp`?

Ans:
  - The program calculates the approximate number of people needed in a group so that the probability of at least two people having the same birthday is at least the given value, by using a mathematical formula that relates the probability to the number of people in the group.

## Task 4: Individual (at home)

- Difference between `Separate Chaining` and `Open Addressing` collision handling techniques?

  https://www.geeksforgeeks.org/open-addressing-collision-handling-technique-in-hashing/

  https://www.geeksforgeeks.org/separate-chaining-collision-handling-technique-in-hashing/

- (Bonus) Run the following program and comment on the code `./src/hashtable.cpp`

Ans: 
  - The program demonstrates the implementation of a hash table using chaining to handle collisions between keys that map to the same index. The hash function is used to compute the index for each key, and a linked list is used to store the keys at each index. The 'insertElement' method is used to insert keys into the hash table, the 'deleteElement' method is used to delete keys from the hash table, and the 'displayHashTable' method is used to display the contents of the hash table.

## Link(s)

- [modulo-calculator](https://www.calculators.org/math/modulo.php)
- [Practice Problems on Hashing](https://www.geeksforgeeks.org/practice-problems-on-hashing/)
