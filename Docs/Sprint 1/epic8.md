# Epic 8 - Define handling of long offline periods

## Objective: 
Determine how the game handles extended periods away from the game.

## Issues

### 8.1 — Define Long Offline Threshold
Determine what qualifies as "long."

### 8.2 — Define Maximum Offline Processing Period
Determine whether there is a maximum period the game processes.

### 8.3 — Define Resource Limits
Determine how Health, Mana, Stamina, and Hunger behave when limits are reached.

### 8.4 — Define Action Completion During Long Offline Periods
Determine what happens when an action completes before the player returns.

### 8.5 — Define Transition After Action Completion
Determine what happens after an offline action finishes.

### 8.6 — Define Rest During Long Offline Periods
Determine whether Rest continues indefinitely.

### 8.7 — Define Multiple State Transitions
Determine whether a character can move through multiple states while offline.
Example:
Gathering
↓
Stamina depleted
↓
Rest
↓
Stamina restored
↓
Gathering

### 8.8 — Define Maximum Offline Resource Gains
Determine whether resources can accumulate indefinitely.

### 8.9 — Create Long Offline Examples
Examples:
1 hour
8 hours
24 hours
3 days
7 days

### 8.10 — Document Long Offline Rules

## Epic 8 Deliverable
A complete specification for processing extended offline periods.