Setup
======

In this document we talk about basic setup required to get started with carnatic music. Since I use Ubuntu for most of my work, using same Ubuntu machine for my carnatic music learning. 

Physical Music keyboard
------------------------
There are wide array of music keyboards available. I did a search to find a keyboard that matches below criteria's

-	Should support MIDI via USB.
-	Affordable.
-	Easy to carry & transport.

I found two keyboards (They just fit inside a laptop bag!!),

-	Akaki LPK25
-	M-Audio Keystation Mini 32

and purchased "M-Audio" from saptaswara musicals (http://www.saptaswara.in/)


Install Ubuntu Packages
------------------------

####	JACK Audio Connection Kit
sudo apt-get install jackd

####	Control UI for JACK
sudo apt-get install qjackctl

####	MIDI sound synthesiser front-end
sudo apt-get install qsynth

####	Soundfonts that will be used by synthesiser
sudo apt-get install fluid-soundfont-gs fluid-soundfont-gm

Connect Everything
-------------------
-	Connect your keyboard & laptop. Make sure volume control is set to max in your keyboard & laptop speaker.


From ubuntu terminal,

-	type qsynth &lt;enter&gt;, Click on "Setup" button -> "Soundfonts" tab -> "Open" and select "FluidR3_GM.sf2". Click on "Ok" button once you have selected sound fonts. It will ask to get restarted to load sound fonts that we have just selected. Go ahead and restart it.
-	type qjackctl &lt;enter&gt;, Click on "Start" button to start the JACK daemon. Click on "Connect" button -> "ALSA" tab -> Connect "M-Audio" to "FLUID Synth" by dragging "M-Audio" from left pane and dropping on "FLUID Synth" in right pane.


After completing above steps, when you press a key in the keyboard, you should hear piano sound from the laptop speaker !!.