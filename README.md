# Stary_PCB 
A star-shaped PCB that has a face that changes when a button is clicked. It is an AI assistant!
Purpose: The Stary PCB can take photos and talk back as an assistant when asked a question, and I might even be able to add more cool stuff once I get to connect it to the wifi. 
I wanted to make a Stary in order for it to function as a pocket assistant! 

<img width="977" height="841" alt="Screenshot 2026-10-11 232927" src="https://github.com/user-attachments/assets/fb7cff24-d356-4d6d-90f8-cbdf4f792acb" />
First, I made a Schematic Design: 
I added a microcontroller (with a camera), a push button, a screen, an amplifier, and a speaker.
Then, after I wired all the parts, I transferred the design into the PCB editor. This is where I first cut out a star shape and made it with rounded edges. Then I carefully placed the schematic design by placing the screen in the middle, the camera in the upper left corner, the amplifier on the back, and the button on the right wing of the star. 
<img width="704" height="508" alt="schematic_design" src="https://github.com/user-attachments/assets/bdf6f452-0a61-4a46-a1d7-5f9e60d88732" />
<img width="1023" height="787" alt="star" src="https://github.com/user-attachments/assets/8e38f0a2-3ed1-4572-af4f-21a69c83f767" />

Finally I waas able to place all the parts so I can view them in the 3d view to fininalize the stary. I also added a png of a shimmer and painted some "connection" (js for it to look cool)!!

<img width="1076" height="913" alt="star3" src="https://github.com/user-attachments/assets/e9f6e08b-159c-4a97-a68a-685619cc270e" />
<img width="1523" height="900" alt="star2" src="https://github.com/user-attachments/assets/a2878be4-64f2-4e7f-97ca-356d5eb7bb85" />

This is my final Stary design! 

### 📋 Bill of Materials (BOM)

| Reference | Qty | Value | Description |
| :--- | :---: | :--- | :--- |
| J1 | 1 | LiPo 3.7V | Battery Connector |
| J2 | 1 | LCD GC9A01 2.1IN | Round LCD Display |
| J3 | 1 | MAX98357A AUDIO | I2S Audio Amplifier |
| SW1 | 1 | SW Push | Momentary Push Button |
| U1 | 1 | XIAO-ESP32-S3-SMD | Microcontroller Board |
