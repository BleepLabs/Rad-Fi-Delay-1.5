# Rad-Fi-Delay-1.5
Breadboard based glitchy delay using the Teensy 3.2

The rad fi delay 1.5 is an updated version of the <a href="http://bleeplabs.com/rad-fi-central/">original arduino based lo-fi glitch effect</a> released by Bleep Labs in 2015. This new version is meant as a quick breadboard or soldering project you can build right now using off the shelf parts. 
Unlike the atmega328 used in the original, this updated device uses the Teensy 3.2. This allows it to sample audio at 44.1k while still maintaining the simple glitchiness of the original. 

The Rad-Fi Delay can work just like a standard delay effect with a feedback and delay time control.
The trick is that the sample rate of the effect and other features can be controlled with digital inputs and three square wave oscillator outputs. This produces odd arpeggiated, granular sounds. 

<a href="https://docs.google.com/spreadsheets/d/1HgXk2Bo4Rd0A5V1MbUsgcbOM54Az-JnbRDxo8K8Pac8/edit?usp=sharing">Parts list</a>

<a href="https://github.com/BleepLabs/Rad-Fi-Delay-1.5/blob/master/Intro%20to%20breadboards.pdf">Getting started with breadbords guide</a>

I like these "12mm" pots on theparts list. All you need to do is remove the large tabs from the back and they fit nicely on a PCB.
Standard ones can be used instead, just move the two small wires to connect to them.

<img src="https://raw.githubusercontent.com/BleepLabs/Rad-Fi-Delay-1.5/master/pots.jpg">

There is one thing that needs soldering or at least a wire twisted tightly on it. The DAC outpt of the Teesny 3.2 is not on the noraml breadboard pins so you'll need to connect a wire to it. 

<img src="https://raw.githubusercontent.com/BleepLabs/Rad-Fi-Delay-1.5/master/DAC.jpg">

Once you get all the parts together upload the code found in the "rad_delay_1v5" folder above to the Teesny. <a href="https://www.pjrc.com/teensy/teensyduino.html">Guide here.</a>

<img src="https://raw.githubusercontent.com/BleepLabs/Rad-Fi-Delay-1.5/master/Rad-fi-delay-1v5-breadboard-layout.png">
All of the marked colums on the bottom side are digital inputs. Theyr are activated when the recieve a low signal, that is they are conencted to ground. You can mannualt use a wire to do thos or one of the oscillator outputs on the top of the Teensy. 

~~~~~~~~~~~

<i>Are you selling a kit</i>
Not right now but if you're interested sign up for this mailing list and I'll email about this only. (Sign up here for all Bleep Labs news). I threw this device together with the simplest parts possbile so anyone could get the parts they need from a variety of sources (see the <a href="https://docs.google.com/spreadsheets/d/1HgXk2Bo4Rd0A5V1MbUsgcbOM54Az-JnbRDxo8K8Pac8/edit?usp=sharing">Parts list</a>
). 

<i>Why not use the <a href="https://www.pjrc.com/teensy/td_libs_Audio.html">Audio libary</a> and board?</i>
I love Paul's audio library and have used it on my producest and even contributed to it but I like to make things from scratch too. Also, this device is meant as an eduatioanl tool for coding Arduino devices using the least amount of parts possible.   





