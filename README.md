# slstatus - Suckless Status Bar (Carson's Build)
Status monitor for window managers that use WM_NAME or stdin to fill the status bar. Original repo can be found here: https://git.suckless.org/slstatus.

# Changes

## Status Fields Added
- **Master Volume Percentage:** Shows the current volume of the Master channel as a percentage. Accomplishes this by utilizing the 'run_command' function on a command that pipes amixer output into an awk script.
- **Percentage of Disk Space Used:** Shows the current percentage of disk space used (runs the disk_perc function provided and passes in '/' as the disk mount point).
- **Battery Percentage:** Shows the percentage of battery charge (runs the battery_perc function and passes in 'BAT0' as the batter name - this may change on different machines).
- **Current Date:** Shows the current day of week, month, day, and time (runs the datetime function, passing in a format string).
