dmon
----


OpenBSD program for easy daemonization of any program. It will start the specified program, write it's PID to a PID file of the same name, and write all `stdout` to a log file of the same name. `dmon` will check if a PID for the program; if there a PID file it will check to see if it is still running and print the `ps aux` line if it dose instead of running a second instance.


Examples
========


Start a program as a daemon


    dmon offlineimap


Follow the log for the program


  tail -f /tmp/dmon/log/offlineimap


