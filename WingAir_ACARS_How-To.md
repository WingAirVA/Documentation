# W i n g  A i r
### Installing and Using our ACARS system.
#### Aircraft Communications Addressing and Reporting System
## BlackBox
We are using [Barry's BlackBox](http://barryballantines.github.io/BarrysBlackBox/) to track our flights. It is a fantastic tool. With it you can:

 * Download your bid/flight from our database.
 * Get current weather and send it to FlightGear.
 * Get the route and Download it to your aircraft FMC.
 * Submit and update flight status/information in "realtime".
 * File a **PIREP**.

## Requirements

 1. Oracle **[JAVA JRE 8](https://www.oracle.com/technetwork/java/javase/overview/index.html)** (JAVA SE 11). (*It has to be Oracacle Java JRE, not JDK nor OpenJDK/JRE*).
 2. **[BlackBox](https://github.com/barryballantines/BarrysBlackBox/releases)**.
 3. BlackBox protocol for FlightGear. (blackbox.xml)

## Installing

 1. Download and install the JRE if you don't already have it.
 2. Download BlackBox **.jar** file from step 2 above and place it somewhere.
 3. Donload BlackBox **.xml** file and place it in the **Protocols** folder ofr your FlightGear.

## Running/Configuration

 1. You will have to add a few arguments to the fgfs (FlightGear) default command line. instead of the regular `fgfs` it will be `--httpd=5500 --generic=socket,out,2,localhost,5555,udp,blackbox`.
 2. That been done, you can open BlackBox, on Windows you can likely simple double click `blackbox.jar` file. On Linux you can launch it by doing something similar to this `jre1.8.0_181/bin/java -jar blackbox-1.7.jar`.
 3. In the **Configuration** tab use `http://wing.megaf.info/action.php/kacars_free` for kACARS URL.
 4. In the **Configuration** tab use your WNG pilot ID and your password, the same that shows in our site.
 5. Click/Enable the two selection boxes, on for password and the other for the live update.

## Flying

 1. Repeat step 1 above.
 2. Repeat step 2 above.
 3. In BlackBox click **"Connect"** icon (first button), to connect BlackBox to our system and start submiting your location and status.
 4. If you have selected a big on our website, you can press the button download bid to download it.
 5. You have to start from a gate, engines off, no fuel, no PAX. After that, you can click the button **"Start Recording"**.
 6. You can use BlackBox other features, such as, get and feed route and metar to FlightGear.
 7. Refuel, board, start engines, taxi to holding point, allign and wait, takeoff, land, taxi to gate, shut down engines, unboard,
 8. Press **"Stop Recording"** in BlackBox.
 9. Click **"Upload PIREP"** to send your flight data to the system. Add notes and or FGTracker URL at will.
 10. Disconnect BlackBox.

## Notes
 * Blackbox might show a bug/crash/stuff when you send the PIREP, before going nuts check on our site your PIREP and edit it as neede.
 * Contact me, `Megaf#6582` or `legoboyvdlp#7946` on Discord or drop us a [AIRMail](http://wing.megaf.info/index.php/Mail).
 * Please read BlackBox's [official guide](http://barryballantines.github.io/BarrysBlackBox/getting-started) as well.