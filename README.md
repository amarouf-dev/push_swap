# Push_swap

A sorting algorithm project written in C, developed as part of the 42 School curriculum.  
The goal of this project is to sort a list of integers using two stacks and a limited set of operations, while minimizing the number of instructions.

This project focuses on algorithm design, data structures, complexity optimization, and low-level C programming.

## Description

Push_swap sorts numbers using two stacks (A and B) and a predefined set of instructions.  
The program must output the smallest possible sequence of operations that sorts the input in ascending order. :contentReference[oaicite:0]{index=0}  

All numbers start in stack A, and stack B is empty.  
The program manipulates the stacks using only allowed operations. :contentReference[oaicite:1]{index=1}  

## Allowed Operations

- sa — swap top 2 of stack A  
- sb — swap top 2 of stack B  
- ss — sa + sb  
- pa — push from B to A  
- pb — push from A to B  
- ra — rotate A  
- rb — rotate B  
- rr — ra + rb  
- rra — reverse rotate A  
- rrb — reverse rotate B  
- rrr — rra + rrb  

If an operation is impossible, it must not crash the program. :contentReference[oaicite:2]{index=2}  

## Features

- Stack-based sorting algorithm
- Optimized instruction count
- Error handling
- Input validation
- Large input support
- Custom sorting strategy
- Memory safe implementation

## Usage

```
./push_swap numbers...
```

Example

```
./push_swap 4 2 3 1 5
```

The program prints the operations needed to sort the numbers.

Example output

```
pb
sa
ra
pa
```

## Bonus (if implemented)

Checker program:

```
./checker numbers...
```

Reads instructions from stdin and checks if the stack is sorted. :contentReference[oaicite:3]{index=3}  

Example

```
ARG="4 2 3 1"
./push_swap $ARG | ./checker $ARG
```

Output

```
OK
```

## Project Structure

```
src/
stack/
sort/
utils/
parse/

include/

Makefile
```

## Build

```
make
```

Clean

```
make fclean
```

Rebuild

```
make re
```

## Concepts Learned

- Algorithms
- Time complexity
- Stack data structure
- Memory management
- Parsing
- Error handling
- Optimization
- Low-level C programming

## Notes

This project follows the 42 subject rules  
and only allowed functions can be used.

The goal is educational and focused on algorithm efficiency.

## Author

Abdellah Marouf  
Morocco  
https://github.com/amarouf-dev
