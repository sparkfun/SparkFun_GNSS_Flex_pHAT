!!! warning "Need Help?"
	If you need technical assistance or more information on a product that is not working as you expected, we recommend heading over to the [SparkFun Technical Assistance](https://www.sparkfun.com/technical_assistance) page for some initial troubleshooting.

	<article style="text-align: center;" markdown>
	[SparkFun Technical Assistance Page](https://www.sparkfun.com/technical_assistance){ .md-button .md-button--primary }
	</article>

	If you can't find what you need there, the [SparkFun Forums](https://forum.sparkfun.com/index.php) is a great place to search product forums and ask questions.

	!!! info "Account Registration Required"
		If this is your first visit to our forum, you'll need to create a [Forum Account](https://forum.sparkfun.com/ucp.php?mode=register) to post questions.


!!! tip "Is PyGPSClient disconnecting?"
	If PyGPSClient disconnects from the serial port after a few seconds, you probably still have the Login Shell enabled. Use 'raspi-config' to ensure: the serial port hardware is enabled; and that [the login shell is *not* accessible](https://www.raspberrypi.com/documentation/computers/configuration.html#disabling-the-linux-serial-console).


## PyGPSClient *(system wide access)*
Users could potentially make the pyGPSCLient application globally available on the Raspberry Pi; however, that is outside the scope of this document.

!!! tip
	For some tips, users can check out these recommendations on [stackoverflow](https://stackoverflow.com/a/78652149)



## PyGPSClient Dependencies
For those not interested in the GUI, but would still like to access its functionality, the libraries of the the `PyGPSClient` Python package are listed below:

- [pynmeagps](https://github.com/semuconsulting/pynmeagps) - a parser and generator for NMEA 0183 protocol messages.
- [pyubx2](https://github.com/semuconsulting/pyubx2) - a parser and generator for u-blox UBX protocol messages.
- [pyrtcm](https://github.com/semuconsulting/pyrtcm) - a parser for RTCM protocol messages.
- [pyspartn](https://github.com/semuconsulting/pyspartn) - a parser for SPARTN protocol messages.
- [pygnssutils](https://github.com/semuconsulting/pygnssutils) - a series of GNSS utility libraries, including NTRIP and SPARTN clients, an NTRIP caster and a `gnssstreamer` utility which has broadly comparable functionality to `gpsd`.
- [pyubxutils](https://github.com/semuconsulting/pyubxutils) - a series of UBX utllities.
