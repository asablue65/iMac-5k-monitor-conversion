# iMac-5k-monitor-conversion
## DIY project
In March 2025, I received a free 2013 iMac 27 to play with. After playing it for 3 months with OCLP and OS Sequoia, I decided the performance is not very suitable for my day-to-day use, so I went ahead and acquired a M4 Mac Mini. In the mean time I learned many users have converted iMacs to monitors, and I just happen to need a good monitor for my Mac Mini, a 27-inch 2K monitor was done after a month through many tries and errors. (I want it to look good and professional)

Then I used the 2K monitor for 6 months, someday the screen went nuts and turned off by itself. It turns out the driver board do not last long for some reason. In this 6 months, I loved the monitor but I felt it could be better if it's a retina display. So, I started to look for how a 5K monitor can be done from internet...(Plus what I have learned by converting my 2K monitor earlier)

Here is the snapshot of what I did:

By capturing ideas from people who successfully converted their iMacs to Monitors, I combined those solutions I like and made my own conversion.

Special thanks to the video from Snazzy Labs inspired me to dig out more possibilities.

https://www.youtube.com/watch?v=5q3SdtiLAPk

And my appreciations to the Macrumors Forum and all contributors inside the Forum filled me with the necessary information.

https://forums.macrumors.com/threads/diy-5k-monitor-success.2253100/



## My Plan
![System Layout](PNG/IMG_7939.png)
![System Input](PNG/IMG_7941.png)
![System Control](PNG/IMG_7942.png)

0. iMac 5K 2014-2020 with good screen
* Instead of buying another used iMac 5k, I purchased a 2020 iMac display replacement to start with
* A wrong move, there will be no true tone, and the camera window is a headache. (I nailed it, but get a 2017/2019 display is easier)

1. R1820 V1 as Driver Board
* The build will be based on the R1820 driver board. It supports the full 5120 x 2880 resolution at 10 bit color depth over a single cable.
* R1820n driver board is DDC compatible, therefore you can use apps suach as BetterDisplay to control your monitor backlite and sound volume just like a normal iMac by using Apple keyboards.

2. Delta PMT-24V200W2B 24V 200W Power Supply
* Unlike most people use MeanWell power supply, I liked Delta better, and its 200W power supply measure the same size as MeanWell's 150W one. So, it's easier to fit and give more power.

3. Thunderbolt/USB-C Ports will be my primary input
* The main input is a USB-C 4.0 and capable of video display and 65W PD output for hooking up a Macbook or any Laptops with a thunderbolt 3/4/5 port.

4. HDMI 2.1 Ports
* HDMI 2.1 offers substantially higher bandwidth and many other useful features. It should be able to drive the full 5K resolution at 10 bit color. 
* R1820 driver board offers 2 HDMI inputs

5. DP(DisplayPort) 1.4 Ports
* For high-resolution displays and seamless data transfer, DP 1.4 offers robust performance. It supports resolutions up to 8K at 60Hz or 4K at 120Hz.
* R1820 driver board offers 2 DP inputs

6. 3D-Print Video Input Bay
* Thanks to pnwkayaker's conversion (https://www.printables.com/model/1225257-imac-5k-conversion-using-sa1-board), I love how he use iMac's RAM Door for all the video inputs, he made a perfect 3D bay for SA1 board, but my R1820 has one extra DP input, so I made minor modification to his design, please check my modification inside the `STL` folder.

7. Webcam, Microphone and Original Speakers
* I will integrate a slim USB autofocus HD webcam and a noise cancelling dual microphones into the iMac for its all-in-one sensation.
* The original speakers of the iMac will be powered by the onboard amplifier on the R1820 connecting from the 4-pin JST connector to two crossover filters distributing treble and bass to the correct speakers.
* Microphones sit at the back of iMac using the ethernet port hole for mic holder at the back of iMac.(Not a great location, but it works for now)

8. The Internal Fan and fan speed control
* Fan will be fairly important to cool off the monitor interior, this 5k monitor can be fairly hot when it's working especially when supplying power to MacBook by its PD 65W. I heard bad things could happen if not having any active ventilation.
* Extra PWM module will be added to control internal fan for lowering its noise. (adjust the PWM according to your working environment.

9. Monitor Control Access
* I have to create my own controller board and reuse the original iMac USB holes as my access and for monitor status LED.
* I also use BetterDisplay to control my monitor backlite and sound volume on my Mac Mini to mimic the iMac experience, it works great!

10. AC plug and extra AC outlet 
* I have reused iMac's original AC inlet and connect it to my power supply by adding a Molex 43640 connector and wire.
* By adding a secured M16 plug, my monitor also provides AC to my M4 Mac Mini. (Special wiring required)

11. My BOM pictures are inside the `PNG` folder, you can photo google them, and purchase at the place at your convenience.
* GOOD LUCK with your own iMac 5K conversion

## Conclusion:
* I like my conversion, though not perfect, I have reused everything I could so it provides suitable functions I needed.
* I do not own the skill to sketch my own 3D printings, but I hope that can be nailed, too ;)

# What to buy

| Item Photo    | Item Description |
| ------------- | ---------------- |
| ![R1820](PNG/StoneTaskin_R1820.png)  | StoneTaskin R1820 V1 Driver Board  |
| ![Delta PMT-24V200W2B](PNG/Delta_PMT-24V200W2B.png) | Delta PMT-24V200W2B Power Supply |
| ![PWM Controller](PNG/12V_PWM_Controller.png) | 12V PWM Controller |
| ![Molex_43640 Connector](PNG/Molex_43640-0300.png) | Molex 43640 for AC inlet Connector |
| ![PCB 80x20mm](PNG/PCB0820.png) | PCB Double Side 80mm x 20mm, Punch Distance: 2.54mm/0.1"  |
| ![Mini Button](PNG/3x6x5mm_Buttons.png) | 3x6mm Mini Buttons 5mm tall |
| ![DP1.4 Adapter](PNG/DP1.4_Ext.png) | Cable Matters DisplayPort 1.4 Adapter Right Angle |
| ![HDMI2.1 Adapter](PNG/HDMI2.1-90D.png) | HDMI 2.1 Adapter Right Angle (up and down) |
| ![USB4 Adapter](PNG/USB4-90D.png) | USB4 Adapter 90-degree)
| ![DP1.4 Extension Cable](PNG/DP1.4-8K.png) | DisplayPort 1.4 Extension Cable |
| ![HDMI2.1 Extension Cable](PNG/HDMI2.1-8K.png) | HDMI 2.1 Extension Cable |
| ![USB4 Extension Cable](PNG/USB4_Ext.png) | USB4 Extension Cable |
| ![iMac Speaker Crossover](PNG/iMac-Speaker-Crossover.png) | iMac Speaker Crossover pair |
| ![USB3 B2C cable for CTRL](PNG/USB3-B2C.png) | USB3 B2C Cable for USB Uplink |
| ![Typec Extension for CTRL](PNG/Type-C_F2F.png) | Type-C extension for USB Uplink |
| ![USB Camera OV5693](PNG/OV5693-72.png) | USB autofocus HD webcam |
| ![USD Active Noise Cancelling Mic Module](PNG/ANC_Dual_Mic.png) | USB noise cancelling dual mic module |
| ![Molex 504050 Connector](PNG/molex_504050.png) | Molex 504050 for internal iMac speaker Connector |
| ![Molex 504051 Connector](PNG/molex_504051.png) | Molex 504051 for internal iMac speaker Connector |