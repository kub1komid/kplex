````
nano /etc/kplex.conf
````
````
# Ensure that the user running kplex has read-write permission
# for this device, which normally involves adding the user to the 'dialout'
# group on Debian-based systems.  For 4800 baud connections (Normal NMEA-0183
# connections not carrying AIS information) either comment out the baud
# specifier or change it to "baud=4800".  "direction=both" is default so is not
# strictly required. Similarly "port=10110" is default so not strictly required.
# See documentation for details on configuration
# Example configuration starts below this line
#
[serial]
filename=/dev/ttyUSB0
direction=both
baud=38400
[tcp]
mode=server
port=10110
direction=both
````
