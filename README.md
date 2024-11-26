# Power Management Automation Script

## **Overview**
A Python script that automates power management for your laptop by monitoring system usage, user engagement, and battery status.
The idea was burn as a step for smarter power management of all devices at home.
It uses collected metrics to decide whether the laptop should **hibernate**, **sleep**, or remain active. 
The goal of the script is to optimize energy efficiency while maintaining usability.

---

## **Goals**
1. Automate power-saving actions based on system and user activity.
2. Collect and analyze metrics to make intelligent decisions.
3. Provide an easy-to-customize script for individual needs.
4. Support efficient energy use by changing the state to Hibernate or Sleep.

---

## **Features**
- **Monitor System Activity**: Track CPU, disk, and network usage.
- **Detect User Engagement**: Identify idle time based on input devices and active applications.
- **Battery Awareness**: Adjust power-saving actions based on battery level and charging status.
- **Time-Based Scheduling**: Align actions with predefined active/inactive hours.
- **Idle Detection**: Dynamically decide based on system idle time.

---

## **Collected Metrics**

| **Category**         | **Metric**               | **Why It's Useful**                     |
|-----------------------|--------------------------|-----------------------------------------|
| **CPU**              | CPU usage (%)           | Detects active processes.               |
| **Disk**             | Disk I/O (bytes/sec)    | Identifies file operations.             |
| **Network**          | Network I/O (bytes/sec) | Monitors streaming or downloads.        |
| **Input Devices**    | Last input time         | Measures user engagement.               |
| **Applications**     | Active window title     | Identifies if critical tasks are running.|
| **Battery**          | Battery % and status    | Optimizes power usage based on charge.  |
| **Time**             | Current hour            | Allows for scheduling rules.            |
| **Idle Time**        | System idle duration    | Decides when to enter power-saving modes.|

---

## **How It Works**
1. **Monitor Metrics**: The script continuously collects data on system activity, user input, and battery status.
2. **Decision Logic**: Based on predefined thresholds (e.g., idle for 20 minutes, battery < 15%), it determines the appropriate action:
   - Hibernate
   - Sleep
   - Remain active
3. **Scheduled Active Hours**: Aligns with user-defined active times (e.g., no power-saving between 7 AM and 11 PM).
4. **Logging**: Records metrics and actions for debugging and review.

---


