# Epic 3 - Define how the current game time is retrieved

## Objective: 
Establish how the game obtains the current authoritative UTC time.

## Issues

### 3.1 — Define Server Time Retrieval
Determine how the game server obtains current UTC time.

### 3.2 — Define Game Time Request
Determine how the game engine requests the current time.

### 3.3 — Define Client Time Display
Determine how the browser receives and displays the current game time.

### 3.4 — Prevent Client Clock Manipulation
Define how changing the player's device clock is prevented from affecting game calculations.

### 3.5 — Define Time Synchronization
Determine how the client maintains synchronization with server time.

### 3.6 — Define Time Retrieval Failure
Determine what happens if the client cannot retrieve current server time.

### 3.7 — Define Time Retrieval Frequency
Determine whether the client:
Requests time continuously
Synchronizes periodically
Uses a server-provided timestamp and calculates locally

### 3.8 — Document Current-Time Retrieval
Document the finalized process.

## Epic 3 Deliverable
The game can reliably obtain authoritative current UTC time.