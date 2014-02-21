plotclock
=========

plotclock

a clock that plots time

What you need
-------------
* Lasercutter or 3D Printer

* one Arduino (e.g. uno)

* three RC-Servos Mini (e.g. Tower Pro 9g)

* one whiteboard marker, dry eerasable (e.g. WB SL DRYWIPE MARKER)

* Screws, nuts, washers M3 and a tap for cutting M3.

Assembly
--------
(see illustrations at http://wiki.fablab-nuernberg.de/w/Ding:Plotclock#Zusammenbau )

# Use the plotclock PDF file for lasercutting acrylic 3mm or 
  use the plotclock SKP file for alternative 3D-Parts.

  The blackend area in the PDF are to be engraved, not cut. This improves grip
  for the servo hubs.

# swee.stl (a wiper) for 3D printing the cap of the pen with the eraser.
  This can also be constructed from cylindrical parts.

# Some holes are 2.5mm only, cut M3 threads there.

# Assemble the servo arms. Gently adjust the counternuts so that the joints
  under the screw heads just have enough play for smooth movement.

# Load the Arduino software (check the comments).
  http://playground.arduino.cc/Code/time is used as a clock library.

# Glue a piece of cloth to the wiper with doublesided tape.

# Connect the servo signal lines to pins 2, 3, and 4 of the Arduino board.
  Employ a small daughterboard for powering the servos, if needed.

# Test drive the software without mounting servo arms.

# Complete the assembly as shown in the illustrations. Widen the holes for
  servo mounting if needed. Acrylic is brittle and easily breaks wen the
  mounting holes are to small. Only push the servo arms onto their hubs, don't
  secure them with screws! For initial calibration do not mount the resting
  clip for the wiper (danger of collision with the pen). Glue or screw the
  servo arms to the acrylic parts.

# When you connect the Arduino, it will first run a calibration routine. The
  arms move between 2 positions, which correspond to exaxtly 90° servo
  movement.

  The calibration values SERVOFAKTOR, SERVOLEFTNULL, and SERVORIGHTNULL allow
  to adjust the actual positions to the ideal ones. Please take care that the
  servos allow sufficient range and do not hit their internal end stops. If
  needed move the servo arms on the hubs.

# Finally mount the pen and wiper rest. Uncomment the #define CALIBRATION in
  the Arduino scetch or remove the line.

# Adjust the current time in the Arduino program and you are ready to go.

--

this actually is my first git project, so merging, forks etc. is still new to me and could take some time
