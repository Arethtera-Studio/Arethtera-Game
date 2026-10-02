# Epic 9 - Define time-related edge cases

## Objective: 
Identify unusual situations that could cause incorrect game behavior.

## Issues

### 9.1 — Define Clock Manipulation Protection
Ensure client clocks cannot affect game calculations.

### 9.2 — Define Server Time Changes
Determine what happens if the server's system clock changes.

### 9.3 — Define Daylight Saving Time
Explicitly establish that UTC eliminates DST effects.

### 9.4 — Define Leap Years
Determine how dates crossing leap years are handled.

### 9.5 — Define Leap Seconds
Determine whether leap seconds matter to the game.

### 9.6 — Define Extremely Long Offline Periods
Determine what happens after months or years.

### 9.7 — Define Duplicate Login Processing
Prevent offline time from being processed twice.

### 9.8 — Define Interrupted Offline Processing
Determine what happens if processing fails midway.

### 9.9 — Define Database Timestamp Corruption
Determine how invalid timestamps are handled.

### 9.10 — Define Missing Timestamps
Determine what happens if a required timestamp doesn't exist.

### 9.11 — Define Negative Elapsed Time
Determine what happens if:
End Time < Start Time

### 9.12 — Define Concurrent Sessions
Determine what happens if the same account attempts to log in from multiple devices.

### 9.13 — Document Time Edge Cases

## Epic 9 Deliverable
A documented set of safeguards for abnormal time conditions.