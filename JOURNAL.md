Post 1 - Starting Schematics
Date - Sat Jul 25
Time - ~2 hours

So I wanted to use the most I can out of the Raspberri Pi, and so I added as many things as I could. A rotary Encoder, An OLED, 14 Columns and 5 Rows of switches. All I did was reverse-engineered this schematics by looking and taking inspiration of how other people did. shoutout daredllama, Tap65, and NMaster23. This was pretty much what I did in those 2 hours and I will probably keep editing until I finalize my schematics and planning of the keyboard

<img width="1866" height="1272" alt="image" src="https://github.com/user-attachments/assets/0c425128-9d10-4d90-9e58-298c0b8d88f5" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Post 2 - Change, finishing Schematics, and starting assigning footprints
Date - Wed Jul 29
Time - ~2 hours

This session I spent time looking for what specfic design I wanted for my keyboard. I decided to get rid of 3 keys on the left of the delete key to save space for the OLED. On the right corner, we the rotary encoder. Below it, there are 3 extra keys. I decided to make the arrow keys stick out by somewhat. I then afterwards set footprints and then went into my PCB editor to see what it looks like. Next post I will probably try to finish everything for the PCB editor. 

<img width="1110" height="1486" alt="image" src="https://github.com/user-attachments/assets/3c3c62fb-38b5-4f77-828c-a9b9c32020ac" />

<img width="1960" height="1342" alt="image" src="https://github.com/user-attachments/assets/67e0e315-606d-4e1f-a622-eff4e35de71a" />

<img width="1474" height="1006" alt="image" src="https://github.com/user-attachments/assets/1140f55c-ddfe-41e4-a1cb-cb858f1d09cb" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Post 3 - Change in rotary encoder switch, changing the u for footprint assignments, and finishing with coordinating the second row of switch
Date - Thu Aug 6
Time - 3.5 hours

I'm back after work and ec. I came back to realizing that I needed to change some of the keys of the switches so that they were appropriate size. 
example - the caps lock was 1.75u I think
And anything with 2u I added a stabilizer instead. Then when converting into PCB I realized there was a warning for missing MP for the rotary encoder so I added one. Afterwards, I started to organize the rows together but they were not perfect using the grid editor, so I had to resort to using coordinates. I was struggling to understanding how to perfectly put the switches and diodes together, but I overcame that by just coordinating. You just add the distance of a switch so it horizontally fits and then have the same Y axis. This took me like ~1.5 hours and I only gotten the second row done.


Here's a photo of the MP attached, afterwards there were no warnings
<img width="1328" height="656" alt="image" src="https://github.com/user-attachments/assets/ff6731b3-c8b8-474a-ae5f-f178fd26b100" />

Here's a photo of my footprints and what I changed 
<img width="852" height="200" alt="image" src="https://github.com/user-attachments/assets/662ecbea-1472-4b97-b7aa-e72fe2a5345e" />
<img width="856" height="112" alt="image" src="https://github.com/user-attachments/assets/423afdce-2352-434f-b76d-001a5412b3c9" />

Here's a photo of all the parts, sorting, and somewhat organizing them into the keyboard layout
<img width="2048" height="1332" alt="image" src="https://github.com/user-attachments/assets/4c8458e2-71a3-4c0a-bcaa-c62c6a02130c" />

Here's a photo of after organizing the first row with coordinates: 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/69b39874-795c-4a15-a587-8ca1fc939195" />

Hope to finish the PCB tomorrow as I have to spend more time before i'm away for a while

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------





















