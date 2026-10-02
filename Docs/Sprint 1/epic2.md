# Epic 2 - Define how timestamps are stored

## Objective: 
Determine exactly how the game records points in time.

## Issues

### 2.1 — Identify Game Events Requiring Timestamps
Determine which game events need timestamps.
Examples:
Character creation
Login
Logout
Action start
Action completion
Action interruption
Rest start
Rest completion
Last activity
Resource update

### 2.2 — Define Timestamp Data Type
Determine what type of timestamp the game uses.

### 2.3 — Define Timestamp Precision
Ensure timestamp precision matches the requirements established in Epic 1.

### 2.4 — Define Timestamp Format
Determine the standardized representation of stored timestamps.

### 2.5 — Define Timestamp Storage Location
Determine whether timestamps belong to:
Character data
Action data
Event data
Other game objects

### 2.6 — Define Timestamp Immutability
Determine which timestamps may be changed and which should never be altered after creation.

### 2.7 — Define Timestamp Update Rules
Determine when timestamps are created or updated.

### 2.8 — Document Timestamp Standards
Create the formal timestamp specification.

## Epic 2 Deliverable
A standardized method for storing and managing all game timestamps.