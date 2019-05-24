# Human_Garden

An immersive multimedia series that combines technology and nature by artist Lani Asuncion.

## Initial
* Turn on the *SEND COMPUTER*.
* Turn on the *RECEIVE COMPUTER*.
* Make sure the Leap Motion is connected to the *SEND COMPUTER*.
* Make sure the ethernet cable connects the *SEND COMPUTER* and *RECEIVE COMPUTER*.

## SEND COMPUTER

### Network setup

* Go to the WiFi option on SEND and Create Network

<h3 align="center">
  <img height="30%" width="30%" src="https://i.ibb.co/JsgWZgF/Human-Garden-Create-Network.png"/>
</h3>


* A Network Name will be provided, do not change it, press create.

<h3 align="center">
  <img height="40%" width="40%" src="https://i.ibb.co/zPCMc0v/Human-Garden-Create-Network-Name.png"/>
</h3>

* Go to the “HumanGarden” folder on the Desktop

<h3 align="center">
  <img height="30%" width="30%" src="https://i.ibb.co/rmMFMnD/Human-Garden-Folder.png"/>
</h3>

Open the patch named “HumanGarden-v2-send-install.maxpat”

<h3 align="center">
  <img height="50%" width="50%" src="https://i.ibb.co/brDxK4P/Human-Garden-Sender-Patch.png"/>
</h3>

* Press toggle #1 to connect to the Leap Motion
* Press toggle #2 to open the data gate
* Press #3 to connect to the IP address and port specified below. The port number and IP address will not change, the IP address is hard coded to the *RECEIVE COMPUTER*.

*All toggles ON*

<h3 align="center">
  <img height="255" width="253" src="https://i.ibb.co/KWXsrmg/Human-Garden-Send-Buttons-ON.png"/>
</h3>

*All toggles OFF*

<h3 align="center">
  <img height="255" width="253" src="https://i.ibb.co/q777dy3/Human-Garden-Send-Buttons-OFF.png"/>
</h3>

## RECEIVE COMPUTER

### Network setup

 * Go to the WiFi option on *RECEIVE* and select the network created in the previous step.
 
 <h3 align="center">
  <img height="255" width="253" src="https://i.ibb.co/rbjML9w/Human-Garden-Receiver-Network.png"/>
</h3>

* Go to the “HumanGarden” folder on the Desktop of the *RECEIVE* computer

<h3 align="center">
  <img height="255" width="253" src="https://i.ibb.co/rmMFMnD/Human-Garden-Folder.png"/>
</h3>

* Open the patch named “HumanGarden-v2-receive-install.maxpat”

<h3 align="center">
  <img height="255" width="253" src="https://i.ibb.co/2yCZn1p/Human-Garden-Receiver-Patch.png"/>
</h3>

* Press toggle #1 to start the video and audio
* Press toggle #2 to receive data from the Leap Motion
* Press toggle #3 to turn on the audio
* At the bottom of the patch you can control the volume of the audio playback
* Press ESC to enter fullscreen.

*All toggles ON*

<h3 align="center">
  <img height="255" width="253" src="https://i.ibb.co/f8Tbbky/Human-Garden-Receiver-Buttons-On.png"/>
</h3>

*All toggles OFF*

<h3 align="center">
  <img height="255" width="253" src="https://i.ibb.co/h9K19SY/Human-Garden-Receiver-Buttons-Off.png"/>
</h3>

Control audio volume using the gain slider

<h3 align="center">
  <img height="255" width="253" src="https://i.ibb.co/L1nqjzL/Human-Garden-Receiver-Audio-Gain.png"/>
</h3>

## TROUBLESHOOTING

*Why are we not using WiFi?*
Using an ethernet connection will ensure the installation does not stop if there is an interruption with WiFi service.

*The video is not reacting to my hand motions?*
* Go to the pillar and hold never your hand over the sensor. Move your hand back and forth slowly. If the video is not moving proceed to option 2.
* On the SEND computer, find the HumanGarden folder and open the max patch named HumanGarden-v2-send-install.maxpat. Click the toggle labeled #1 to turn off the Leap Motion connection, the toggle X will be dark green. Then click the same toggle to turn on the Leap Motion connection, the toggle X will now be pink. Then press toggle #2 to open data gate and then press #3 to connect the patch to the RECEIVE computer. If you are still get no data from the Leap Motion, proceed to step 3.
* Disconnect the Leap Motion from the Mac Mini, wait 3-5 seconds and reconnect the Leap Motion to the Mac Mini. 

*The sensor is not responding consistently, but it is responding.*
Check to see if there is any obstruction on the sensor, i.e. grass shaving, that could be disrupting the connectivity. Also check for smudges on the sensor. Wipe down occasionally for best connectivity results. 

*I do not hear any audio, what's the deal?*
* Audio is generated when the Leap Motion is connected and a hand motion is detected. If there is no audio, check the *Audio* settings on the *RECEIVE* computer and make sure the *Audio Output* is set to HDMI and not Built-In Internal Speakers. Check your local Sound settings within System Preferences.

  *System Preferences > Sound > Output*
