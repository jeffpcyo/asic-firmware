File coming from : https://bitcointalk.org/index.php?topic=2346161.0

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

v1.12 :: 10/12 :: RECOMMENDED UPDATE


link / info to latest beta: https://bitcointalk.org/index.php?topic=2346161.msg27576989#msg27576989

Upgrade instructions: 
Recommended, at your current firmware, set the miner frequency at 400mhz and set your fan speed manual at 25% before flashing.
Download the custom firmware. (don't unpack it)
Flash by going to "System" -> "Upgrade" -> "Flash new firmware image" and select the custom firmware.
After flashing, check the advanced settings page and start at the lowest voltage setting and 400mhz. From there increase your frequency to see how high you can go at the lowest voltage setting.
Start tweaking some more. See the profile suggestions below.

Changes 10/12:
- Improved awesome miner / other mining managers compatibility (setting the priority was not working) 
- fix kernel log window height (saves you double scrolling...)
- added permanent antbleed fix (prevent remote control of your miner by bitmain Roll Eyes) -> for details see http://www.antbleed.com/

Changes 08/12:
- improved stability on some pools (included prohashing)
- fixed pool priority issue after a pool temporary died.
- fixed high frequency settings above 650 Mhz
- increased frequency settings to the boards max physical limits (825Mhz. Don't try this without knowing what you're doing Wink)

Changes 02/12:
- improved temperature sensor reading stability of all chains
- improved board / chain detection
- fixed an issue where the miner could hang mining the dev fee if your first pool is down
- improved awesome miner compatibility (special thanks to @funminer for beta testing)

Changes 29/11:
- seperated low hashrate and ASIC fail detection option in advanced configuration screen 
- reboot on low hashrate or high ASIC fail rate only after 3 times consecutive detection (less sensitive now)
- further improved startup stability of all chains
- further cgminer binary optimizations

Changes 28/11:
- Fixed the automatic reboot on low hashrate or high ASIC fail rate.
- updated cgminer to v4.10 (for details see: https://bitcointalk.org/index.php?topic=28402.msg17594456#msg17594456)
- improved pool switching behavior
- improved startup stability of all chains
- cgminer binary optimizations

Please update versions older then 26/11 as it can damage your D3.

Changes 26/11:
- Solved an issue where loosing your network connection for a longer period could burn out your hashing boards as the fans run at a very low RPM.

Changes 25/11 v2:
- Hashrate calculation is now according bitmain stock firmware (displayed  hashrate is ~3% higher now)
- + ~1% performance improvment by providing the work faster to the ASICs  Cool
- removed dev pool from miner status page to speed up webinterface and avoid confusion (exact dev mining details are visible in the kernel log)

Changes 25/11:
- fixed auto reboot on low hashrate / xxxx
- fixed issue where temperature readings could be wrong
- fixed fan error on some units
- improved stability
- allows for zero RPM fan (all custom fans should work now)
- increased upper limit frequency for overclocking. (not recommended though Wink)
- dev fee kicks in a bit later now after changing settings

Changes 23/11:
- way faster mining startup after changing settings / reboot
- adds the reboot on low hashrate option
- ~ 1% improvement on effective average hashrate *jeeej* 
- fixed flash upgrade speed to new versions
- added AUTO FAN profiles: 
The AUTO default profile is the one that's in since the start, the performance is more like the stock bitmain auto fan profile and the silent profile keeps things nice and quiet. Manual mode is for setting a static fan speed.

Changes 21/11:
- Firmware now based on latest Bitmain firmware (20/11/2017)
- made default bitmain voltage a bit more clear in the list.
- Applied a more silent AUTO fan profile.
- Fixed the high fan RPM at startup when using AUTO fan speed
- several webinterface fixes

Changes 20/11:
- ASIC frequency adjustable per chain
- Voltage settings adjustable per chain 
- new graphics. (You might need to clear your browser cache)
- Switching pools overhead lowered (now mines for fee every 2 hours)

Changes 18/11:
- fixes the pool priority, it will now mine on your own backup pools when your first pool goes down.
- Dev fee lowered to 1,5% (it was actually 1,66%)

Changes 17/11:
- fixes the high fan speed when switching to the dev pool and back to your main pool
- fixes the close PIC and need reboot!!! error on the original bitmain firmware
- Made the ASIC default voltage less confusing as it is now comparable to the default bitmain voltage.
- Lowered the AUTO profile fan RPM's a little bit.


know issues:
- switching pools can sometimes cause the miner to wait for work for ~5 seconds. (improved from ~10 seconds)
- loosing network connection doesn't stop the mining boards properly (this is default bitmain behavior, but I don't like it, so it will be changed in the future)


Important:
- As this firmware allows extreme overclocking / reduce fan speeds, I am not responsible for any damage to your miner. So flash at your own risk and please use the firmware wisely.
- There is a 1,5% mining fee as compensation for the effort I put into this project.