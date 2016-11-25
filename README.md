# Raspberry-Pi-Floppy-Drive-Song
Uses C language to send certain frequencies or tones to the floppy drive

This is a cool project - if you haven't seen the floopy drive orchestras or songs, go check them out on Youtube or something, they are really cool.

I used a Raspberry Pi 2, just running standard Raspbian Jessie, and a GPIO connection board (bread board and jumoers). The software was already written (thankfully) and I finally got this to work.

So I decided to have a go at this project, and went to a local PC repair shop and got some old Floppy Drives for free. Then I researched and found a program pre-weitten for this in C. SO I just had to set up the wiring.

I ended up figuring out a few things that are important in order for it to work - ground requirements, pins etc, and at one point I very nearly blew my Pi by wiring something incorrectly. I wrote a PDF step by step guide for how I managed to get this set up and running, and the main aim of this repo was to have the resources all in one place. So the C code isn't mine but I don't claim thet it is in any way.

So from what I understand, the Pi has GPIO pins that can be switched between 2 values (for example: 0 and 1, or, On and Off, or,  High and Low). Easy....but I did another project where you send signals through the GPIO at certain frequencies, and transmit audio wirelessly (using a square wave if done in the most basic way). Anyway, this opened up my eyes and I realised that some GPIO pins have more than just binary values (eg: on or off). This C program has all of the Star Wars theme notes written into it as frequencies. 

So for testing I literally just hooked up a tiny speaker to the GPIO pins that were transmitting frequencies, and got the song playing first...if you listen to it like that it is by NO means mp3 quality but the frequencies are output at certain tones, to put it simply, it plays a note by making vibrations.

Once the C program is compiled and running (playing through a simple speaker set-up) the Floppy drive needs to be wired up. When done properly, the frequencies are sent to the FLoppy Drive stepper-motor and it buzzes along at the right frequencies to play the Star Wars theme.

I had to overcome a few problems for this:

* The software is written in C
* Only ever used Python before this
* No idea how to compile C code before executing
* Didn't even know why I had to compile code before running
* Majority of resources for this are for Arduino
* Floppy drives and Raspberry Pi's have an awkward ground preference
* Tons of conflicting information online for setting up the hardware side

So this repo should contain:
----------------------------
The PDF Booklet I wrote with full steps to get this running

The C source code for the song

Link to the video showing the end ressult - the musical FLoppy:



Heres the link to the video showing it in action:
-------------------------------------------------
https://www.youtube.com/watch?v=8nLwsowVrxU


Ben


NOTE
-------
If you read this and the resources aren't here I will hopefully have it all together and uploaded within the hour

