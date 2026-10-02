# Epic 6 - Define how offline time is calculated

## Objective: 
Establish the calculation used when the player returns after being offline.

##Issues

### 6.1 — Define Logout Timestamp
Determine what timestamp represents the beginning of offline time.

### 6.2 — Define Login Timestamp
Determine what timestamp represents the end of offline time.

### 6.3 — Define Offline-Time Formula
Essentially:
Login UTC − Logout UTC = Offline Time

### 6.4 — Define Offline Processing Order
Determine the order in which systems process elapsed offline time.
This is particularly important.
For example:
Offline Time
↓
Active Action
↓
Stamina/Hunger
↓
Stopping Condition
↓
Rest
↓
Recovery

### 6.5 — Define Offline-Eligible Actions
Determine which actions can continue offline.

### 6.6 — Define Offline-Ineligible Actions
Determine what happens when the player logs out during an action that cannot continue offline.

### 6.7 — Define Offline Processing Limits
Determine whether an offline action can process indefinitely.

### 6.8 — Define Offline Processing Results
Determine what information is generated during offline processing.

### 6.9 — Define Offline Processing Failure Handling
Determine what happens if offline processing cannot be completed normally.

### 6.10 — Document Offline-Time Processing

## Epic 6 Deliverable
A complete specification for calculating and processing the time a player spends offline.