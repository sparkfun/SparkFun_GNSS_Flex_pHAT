!!! warning "Need Help?"
	If you need technical assistance or more information on a product that is not working as you expected, we recommend heading over to the [SparkFun Technical Assistance](https://www.sparkfun.com/technical_assistance) page for some initial troubleshooting.

	<center>
	[SparkFun Technical Assistance Page](https://www.sparkfun.com/technical_assistance){ .md-button .md-button--primary }
	</center>

	If you can't find what you need there, the [SparkFun Forums](https://forum.sparkfun.com/index.php) is a great place to search product forums and ask questions.

	!!! info "Account Registration Required"
		If this is your first visit to our forum, you'll need to create a [Forum Account](https://forum.sparkfun.com/ucp.php?mode=register) to post questions.



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







RTCM Parser: https://github.com/semuconsulting/pynmeagps
API: https://www.semuconsulting.com/pynmeagps/pynmeagps.html

**Message IDs???**

---

- AAM: Waypoint arrival alarm
- ABK: AIS addressed and binary broadcast acknowledgement
- ABM: AIS addressed binary and safety related message
- ACA: AIS channel assignment message
- ACK: Acknowledge alarm
- ACN: Alert Command
- ACS: AIS channel management information source
- AIR: AIS interrogation request
- AKD: Acknowledge detail alarm condition7
- ALA: Report detailed alarm condition
- ALC: Cyclic alert list
- ALF: Alert sentence
- ALR: Set alarm state
- APA: Auto Pilot A sentence
- APB: Heading/track controller (autopilot) sentence
- ARC: Alert command refused
- BBM: AIS broadcast binary message
- BEC: Bearing and distance to waypoint - Dead reckoning
- BOD: Bearing origin to destination
- BWC: Bearing and distance to waypoint - Great circle
- BWR: Bearing and distance to waypoint - Rhumb line
- BWW: Bearing waypoint to waypoint
- CUR: Water current layer - Multi-layer water current data
- DBT: Depth below transducer
- DDC: Display dimming control
- DOR: Door status detection
- DPT: Depth
- DSC: Digital selective calling information
- DSE: Expanded digital selective calling
- DTM: Datum reference
- EPV: Command or report equipment property value
- ETL: Engine telegraph operation status
- EVE: General event message
- FIR: Fire detection
- FOO: Dummy message
- FSI: Frequency set information
- GAQ: Poll Standard Message - Talker ID GA (Galileo)
- GBQ: Poll Standard Message - Talker ID GB (BeiDou)
- GBS: GNSS satellite fault detection
- GEN: Generic binary information
- GFA: GNSS fix accuracy and integrity
- GGA: Global positioning system fix data
- GLL: Geographic position - Latitude/longitude
- GLQ: Poll Standard Message - Talker ID GL (GLONASS)
- GMP: GNSS Map Projection Fix Data
- GNQ: Poll Standard Message - Talker ID GN (Any GNSS)
- GNS: GNSS Fix Data
- GPQ: Poll Standard Message - Talker ID GP (GPS, SBAS)
- GQQ: Poll Standard Message - Talker ID GQ (QZSS)
- GRS: GNSS range residuals
- GSA: GNSS DOP and active satellites
- GST: GNSS pseudorange noise statistics
- GSV: GNSS satellites in view
- HBT: Heartbeat supervision sentence
- HCR: Heading correction report
- HDG: Heading, deviation and variation
- HDM: Heading, Magnetic
- HDT: Heading true
- HMR: Heading monitor receive
- HMS: Heading monitor set
- HRM: heel angle, roll period and roll amplitude measurement device
- HSC: Heading steering command
- HSS: Hull stress surveillance systems
- HTC: Heading/track control command
- HTD: Heading /track control
- LLQ: Leica local position and quality
- LR1: AIS long-range reply sentence 1
- LR2: AIS long-range reply sentence 2
- LR3: AIS long-range reply sentence 3
- LRF: AIS long-range function
- LRI: AIS long-range interrogation
- MOB: Man over board notification
- MSK: MSK receiver interface
- MSS: MSK receiver signal status
- MTW: Water temperature
- MWD: Wind direction and speed
- MWV: Wind speed and angle
- NAK: Negative acknowledgement
- NRM: NAVTEX receiver mask
- NRX: NAVTEX received message
- NSR: Navigation status report
- OSD: Own ship data
- POS: Device position and ship dimensions report or configuration
- PRC: Propulsion remote control status
- RLM: Return link message
- RMA: Recommended minimum specific LORAN-C data
- RMB: Recommended minimum navigation information
- RMC: Recommended minimum specific GNSS data
- ROR: Rudder order status
- ROT: Rate of turn
- RPM: Revolutions
- RRT: Report route transfer
- RSA: Rudder sensor angle
- RSD: Radar system data
- RTE: Routes
- SFI: Scanning frequency information
- SM1: SafetyNET Message, All Ships/NavArea
- SM2: SafetyNET Message, Coastal Warning Area
- SM3: SafetyNET Message, Circular Area address
- SM4: SafetyNET Message, Rectangular Area Address
- SMB: IMO SafetyNET Message Body
- SPW: Security password sentence
- SSD: AIS ship static data
- STN: Multiple data ID
- THS: True heading and status
- TLB: Target label
- TLL: Target latitude and longitude
- TRC: Thruster control data
- TRD: Thruster response data
- TRF: Transit Fix Data
- TRL: AIS transmitter-non-functioning log
- TTD: Tracked target data
- TTM: Tracked target message
- TUT: Transmission of multi-language text
- TXT: Text transmission
- UID: User identification code transmission
- VBW: Dual ground/water speed
- VDM: AIS VHF data-link message
- VDO: AIS VHF data-link own-vessel report
- VDR: Set and drift
- VER: Version
- VHW: Water speed and heading
- VLW: Dual ground/water distance
- VPW: Speed measured parallel to wind
- VSD: AIS voyage static data
- VTG: Course over ground and ground speed
- WAT: Water level detection
- WCV: Waypoint closure velocity
- WNC: Distance waypoint to waypoint
- WPL: Waypoint location
- XDR: Transducer measurements
- XTE: Cross-track error, measured
- XTR: Cross-track error, dead reckoning
- ZDA: Time and date
- ZDL: Time and distance to variable point
- ZFO: UTC and time from origin waypoint
- ZTG: UTC and time to destination waypoint









**Talkers???**

---

- AB: Independent AIS Base Station
- AD: Dependent AIS Base Station
- AG: Heading Track Controller (Autopilot): General
- AI: Mobile Class A or B AIS Station
- AN: AIS Aids to Navigation Station
- AP: Heading Track Controller (Autopilot): Magnetic
- AR: AIS Receiving Station
- AS: AIS Station (ITU_R M1371, (Limited Base Station))
- AT: AIS Transmitting Station
- AX: AIS Simplex Repeater Station
- BD: BDS (BeiDou System)
- BI: Bilge Systems
- BN: Bridge Navigational Watch Alarm System
- CA: Central Alarm Management
- CD: Digital Selective Calling (DSC)
- CR: Data Receiver
- CS: Satellite
- CT: Radio-Telephone (MF/HF)
- CV: Radio-Telephone (VHF)
- CX: Scanning Receiver
- DE: DECCA Navigator
- DF: Direction Finder
- DP: Dynamic Position
- DU: Duplex Repeater Station
- EC: Electronic Chart System (ECS)
- EI: Electronic Chart Display & Information System (ECDIS)
- EP: Emergency Position Indicating Beacon (EPIRB)
- ER: Engine Room Monitoring Systems
- FD: Fire Door Controller/Monitoring Point
- FE: Fire Extinguisher System
- FR: Fire Detection Point
- FS: Fire Sprinkler System
- GA: Galileo Positioning System
- GB: BDS (BeiDou System)
- GI: NavIC (IRNSS)
- GL: GLONASS Receiver
- GN: Global Navigation Satellite System (GNSS)
- GP: Global Positioning System (GPS)
- GQ: QZSS
- HC: Compass, Magnetic
- HD: Hull Door Monitoring
- HE: Gyro, North Seeking
- HF: Fluxgate
- HN: Gyro, Non-North Seeking
- HS: Hull Stress Monitoring
- IC: Integrated Communications System
- II: Integrated Instrumentation
- IN: Integrated Navigation
- LC: Loran C
- MP: Microprocessor Controller
- ND: Network Device
- NL: Navigation Light Controller
- P: Proprietary
- RA: Radar and/or Radar Plotting
- RC: Propulsion Machinery including Remote Control
- SA: Physical Shore AIS Station
- SC: Steering Control System/Device
- SD: Sounder, Depth
- SG: Steering Gear/Steering Engine
- SI: Serial to Network Gateway Function
- SN: Electronic Positioning System
- SS: Sounder, Scanning
- TC: Track Control System
- TI: Turn Rate Indicator
- U0: User-configured talker identifier
- U1: User-configured talker identifier
- U2: User-configured talker identifier
- U3: User-configured talker identifier
- U4: User-configured talker identifier
- U5: User-configured talker identifier
- U6: User-configured talker identifier
- U7: User-configured talker identifier
- U8: User-configured talker identifier
- U9: User-configured talker identifier
- UP: Microprocessor Controller
- VD: Doppler
- VM: Speed Log, Water, Magnetic
- VR: Voyage Data Recorder
- VW: Speed Log, Water, Mechanical
- WD: Watertight Door Controller/Monitoring Panel
- WI: Weather Instruments
- WL: Water Level Detection Systems
- YX: Transducer
- ZA: Atomic Clock
- ZC: Chronometer
- ZQ: Quartz
- ZV: Radio Update



**Proprietary???**

---

- ASHR: RT300 Roll and Pitch
- ASHRALR: Alarms
- ASHRARA: True Heading
- ASHRARR: Vector & Accuracy
- ASHRATT: True Heading
- ASHRBTS: Bluetooth Status
- ASHRCAP: Parameters of Antenna Used at Received Base
- ASHRCPA: Height of Antenna Used at Received Base
- ASHRCPO: Position of Received Base
- ASHRDDM: Differential Decoder Message
- ASHRDDS: Differential Decoder Status
- ASHRHPR: True Heading
- ASHRLTN: Latency
- ASHRMDM: Modem State and Parameter
- ASHRPBN: Position and Velocity Information
- ASHRPOS: Position
- ASHRPTT: PPS Time Tag
- ASHRPWR: Power Status
- ASHRRCS: Recording Status
- ASHRSBD: BEIDOU Satellites Status
- ASHRSGA: GALILEO Satellites Status (E1,E5a,E5b)
- ASHRSGL: GLONASS Satellites Status
- ASHRSGO: GALILEO Satellites Status (E1,E5a,E5b,E6)
- ASHRSGP: GPS Satellites Status
- ASHRSIR: IRNSS Satellites Status
- ASHRSLB: L-Band Satellites Status
- ASHRSQZ: QZSS Satellites Status
- ASHRSSB: SBAS Satellites Status
- ASHRTEM: Receiver Temperature
- ASHRTHS: True Heading and Status
- ASHRTTT: Event Marker
- ASHRVCR: Vector and Accuracy
- ASHRVCT: Vector and Accuracy
- ASHRVEL: Velocity
- FECGPATT: Attitude yaw, pitch, roll
- FECGPHVE: Heave
- FUGDP: Fugro Dynamic Positioning
- GPPADV110: Position and satellite information for RTK network operations 110
- GPPADV120: Position and satellite information for RTK network operations 120
- GRMB: DGPS Beacon Information
- GRMC: Set Sensor Configuration information
- GRMC1: Set Additional Sensor Configuration Information
- GRME: Estimated Error Information
- GRMF: GPS Fix Data sentence
- GRMH: Aviation Height and VNAV data
- GRMI: Set Sensor Initialisation Information
- GRMM: MapDatum
- GRMO: Set Output Sentence Enable
- GRMT: Sensor Status Information
- GRMV: 3D Velocity Information
- GRMW: Set Additional Waypoint Information
- GRMZ: Altitude
- INVCRES: Clear the NVM data
- INVCSTR: Start session
- INVMATTIT: ATTIT information
- INVMIMU: MEMS RAW-DATA message information
- INVMINR: Calibration status
- INVMSLOPE: SLOPE information
- INVMSTR: Session Status
- KLDS: Position, Speed, Course
- KLSH: FleetSync GNSS sentence
- KNDS: Position, Speed, Course
- KNSH: Position
- KWDWPL: Waypoint Location
- LSC: Set status/poll version
- LSR: Set status response
- LSVD: Attitude yaw, pitch, roll
- MGNWPL: Waypoint Location
- QTMCFGCNST: Sets/Gets Constellation Configuration
- QTMCFGFIXRATE: Sets/Gets Fix Interval
- QTMCFGGEOFENCE: Sets/Gets Geofence Feature
- QTMCFGMSGRATE: Sets/Gets Message Output Rate on Current Interface
- QTMCFGNMEADP: Sets/Gets NMEA Precision
- QTMCFGODO: Sets/Gets Odometer Feature
- QTMCFGPPS: Sets/Gets PPS (Pulse Per Second) Feature
- QTMCFGPROT: Sets/Gets I/O Protocol for Specified Port
- QTMCFGRCVRMODE: Sets/Gets Receiver Working Mode
- QTMCFGRSID: Sets/Gets Reference Station ID
- QTMCFGRTCM: Sets/Gets RTCM
- QTMCFGRTK: Sets/Gets RTK Mode
- QTMCFGSAT: Sets/Gets GNSS Satellite Mask
- QTMCFGSIGNAL: Sets/Gets GNSS Signal Mask
- QTMCFGSVIN: Sets/Gets Survey-In Feature
- QTMCFGUART: Configure UART Interface
- QTMCOLD: Cold Start
- QTMDEBUGOFF: Disable Debug Log Output
- QTMDEBUGON: Enable Debug Log Output
- QTMDOP: Outputs Dilution of Precision
- QTMEPE: Output Estimated Position Error
- QTMGEOFENCESTATUS: Outputs Geofence Status
- QTMGNSSSTART: Starts GNSS Engine
- QTMGNSSSTOP: Stops GNSS Engine
- QTMHOT: Hot Start
- QTMODO: Outputs Odometer Information
- QTMPL: Outputs Protection Level Information
- QTMPVT: Outputs PVT (GNSS) Result
- QTMRESETODO: Reset Odometer Distance
- QTMRESTOREPAR: Restore to Default Values after Restart
- QTMSAVEPAR: Save Configuration to Non-Volatile Memory
- QTMSRR: System Reset and Reboot
- QTMSVINSTATUS: Outputs Survey-In Status
- QTMTXT: Outputs Short Text Message
- QTMUNIQID: Query Module Unique ID
- QTMVEL: Output Velocity Information
- QTMVER: Firmware Version
- QTMVERNO: Query Firmware Version
- QTMWARM: Warm Start
- SSNHRP: Heading, Roll, Pitch
- SSNRBD: Rover Base Direction
- SSNRBP: Rover Base Position
- SSNRBV: Rover Base Velocity
- SSNSNC: NTRIP Client Status
- SSNTFM: Used RTCM Coordinate Transformation Messages
- TNLAVR: Time, yaw, tilt/roll, range for moving baseline RTK
- TNLBPQ: Base station position and quality indicator
- TNLDG: L-band corrections and beacon signal strength and related information
- TNLEVT: Event marker data
- TNLGGK: Time, position, position type, DOP
- TNLGGKx: GNSS Position Message
- TNLPJK: Local coordinate position output
- TNLPJT: Projection type
- TNLREX: Rover Extended Output
- TNLVGK: Vector information
- TNLVHD: Heading information
- UBX00: PUBX-POSITION Lat/Long Position Data
- UBX03: PUBX-SVSTATUS Satellite Status
- UBX04: PUBX-TIME Time of Day and Clock Information
- UBX05: Lat/Long Position Data
- UBX06: Lat/Long Position Data
- UBX40: Set NMEA message output rate
- UBX41: PUBX-CONFIG Set Protocols and Baudrate





- RTCM Parser: https://github.com/semuconsulting/pyrtcm
- API: https://www.semuconsulting.com/pyrtcm/pyrtcm.html


**MSM message identity prefix**

---

- 107: ('GPS', 'DF004')
- 108: ('GLONASS', 'DF034')
- 109: ('GALILEO', 'DF248')
- 110: ('SBAS', 'DF004')
- 111: ('QZSS', 'DF428')
- 112: ('BEIDOU', 'DF427')
- 113: ('NAVIC', 'DF546')

**Map of 4076_201 and 1264**

---


1264:
- 0: ('DF476', 'Cosine Coefficients')
- 1: ('DF477', 'Sine Coefficients')

4076_201:
- 0: ('IDF039', 'Cosine Coefficients')
- 1: ('IDF040', 'Sine Coefficients')


**Map of 4076_201 and 1264**

---

- DF475: ('DF474', 'DF475')
- IDF038: ('IDF037', 'IDF038')


Message definitions 1240-1264