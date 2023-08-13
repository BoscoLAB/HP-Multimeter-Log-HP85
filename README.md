# HP-Multimeter-Log-HP85
HP 3478A Multimeter and other Log long-therm measurements for HP85 series.

The software is programmed in HP BASIC on a HP85 / HP85B with EBTKS card. The program used the DATETIME function of the EBTKS card to display date and measurement time. For the development, an EBTKS card is needed for the time being, e.g. for the real-time clock and other functions. This enables the simple storage of the measurement data. Information about the EBTKS card is available here: http://www.fliptronics.com/EBTKS/EBTKS.html An HP-IB interface is required for communication with the multimeter.

The software is under development and more features will be added. 

The latest version is available here: https://github.com/BoscoLAB/HP-Multimeter-Log-HP85/releases

Change log:
- Version 0.2.1 Small bug fix
- Version 0.2 Added Display and Print of the maximum, minimum and average measured values.

The following devices are supported:
- HP 3455A
- HP 3456A
- HP 3478A
- HP 3457A
- HP 34401A

The following functions will come soon:
- Selection of measurement function on HP multimeter such as V DC, V AC, amps, 2Wr Ohm and 4Wr Ohm.
- Selection of an external printer.
- Saving the measured values on a drive.
- Print a graphic plot after the measurement.
- Selection of a second HP device for dual measurement of e.g. volts and amps.


How it works:
After starting the program, the HP-IB address of the HP multimeter is queried. The input is made with code 7 and address, e.g. 703 (address 03). Then the number of measuring points must be entered and the time between the measurements in milliseconds. All entries are sent to the printer. 
The current date is displayed and printed. 
Now the measurement starts with the specified number and waiting time. After completion of the measurement series, a summary is displayed and printed. The measurement is finished.


For improvement suggestions please mail to input@boscolab.de 
Thanks
