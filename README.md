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

| Reference | Qty | Value | Description |Link
| :--- | :---: | :--- | :--- |
| J1 | 1 | LiPo 3.7V | Battery Connector |https://www.amazon.com/JLJLUP-Rechargeable-Integrated-Protection-Development/dp/B0FH9XHXRT/ref=sr_1_1_sspa?crid=1ZFPTSMA4R4VS&dib=eyJ2IjoiMSJ9.li4cggKoqEX1SCSDpXCjx5rcFOkZCffsMpN0MZvvsb-3ts514JaD77b9Zi0EoE2yvqWQQho6XYXZFpXVU01_6DGqK17vN5Z8FfuaJuQFyrumgg5MBa_YGPVEs4JH-amadvfSivi-WXWeFsumB_FD1lDSzuhinzHSJvADKcDifkW4G4adNW5mFZstXtEkIi1csCe7JqPzCbmqA16msmUSZQWdUL0mZaU-c17hyT1By5HbN10kOAZ3ndsB4pG1EU99eW3xAJllsy_c1jy_87fAJLbL3LeosiFYIYiWEbcxx-s.wyrMGXUMYZBJfQJD3PuQXGeb1in74XmtxEOdm40uDCM&dib_tag=se&keywords=lipo+battery&qid=1792773489&sprefix=lipo+battery%2Caps%2C141&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1
| J2 | 1 | LCD GC9A01 2.1IN | Round LCD Display | https://www.seeedstudio.com/XIAO-ESP32S3-Sense-p-5639.html
| J3 | 1 | MAX98357A AUDIO | I2S Audio Amplifier |https://www.adafruit.com/product/3006?srsltid=AU7gw4XkQBUtkr-MiJQN6yo5ufW_RndERFHiWExqMsFZ_fTOXYAt0ue0
| SW1 | 1 | SW Push | Momentary Push Button |(I ONLY NEEED ONE PIECE BUT NO ONE SELLS THAT. IS THERE AN ANOTHER WAY?) https://www.amazon.com/DAOKI-Miniature-Momentary-Tactile-Quality/dp/B01CGMP9GY/ref=sr_1_6?dib=eyJ2IjoiMSJ9.0H9GGs7qKjJ-EE5XDHapeq6keJD7doZZEm6qtEyq8T7-KaPERURoCLBFP1qOYl6YLds8TJOgMgvnXL3f1NBFE67etRNuZ9ImayEXy_1lNtqVa3t7NKQq6WhjyP7mmnWYqX3rdJgLken45dYqB4j0SRmClKEQnKvHoAArC_6PD0Mdp0Vdl72WsIPQcEg8eEw557fQPyhu0oF4hBfRM7IZeCpzchp5PWkb25Zsunbi-rU.QXzTg7w_MsQd-DoV5N1WCv5esSvixRuEVVS-i6S7Ask&dib_tag=se&keywords=tactile%2Bpush%2Bbutton%2Bswitch&qid=1791770041&sr=8-6&th=1
| U1 | 1 | XIAO-ESP32-S3-SMD | Microcontroller Board |https://www.seeedstudio.com/XIAO-ESP32S3-Sense-p-5639.html
