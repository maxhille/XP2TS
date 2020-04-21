# XP2TS
Connects IVAO Altitude & X-Plane with Teamspeak2 on Linux systems

## Overview
This plugin listens to changes in your plane's COM frequencies and uses data from IVAO and your local Altitude config to switch Teamspeak2 to the correct channels

## Installation

- a. Install the [PythonInterface Plugin]
- b. Put the PI_XP2TS.py Script into the ./Resources/plugins/PythonScripts folder
- c. Now modify the PI_XP2TS.py file:
	search for all occurences of "/home/mh" and replace with the correct paths for you
- d. The line where is says tsControl/ts2-wrap point to the executable used for remove controlling Teamspeak2. I use a wrapper script because using TS2 via wine was much easier than the original Linux version. You can find the script also in this repository.

## ToDo
- I'm not quite sure weather the swap to Channels with 8.33kHz will work always. As X-Plane does only provide 2 decimals. 120.175 e.g. is transmitted as 120.17. In that case I match every frequence from 120.16 to 120.18. The closest open ATC Station that matches the frequency will be connected in TS2.

## Credits
The original Contributor of the Source is Enrico Gallesio who did an incredible work. 
