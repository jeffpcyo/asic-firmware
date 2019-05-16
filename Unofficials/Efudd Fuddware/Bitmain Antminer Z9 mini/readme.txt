File coming from : https://bitcointalk.org/index.php?topic=5036968.0

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

Change log for version 2.1c and d:

 - Corrects a condition where the wrong pool was sometimes being returned to after the dev-fee cycle.
 - Added frequency tuning guide to "Miner Configuration -> Advanced Settings" page; If you do not see this, please clear your browser cache.
 - Updated the frequency selection list up to 850; this corrects an oversight for the Mini releases and allows you wild and crazy kids to try extreme (but not recommended by me!) frequencies.
 - Resolved a race condition where multiple cgminer processes could start running after setting new frequencies; I'm 99% confident this is resolved now.
 - Corrects an issue where certificates expired after 30 days resulting in a failure to mine properly; paid license users will need to re-apply their license after upgrading. This is a mandatory upgrade as 2.1(c) and earlier will stop working because of the early expiration mistake.