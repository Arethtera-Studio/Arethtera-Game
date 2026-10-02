# Epic 1 - Define UTC as the authoritative time standard

## Objective:
Establish exactly how UTC will function as the game's universal time reference.

## Issues
### 1.1 — Define UTC as the Game's Authoritative Time
UTC is the authoritative temporal reference for the game world. Player-selected time zones determine how authoritative game time is presented to the player but do not alter the underlying game time.

All game-time calculations shall originate from UTC.
This includes, but is not limited to:
- World events
- Scheduled events
- NPC activities
- Cooldowns
- Timers
- Resource regeneration
- Daily resets
- Weekly resets
- Quest timing
- Combat timing where applicable
- Server logs
- Transaction timestamps
- Player actions requiring timestamps
- Persistent game-state calculations
The game shall not use a player's local time zone as the authoritative source for game-time calculations.

### 1.2 — Define Server Time as the Authority
The Arethtera server is the sole authority for game time. The player's device clock, operating-system clock, or client-generated time shall never establish, modify, or advance authoritative game time.

### 1.3 — Define Client Clock Behavior
The player's selected time zone determines how game time is displayed to the player. The server converts authoritative UTC game time to the player's selected time zone and provides the resulting display time to the client. The client shall not use its own device clock to determine or modify game time.

The player's selected time zone affects presentation only. It does not alter the timing of game events.

### 1.4 — Define UTC Display Format
Arethtera shall allow players to select either a 12-hour or 24-hour clock format for player-facing local time displays. UTC shall always use a 24-hour clock format. The player's clock-format preference shall affect presentation only and shall not affect authoritative game time or game mechanics.

The primary game interface shall display the authoritative Game Time (UTC) and the player's localized time simultaneously. Game Time shall be displayed above the player's localized time.

### 1.5 — Define UTC Date Format
Arethtera shall use UTC as the authoritative source for all dates. Player-facing dates shall be converted to and displayed according to the player's selected time zone. Player-facing dates shall use the Month Day, Year format. Technical dates shall use YYYY-MM-DD, and complete UTC timestamps shall use ISO 8601 format with the UTC designator Z.

The Arethtera game calendar shall be based on UTC. A new game day begins at 00:00 UTC. All players share the same game date regardless of their selected time zone. Player time zones affect only the presentation of the date and time, not the underlying game date.

### 1.6 — Define UTC Time Precision
Arethtera shall use one-second precision for authoritative game time. Game-time calculations, timestamps, timers, durations, and time-dependent mechanics shall resolve to whole seconds. Sub-second precision shall not affect game mechanics.

### 1.7 — Document the UTC Time Standard
UTC Time Standard

1. Authoritative Time Standard
Arethtera shall use Coordinated Universal Time (UTC) as the authoritative time standard for the game world.
All authoritative game-time calculations shall originate from UTC.

2. Server Authority
The Arethtera server is the sole authority for game time.
The player's:
- Device clock
- Operating-system clock
- Browser clock
- Mobile device clock
- Desktop clock
- Client-generated time
shall never establish, modify, or advance authoritative game time.

3. Player Time Zone
Each player may select a time zone for displaying game time.
The selected time zone affects presentation only.
It does not alter:
- Game time
- Game date
- Event schedules
- Timers
- Cooldowns
- Game mechanics
The server converts authoritative UTC time into the player's selected time zone for display.

4. Player Clock Format
Players may select either:
- 12-hour format
- 24-hour format
for their localized time display.
UTC shall always use the 24-hour format.
Example:
Game Time: 21:47 UTC
Your Time: 5:47 PM

or, if the player selects a 24-hour clock:
Game Time: 21:47 UTC
Your Time: 17:47

5. Game Date
The Arethtera game calendar is based on UTC.
A new game day begins at:
00:00 UTC

All players share the same game date regardless of their selected time zone.
A player's local date may differ from the game date.

6. Date Display
The player's displayed date shall correspond to their selected time zone.
The underlying game date shall correspond to UTC.
Player-facing dates shall use:
Month Day, Year

Example:
October 2, 2026

Technical dates shall use:
YYYY-MM-DD

Complete UTC timestamps shall use ISO 8601 notation with the UTC designator:
2026-10-02T21:47:32Z

7. Time Precision
Arethtera shall use one-second precision for authoritative game time.
The smallest unit of authoritative game time shall be:
1 second

Sub-second precision shall not affect game mechanics.
This allows future mechanics to modify activity and skill completion times to individual seconds.

8. Connection Loss
If a player's connection to the game server is lost, the player shall be treated as offline.
The game world and server continue operating according to normal game rules.
The client shall not assume authority over game time while disconnected.
When the player reconnects, their game state shall synchronize with the current authoritative server state.
Player Time Display
Based on our discussion, I would also document the interface requirement:
The primary game interface shall display the authoritative Game Time and the player's localized time simultaneously, with Game Time displayed above the player's localized time.

For example:
┌─────────────────────────┐
│ GAME TIME: 21:47 UTC    │
│ YOUR TIME:  5:47 PM     │
└─────────────────────────┘

This gives every player a universal reference while still allowing them to plan activities according to their own local time.

## Epic 1 Deliverable
Arethtera uses server-authoritative UTC as the universal game clock and calendar, while allowing each player to view that same game time in their selected time zone and preferred clock format.