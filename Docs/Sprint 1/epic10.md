# Epic 10 - Create basic time-system tests

## Objective: 
Verify that everything established in Epics 1–9 actually works.

## Issues

### 10.1 — Test UTC Retrieval
Verify authoritative UTC time.

### 10.2 — Test Timestamp Storage
Verify timestamps are stored correctly.

### 10.3 — Test Timestamp Precision
Verify expected precision.

### 10.4 — Test Elapsed-Time Calculation
Test known start/end times.

### 10.5 — Test Partial Time Periods
Test seconds and fractional periods.

### 10.6 — Test Action Start/End Times
Verify action timestamps.

### 10.7 — Test Short Offline Period
Verify short offline processing.

### 10.8 — Test Long Offline Period
Verify extended offline processing.

### 10.9 — Test Offline Action Completion
Verify an action completing while the player is offline.

### 10.10 — Test Offline Action That Cannot Continue
Verify the character enters the appropriate Wait/Rest state.

### 10.11 — Test Resource Depletion
Verify offline Stamina/Hunger behavior.

### 10.12 — Test Resource Recovery
Verify offline recovery.

### 10.13 — Test Multiple State Transitions
Verify:
Action → Exhaustion → Rest
and potentially:
Action → Rest → Action
if our later rules permit it.

### 10.14 — Test Invalid Timestamps
Verify protection against bad timestamp data.

### 10.15 — Test Duplicate Offline Processing
Verify the same offline period cannot be processed twice.

### 10.16 — Test Concurrent Sessions
Verify the time system behaves correctly with multiple login attempts.

### 10.17 — Create Sprint 1 Integration Test
Run the entire time system from:
Start Action
↓
Logout
↓
Time Passes
↓
Login
↓
Offline Processing
↓
Updated Character State

### 10.18 — Document Test Results
Record the results and any issues discovered.

## Epic 10 Deliverable
A tested and verified Game Clock & Time system.