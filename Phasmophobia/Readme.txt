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

Phasmophobia Stream is a small controller for controlling the majority of the information into the stream overlay. 
Phasmo Names is for entering the ghost name.

There are three Trigger button commands and two stream deck change commands that you need to be aware of.

Red Check - In each of the Primary evidence buttons as Command: Trigger Button ID47 - Checks to see if there are two pieces of evidence found, marks as red any evidence that is unavailable, and then calls the Ghost Type button.

Ghost Type button - In the Red Check button as Command: Trigger Button ID49 - Checks to see if there are 3 pieces of evidence marked and determines the type of ghost and marks the other evidence as Red/Unavailable

Ghost Name (Deck) - In the Phasmo Name Stream Deck's Phasmo Control button as Command: Trigger Button ID124 - Calls the function that changes the ghost name on the stream.

Find the ID of each of these buttons and confirm that they are the same.  If they are not, update their appropriate calls.

Streamdeck changes:

Phasmo Names - In Phasmo Control - Changes to the stream deck number for Phasmo Names currently set to 2

Phasmo Control - In Phasmo Names - Changes to the stream deck number for the Phasmo Control currently set to 1
