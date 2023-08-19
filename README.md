# FM-Radio-Transmission-Data-Logger

When we went to nerd, we brought in a street light that could be controlled by its FM Radio Transmission
for field testing. The scope of that project is to design a cost-effective, safe, and reliable streetlight control
system suitable for Sri Lanka and to develop necessary prototypes and carry out reliability tests to ensure
satisfactory operation in all environmental conditions. There had been a number of solutions proposed and
tested for the purpose of controlling the streetlights. The design efforts were conducted in NERD Center as
well as in Australia by Eng. Dayantha Jayarathna.
As a result of the efforts made, a prototype has been developed for demonstration and for field trials. The
product uses the signaling system incorporated in FM Radio Transmission called Radio Data System
(RDS). Initial testing of the test circuit was conducted in Australia as well as in Sri Lanka.

![image](https://github.com/Maduranga-Dinesh/FM-Radio-Transmission-Data-Logger/assets/57862065/96d8b136-0971-4588-a2d7-4225fb8f4199)

The device can receive the time signal accurately and can activate a relay to control a lamp or a contractor.
So we could not get information about the process inside it, but we had the opportunity to create a data
logger for its field testing.
For that, we used the ATMEGA328PU microcontroller. We also mastered the RTC3231 module for
accurate timing, the SDCAD module for storing all data, and the DHT11 sensor for measuring ambient
temperature and humidity. An Arduino UNO board was used to make improvements here. We connected
the street light to a wire with the help of a relay and got the street light on or off situation.
Figure 7. Street Light Controller
13
When it is on, an electric current of street light travels through it. We also considered it as the bulb on
occasion. The time when no current flows through the bulb is considered the off state. Then no pulse is
applied to the microcontroller. The bulb turned on the RTC module at the exact time of the on and off
modes, taking into account the ambient temperature and humidity and sending the data to an SDCAD via
the SD card module. The data is stored in a CVS file format so that we can make it available to the element
chart system or any other function we want.
So this is the basic concept of the data logger. Using this we can get the above data. after upgrading this I
created it for a PCB. We used the Altiam software to create the PCB . When we designed the PCB we have
to use an ATMEGA328P chip instead of the Arduino UNO. We have to design our schematic according to
that. This design works at a maximum voltage of 5v. We use a voltage regulator circuit to reduce DC 32V
into DC 5V.
After designing the PCB we wanted to test the PCB for that we have to connect it to a 230V AC supply so
we have to use AC to DC convert
After done the enclosing process again we test our PCB by applying 230V and applying the data signal that
we get from the streetlight and saving it on the SD card in the Excel sheet.

![image](https://github.com/Maduranga-Dinesh/FM-Radio-Transmission-Data-Logger/assets/57862065/71bc0b06-f5ac-4bd1-af68-28e431db8f77)

