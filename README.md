# Rad-Fi-Delay-1.5
Breadboard based glitchy delay using the Teensy 3.2

The rad fi delay 1.5 is an updated version of the <a href="http://bleeplabs.com/rad-fi-central/">original arduino based lo-fi glitch effect</a> released by Bleep Labs in 2015. This new version is meant as a quick breadboard or soldering project you can build right now using off the shelf parts. 
Unlike the atmega328 used in the original, this updated device uses the Teensy 3.2. This allows it to sample audio at 44.1k while still maintaining the simple glitchiness of the original. 

The Rad-Fi Delay can work just like a standard delay effect with a feedback and delay time control.
The trick is that the sample rate of the effect and other features can be controlled with digital inputs and three square wave oscillator outputs. This produces odd arpeggiated, granular sounds. 

<img src="https://raw.githubusercontent.com/BleepLabs/Rad-Fi-Delay-1.5/master/Rad-fi-delay-1v5-breadboard-layout.png">

