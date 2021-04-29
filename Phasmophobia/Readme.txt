There will be two types of files needed for this:
1. Scene Export from OBS
2. Lioranboard configs for the streamdecks

Since you are here, I am assuming that you followed the Lioranboard instructions and have tested it as working with the websocket.

Download all the files in this folder to your system

Preparing OBS:
To import:
Download the PhasmoOverlay.json file and put it somewhere that you can easily find and you won't delete it.
Open OBS Studio
Click Scene Collection in the top menu
Click Import
Use the three dots in the Collection Path field to open the Windows browser
Navigate to wherever you downloaded the .json file to and select it and click OK
Click Import

Click Scene Collection and you should see Phasmo in the Scene Collection list.  Select that and you should see the base overlay that I've designed.

Preparing Lioranboard:
Open the LioranBoard Receiver folder where you've been running LioranBoard from.
Look at the config.ini files and take note of the last number in the config structure.


For example:  If you have config, config1, config2 and nothing else, then rename name the downloaded files: Change config.ini to config3.ini and config1.ini to config4.ini before copying them into the receiver folder

You can then open Lioranboard Receiver and see the two new streamdecks added to your list: Phasmophobia Stream and Phasmo Names.

Phasmophobia Stream is a small controller for entering the majority of the information and Phasmo Names is for entering the ghost name.
