# Temperature Monitoring System 🌡️

Small multithreaded Python project from my Parallel & Distributed Computing course. It imulates temperature sensors, processes readings, and displays live data in the console with thread-safe synchronization.

## Features
- Random temperature generation (15–40°C) every second
- Rolling averages updated in real time
- In-place console updates (no full clears)
- Thread-safe with `RLock`, `Queue`, and `Condition`
## Objectives
- Simulate temperature sensors generating real-time readings.
- Process temperature data and compute averages.
- Display updated data on the console with proper synchronization.

## Synchronization Mechanisms Used:
1. **Locks (`RLock`)**: Ensures only one thread modifies `latest_temperatures` at a time.
2. **Queue (`Queue`)**: Thread-safe communication for sensor readings.
3. **Condition (`Condition`)**: Synchronizes access to display updates.
