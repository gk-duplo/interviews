# Problem Statement: Elevator System with Shortest Seek Time First (SSTF) Algorithm

## Background:

Imagine you are designing a simple control system for the elevators in a building. The building has multiple floors and several elevators. The goal is to make the elevators operate efficiently by minimizing the travel distance for each request to move to a specific floor. To achieve this, the system will use a strategy where each elevator moves to the nearest requested floor first.
Elevator States:
Current Floor or Next Floor: The current floor if the elevator is stationary, or the next floor if the elevator is moving.
Direction: The current direction of movement (up, down, or stationary).

==========================================================
## Initial State:
```json
[
  {"elevator": 0, "current_floor": 0, "direction": "stationary"},
  {"elevator": 1, "current_floor": 7, "direction": "stationary"},
  {"elevator": 2, "current_floor": 4, "direction": "stationary"}
]
```
### Request from the 9th floor.
```json
[
  {"elevator": 0, "current_floor": 0, "direction": "stationary"},
  {"elevator": 1, "current_floor": 7, "next_floor": 8, "direction": "up", dest[9]},
  {"elevator": 2, "current_floor": 4, "direction": "stationary"}
]
```
## Request from the 2nd floor.
```json
[
  {"elevator": 0, "current_floor": 0, "next_floor": 1, "dest": [2] "direction": "up"},
  {"elevator": 1, "current_floor": 7, "direction": "stationary"},
  {"elevator": 2, "current_floor": 4, "direction": "stationary"}
]
```
====================================================================
# Another Initial State
```json
[
  {"elevator": 0, "current_floor": 0, "direction": "stationary"},
  {"elevator": 1, "current_floor": 8, "next_floor": 7, "direction": "down", "dest": [2]},
  {"elevator": 2, "current_floor": 3, "direction": "stationary"}
]
```
## Request from 9th Floor
```json
[
  {"elevator": 0, "current_floor": 0, "direction": "stationary"},
  {"elevator": 1, "current_floor": 8, "next_floor": 7, "direction": "down", "dest": [2]},
  {"elevator": 2, "current_floor": 3, "next_floor": 4, "direction": "up", "dest": [9]}
]
```
## Request from 5th Floor
```json
[
  {"elevator": 0, "current_floor": 0, "direction": "stationary"},
  {"elevator": 1, "current_floor": 8, "next_floor": 7, "direction": "down", "dest": [5, 2]},
  {"elevator": 2, "current_floor": 3, "direction": "stationary"}
] 
```
