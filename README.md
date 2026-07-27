# iMac-5k-monitor-conversion
# DIY project
In March 2025, I received a free 2013 iMac 27 to play with. After playing it for 3 months with OCLP and OS Sequoia, I decided the performance is not very suitable for my day-to-day use, so I went ahead and acquired a M4 Mac Mini. In the mean time I learned many users have converted it to monitor, and I just happen to need a good monitorfor my Mac Mini, a 27-inch 2K monitor was done after a month through many tries and errors. (I want it to look good and professional)

Then I used the 2K monitor for 6 months, someday the screen went nuts and turned off by itself. It turns out the driver board do not last long for some reason. In this 6 months, I loved the monitor but I felt it could be better if it's a retina display. So, I started to look for how a 5K monitor can be done from internet...(Plus what I have learned by converting my 2K monitor earlier)

Here is the snapshot of what I did:

By capturing ideas from people who successfully converted their iMacs to Monitors, I combined those solutions I like and made my own conversion.

Special thanks to the video from Snazzy Labs inspired me to dig out more possibilities.

https://www.youtube.com/watch?v=5q3SdtiLAPk

And my appreciations to the Macrumors Forum and all contributors inside the Forum filled me with the necessary information.

https://forums.macrumors.com/threads/diy-5k-monitor-success.2253100/



#My Plan
![System Info](https://github.com/asablue65/iMac-5k-monitor-conversion/blob/main/PNG/IMG_7939.png)
![System Info](https://github.com/asablue65/iMac-5k-monitor-conversion/blob/main/PNG/IMG_7941.png)
![System Info](https://github.com/asablue65/iMac-5k-monitor-conversion/blob/main/PNG/IMG_7942.png)

0. iMac 5K 2014-2020 with good screen
* Instead of buying another used iMac 5k, I purchased a 2020 iMac display replacement to start with
* A wrong move, there will be no true tone, and the camera window is a headache. (I nailed it, but get a 2017/2019 display is easier)

1. R1820 V1 as Driver Board
* The build will be based on the R1820 driver board. It supports the full 5120 x 2880 resolution at 10 bit color depth over a single cable.
* R1820n driver board is DDC compatible, therefore you can use apps suach as BetterDisplay to control you monitor backlite and sound volume just like a normal iMac by using Apple keyboards.

2. Thunderbolt/USB-C Ports will be my primary input
* The main input is a USB-C 4.0 and capable of video display and 65W PD output for hooking up a Macbook or any Laptops with a thunderbolt 3/4/5 port.

3. HDMI 2.1
* HDMI 2.1 offers substantially higher bandwidth and many other useful features. It should be able to drive the full 5K resolution at 10 bit color. 
* R1820 driver board offers 2 HDMI inputs

4. DisplayPort 1.4
* For high-resolution displays and seamless data transfer, DP 1.4 offers robust performance. It supports resolutions up to 8K at 60Hz or 4K at 120Hz.
* R1820 driver board offers 2 DP inputs
* To place 2 DP inlets, I have to dig extra holes from the RAM Door housing and FAN Duct housing for the DP extension to work.

5. Webcam, Microphone and Speakers
* An integral part of the iMac experience is the all-in-one sensation. 
* We will install and integrate a slim HD USB autofocus webcam and a noise cancelling dual microphones.

6. Original Speakers
* The original speakers of the iMac will be powered by the onboard amplifier on the R1820 connecting from the 4-pin JST connector to two crossover filters distributing treble and bass to the correct speakers.
* Extra Camera and Microphone modules will be added to simulate the iMac experience.
* Microphones sit outside where Ethernet plug was.

7. The Internal Fan and fan speed control
* Fan will be fairly important to cool off the monitor interior, this 5k monitor can be fairly hot when it's working. I heard bad things happened for not having any ventilation used.
* Extram PWM module will be added to control internal fan.

8. Monitor Controll Access
* I have to create my own controll board and reuse the original iMac USB holes as my access and for monitor status LED.
* I have also modified the input access 3D print to accomdate one more DP port.

9. extra AC outlet 
* By placing a secured M16 plug, my monitor provides AC to my M4 Mac Mini. (Special wiring required)

10. My BOM pictures are inside the PNG folder, you can photo google them, and purchase at the place at your convenience.
* GOOD LUCK with your own iMac 5K conversion

#Conclusion:
* I like my conversion, though not perfect, I have reused everything I could so it provides suitable functions I needed.
* I do not own the skill to sketch my own 3D printings, but I hope that can be nailed, too ;)