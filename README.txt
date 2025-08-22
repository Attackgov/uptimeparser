===========================================
      Uptime Parser by Attack
===========================================

Description:
------------
This tool monitors the uptime and status of specific Windows services
and processes. It detects restarts, late starts (after system boot),
and missing services/processes. It is designed to run in real-time
and provides colored console output for clarity.

Features:
---------
- Admin privilege check and auto-restart with elevation.
- Monitors both Windows services and user processes.
- Tracks uptime of services and processes.
- Detects restarts and delayed starts relative to system uptime.
- Real-time console updates every second.
- Colored output for better readability:
  * Orange = service/process name
  * Green  = running/healthy
  * Red    = stopped/missing/issue detected

Monitored Targets:
------------------
By default, the program monitors the following:
- Services: dps, dnscache, sysmain, pcasvc, diagtrack, eventlog, bam
- Processes: explorer.exe

Requirements:
-------------
- Windows OS (tested on Windows 10/11)
- Admin rights (program will auto-request if not run as admin)
- Console environment (default CMD/PowerShell works)

Build Instructions:
-------------------
1. Open the project in Visual Studio (or any C++17 compatible compiler).
2. Ensure the following libraries are linked:
   - advapi32.lib
   - shell32.lib
3. Compile in x64 Release or Debug mode.

Usage:
------
1. Run the executable. If not elevated, it will request admin privileges.
2. The console will display monitored services and processes in real time.
3. Detected issues will be shown under the "Detections" section:
   - "<name> not running"
   - "<name> started after boot"
   - "<name> Restarted"

Notes:
------
- System uptime is displayed at the bottom of the console.
- The program runs continuously until manually closed.
- Console auto-refreshes every second to keep the view clean.

Author:
-------
Attack

===========================================
