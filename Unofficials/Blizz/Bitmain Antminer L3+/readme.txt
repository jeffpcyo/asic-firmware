File coming from : https://bitcointalk.org/index.php?topic=2694602.0

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

v1.02 :: 14/01/2018 :: L3+ recommended update


Upgrade instructions: 
Recommended, at your current firmware, set the miner frequency at 350mhz before flashing.
Download the custom firmware. (don't unpack it)
Flash by going to "System" -> "Upgrade" -> "Flash new firmware image" and select the custom firmware.
When the reboot is complete: please clear your browser cache or use ctrl + f5 if you don't see the pages  properly loaded
Then check the advanced settings page and set the global values to the lowest voltage setting and 375mhz. From there increase your frequency to see how high you can go at the lowest voltage setting.
Start tweaking some more. See the profile suggestions below.

v1.02 L3+ version 14/01/2018:
- adds power usage (Watt) indication per chain in the mining status overview. Really useful for if you don't own a wattage meter
- cleaned kernel logging when not using all the pools
- cleaned API code for faster miner status update speed.

v1.01 L3+ version 13/01/2018:
- Fixed an issue where the status page was empty on lowest voltage setting.

v1.0 L3+ version 12/01/2018:
- first stable release  Cool
- reboot (and cool down) on too high temperatures (PCB temp > 85 deg celcius)
- optional: reboot on too high ASIC fail count
- optional: reboot on detection of low hashrate (if falls down 8% under the expected hashrate)
- now shows the voltage setting on the overview page
- fixed showing high FAN speed RPM's
- added option to mine the dev fee one time a day (increases daily profit a bit in case you run it on one pool)

v0.02 L3+ version 05/01/2018:
- awesome miner support / other API tools now compatible
- fixed frequency ranges in advanced miner page

First L3+ version 05/01/2018:
- Adds unlocked voltage global or individual per chain. Saves up to 20% energy usage compared to the stock firmware. (unit runs ~500Mh/s @ ~670watt)
- Adds frequency setting per individual chain.
- cgminer update to 4.10
- Adds 3 fan profile modes
- No more high fan speed durings startup
- Faster startup time
- Cleaned up web interface
- Cleaned up kernel log
- Possible to flash back to the default firmware (see guide below)
- Possible to change the stock fans for custom fans

know issues:
- Only tested on L3+. Unsure if this runs on the a normal L3 (non plus).

Important:
- As this firmware allows extreme overclocking / reduce fan speeds, I am not responsible for any damage to your miner. So flash at your own risk and please use the firmware wisely.
- There is a 1,5% mining fee as compensation for the effort I put into this project.