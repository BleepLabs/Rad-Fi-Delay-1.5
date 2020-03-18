# Rad-Fi-Delay-1.5
Breadboard based glitchy delay using the Teensy 3.2

See it in action here 

The rad fi delay 1.5 is an updated version of the <a href="http://bleeplabs.com/rad-fi-central/">original arduino based lo-fi glitch effect</a> released by Bleep Labs in 2015. This new version is meant as a quick breadboard or soldering project you can build right now using off the shelf parts. 
Unlike the atmega328 used in the original, this updated device uses the Teensy 3.2. This allows it to sample audio at 44.1k while still maintaining the simple glitchiness of the original. 

The Rad-Fi Delay can work just like a standard delay effect with a feedback and delay time control.
The trick is that the sample rate of the effect and other features can be controlled with digital inputs and three square wave oscillator outputs. This produces odd arpeggiated, granular sounds. 

This is a simple but fun educational device that can help you get started making Arduino devices. Check out the fully comemnted code for more info. 

<img src="https://raw.githubusercontent.com/BleepLabs/Rad-Fi-Delay-1.5/master/assembled-device.jpg">

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


<img src="https://raw.githubusercontent.com/BleepLabs/Rad-Fi-Delay-1.5/master/rad%20fi%20delay%201v5%20schematic.bmp">
An input opamp is required to get the audio to the correct level and protect the Teensy. 
After the input jack there is a simple attenuator. This volume control pot allows you to use signals with a large range like those coming from a modualr syth or quieter ones like those coming from a line level output. 
Then a capacitor and resitors going to 3v3 and ground. This centers the signal around the halfway point, 1.65V. Next another resistor and opamp. This buffers and amplifies the signal and keeps the output between 3v3 and ground. The opamp below it makes another voltage referance at 1.65V for the first opamp to operate with. 

---------------

<i>Are you selling a kit?</i><br>
Not right now but if you're interested sign up for <a href="https://confirmsubscription.com/h/r/35B95AB32EF3DEEC2540EF23F30FEDED">this mailing list<a/> and I'll email about this <b>only</b>. (Sign up <a href="https://confirmsubscription.com/h/r/A3B09EAD151885B6">here</a> for all Bleep Labs news). I threw this device together with the simplest parts possbile so anyone could get the parts they need from a variety of sources (see the <a href="https://docs.google.com/spreadsheets/d/1HgXk2Bo4Rd0A5V1MbUsgcbOM54Az-JnbRDxo8K8Pac8/edit?usp=sharing">Parts list</a>
). 

<i>Why not use the <a href="https://www.pjrc.com/teensy/td_libs_Audio.html">Audio libary</a> and board?</i><br>
I love Paul's audio library and have used it on my producest and even contributed to it but I like to make things from scratch too. Also, this device is meant as an eduatioanl tool for coding Arduino devices using the least amount of parts possible.   

Email me with any questions
drbleep@bleeplabs.com



