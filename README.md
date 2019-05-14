# TemperData

Data collected from the van

<pre>

 Col      Register     Description
------    --------     -----------
A   1       nil         Seconds since midnight
B   2       nil         Date
C   3       nil         Time
D   4       nil         Temperature from USB device
E   5      0x3100       Input Voltage
F   6      0x3101       Input Current
G   7      0x3102       Input Power
H   8      0x3104       Charging Equipment Output Voltage
I   9      0x3105       Charging Equipment Output Current
J   10     0x3106       Charging Equipment Output Power
K   11     0x310C       Discharging Equipment Output Voltage
L   12     0x310D       Discharging Equipment Output Current
M   13     0x310E       Discharging Equipment Output Power
N   14     0x3110       Battery Temperature (Probe)
O   15     0x3111       Temperature inside equipment
P   16     0x311A       Battery State of Charge
Q   17     0x3200       Battery Status
R   18     0x3201       Charging Equipment Status  (see below)
S   19     0x330C       Energy Generated Today
T   20     0x330E       Energy Generated this Month
U   21     0x3310       Energy Generated this Year
V   22     0x331B       Battery Current
W   23     0x331D       Battery Temperature
X   24     0x331E       Ambient Temperature
Y   25     0x9013       RTC-1
Z   26     0x9014       RTC-2
AA  27     0x9015       RTC-3
AB  28     Coil 2       Manual Control of the Load.   True=Manual On


Charging Equipment Status:

     D0:   1=running   0=standby
     D1:   1=fault     0=normal
  D3/D2:   00 = No Charging
           01 = Float
	   10 = Boost
	   11 = Equalization


</pre>










