---
title: "Stary_PCB"
github: "https://github.com/MPichhika2/Stary_PCB"
description: "Stary is a mini keychain. This has the ability to display a face on its circular screen"
created_at: "2026-10-10"
---
# October 10th: Version one of Stary (before I make version 2!!)
Total time: 4.15 hours (with my trying fix errors :( (troubleshooting)))
 **I DO NOT REMMBER IF I TOOK ANY BREAKS BUT I AM ACCOUNTING FOR IT** **In my photos and lapeses, I started at 3:45pm and ended at 9:00pm but I probably had some pauses or breaks so I will am taking an hour off** 

STARY: Version 1
Purpose: The goal is to make a star-shaped PCB Keychain with a circular screen, so when a button is clicked, it will change faces/expression.

**3:30 pm** (DID NOT COUNT AS PROJECT TIME): Took this time to set up; I downloaded Kicad and set that up. I first downloaded all the necessary Libraries into my project Stary_PCB. The New_XIAO_Seriers_Footprints and XIAO_Series_SCH_Symbols. Placed them into a library folder I made in my Stary_PCB folder. 

**3:45 pm:** Started the actual project. I worked on the schematic design where I added:

- **Seeed Studio XIAO ESP32-C3-SMD**: Main microcontroller with Wi-Fi and Bluetooth
- **LiPo 3.7V battery connector**: Connects the rechargeable battery to Stary
- **10-pin GC9B72 LCD connector**: Connects the 2.1-inch circular display for animated faces
- **Pushbutton switch (SW_Push)**: Allows the user to interact with Stary

**3:50 pm:** Started to wire all the components together in the schematic file.  
- Connection from ESP32-C3 D0 (pin 1) to the GND (pin 22) on SW1.
![alt text](image-1.png)

Connections: 

LCD J2 pin	 Display function	Connect to ESP32 U1
1 — TE	 Frame synchronization	 Leave disconnected
2 — SDO	 Data output	         Leave disconnected
3 — BL	 Backlight	             Leave disconnected for now
4 — CS	 Chip select	         D1 — pin 2
5 — DC	 Data/command	         D2 — pin 3
6 — RST	 Reset	                 D3 — pin 4
7 — SDA	 SPI data	             D10 — pin 11
8 — SCL	 SPI clock	             D8 — pin 9
9 — VCC	 Power	                 3V3_OUT — pin 12
10 — GND Ground	                 GND — pin 13

![alt text](image-2.png)
fixed the D0/D1 short circuit!

YAYYYYY!! finished wiring!!

**4:05pm**:FIXED Error.
I opened the PCB editor, then imported the New_XIAO_Series_Footprints into ki-cad. Then I hovered over U1 and matched it with the Seeed Studio Footprint. 
I ended up renaming the libraryu nickname from New_XIAO_Series_Footprints to Seeed_Studio_XIAO_Series because it did not work when imported.Then verified the footprint.

**4:15pm**: Assigned the button footprint!
Searched for the SW_SPST_TL3301AF160QG under the Button_Switch_SMD library 
![alt text](image-3.png)

**4:20pm**: 
![alt text](image-4.png)
Final Schematic design after assigning all the footprints and addressing all error. 

**4:21pm**![alt text](image-5.png) 
I researched more on the screen I was buying to confirm add the deatils and the conenction size. 

**4:41pm**
![alt text](image-6.png)
I ran an Electrical Rules Checker (ERC):
- 13 erroros
- 3 warnings
I added a LCD_BL_CTRL label to both ESP32 D5 and LCD pin 3, labeling them as a LCD backling pin.I also learned that Matching net labels are a electrical connection in ki-cad, not just a note.

**4:47pm**:Crossed off unused pins!
I also went in and fixed unused pins!Used the No Connect Flag tool to do this.
Component	Pin numbers
U1 ESP32	1, 7, 8, 10, 14, 15, 16, 17, 19, 20
J2 LCD	    1, 2

![alt text](image-7.png)

Fixed backlight labels so they are not directly on top. And fixed the missing symbol library (warning). Found the library path of Seeed_Studio_XIAO_Series, then used the folder browser to select the actual .kicad_sym file inside my Stary_PCB file. Then I ran the ERC again and I got 0 erros and also double checked all the footprints for all the components. 

**4:52pm** FINALLY TRANSFERED SCHEMATIC INTO PCB
![alt text](image-8.png)

In my .sch file I went to tools and then I choose Update PCB from Schematic!
Then I arranged the components by placing U1 at the top (of the star we are about to make), the Sw1 to the left, J1 to the right and the J2 LCD towards the bottom. 

**5:10pm** Finished making the basic star outline, after figuring out how to navigate around PCB-editor! I made a star in Edge.cuts layer. 
![alt text](image-9.png)

**5:24pm** Watched tutorials and ended making a good star.
![alt text](image-10.png)
![alt text](image-11.png)
I kept making the star too small, so after a few tries I ended up getting to a nice looking star. Then debated on doing a pixelated look but gave up on that idea lol. BUTTT... I ended adding arc to the star I had making it look better!

**5:45pm**I also measured the star and it has 77.905 mm (width) and 67.319mm(height) then I realizzed the LCD was 2.1 inche and this would be too small!
![alt text](image-12.png)

**20 min break(me js crying)

**6:52pm**Then I tried resizing and changing measurements but my star was still small *still...CRYING* and I gave up again and made a whole new star 
![alt text](image-13.png)
Looking at my screenshot I took almost a whole 30 learning kicad and drawing a star(Gosh so slow). oooo but I learned a lot of stuff:
Blue thin lines are called Rasnet lines and they show the connections that still need routing. 
The red copper tracks are the traces on the front (F.cu)
The Blue copper tracks are traces on the back (B.cu)

**7:00 - 7:30pm** Routing!
![alt text](image-14.png)
 
 All in lapse from here and forward. 

Ended work at **9:00pm** this is where I change to version 2 and think about adding more parts. **I DO NOT REMMBER IF I TOOK ANY BREAKS BUT I AM ACCOUNTING FOR IT** **In my photos and lapeses, I started at 3:45 and ended at 9:00 but I probably had some pauses or breaks so I will am taking an hour off**