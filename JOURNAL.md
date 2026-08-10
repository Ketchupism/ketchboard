Post 1 - Starting Schematics

Date - Sat Jul 25

Time used - 2 hours

So I wanted to use the most I can out of the Raspberri Pi, and so I added as many things as I could. A rotary Encoder, An OLED, 14 Columns and 5 Rows of switches. All I did was reverse-engineered this schematics by looking and taking inspiration of how other people did. shoutout daredllama, Tap65, and NMaster23. This was pretty much what I did in those 2 hours and I will probably keep editing until I finalize my schematics and planning of the keyboard

<img width="1866" height="1272" alt="image" src="https://github.com/user-attachments/assets/0c425128-9d10-4d90-9e58-298c0b8d88f5" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Post 2 - Change, finishing Schematics, and starting assigning footprints

Date - Wed Jul 29

Time used - 2 hours

This session I spent time looking for what specfic design I wanted for my keyboard. I decided to get rid of 3 keys on the left of the delete key to save space for the OLED. On the right corner, we the rotary encoder. Below it, there are 3 extra keys. I decided to make the arrow keys stick out by somewhat. I then afterwards set footprints and then went into my PCB editor to see what it looks like. Next post I will probably try to finish everything for the PCB editor. 

<img width="1110" height="1486" alt="image" src="https://github.com/user-attachments/assets/3c3c62fb-38b5-4f77-828c-a9b9c32020ac" />

<img width="1960" height="1342" alt="image" src="https://github.com/user-attachments/assets/67e0e315-606d-4e1f-a622-eff4e35de71a" />

<img width="1474" height="1006" alt="image" src="https://github.com/user-attachments/assets/1140f55c-ddfe-41e4-a1cb-cb858f1d09cb" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Post 3 - Change in rotary encoder switch, changing the u for footprint assignments, and finishing with coordinating the second row of switch

Date - Thu Aug 6

Time used - 3.5 hours

I'm back for work. I came back to realizing that I needed to change some of the keys of the switches so that they were appropriate size. 
example - the caps lock was 1.75u I think
And anything with 2u I added a stabilizer instead. Then when converting into PCB I realized there was a warning for missing MP for the rotary encoder so I added one. Afterwards, I started to organize the rows together but they were not perfect using the grid editor, so I had to resort to using coordinates. I was struggling to understanding how to perfectly put the switches and diodes together, but I overcame that by just coordinating. You can perfectly put switches side by side by having two switches in the same coordinates and adding 19.05, the length of the switch. Using this method took me like ~1.5 hours and I only gotten the second row done.

Another thing to know is if your key is > 1u, but < 2u, then you have to assign the footprint. If the key is > 2u, then you have to add the stabilizer in the schematics and footprint.


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

Post 4 - Time wasted with making the PCB, finished the coordinations of the keyboard, and lastly ended with starting to trace copper wires.

Date - Fri Aug 7

Time used - 4 hours

Half way through today when coordinating the diodes, I realized that the traces were unusual. Most switches also had column 0's instead of 0-5 rows. I searched deeper into my schematics and realized when using net highlights, column 0 went through the rows aswell. I had to restart an hour of work back to square one because after fixing, most of the diodes were set randomly since before it did not properly show the differences between the diodes. Thankfully, I ended the day with finishing all of the switches, diodes, and other parts. I even got to start tracing the OLED and switches. I managed to find coordinates with the OLED using AI because I didn't understand how to find the coordinates where the first pin of the OLED were the one being shown. For the diodes, I use the same coordinates of the switches and x = x+8.25mm, y = y+2.25mm. This was used for all the switches and rotary encoders. I saved some time where all the rows / y of the switches and diodes were the same. Hope to completely finish the PCB tomorrow

Here was what happened after fixing the column 0 and tracing problem
<img width="1754" height="778" alt="image" src="https://github.com/user-attachments/assets/da14b926-a935-4a3e-bf80-f222728dcc8c" />

I literally had to restart the left and right sides of the switches, including all of the diodes which looked like this
<img width="2048" height="1332" alt="image" src="https://github.com/user-attachments/assets/48514284-8320-4ccc-9795-e5e92338ca58" />

Here's a photo of what the last thing I finished with after restarting back to square one, recoordinating diodes, switches, and then started tracing
<img width="1644" height="712" alt="image" src="https://github.com/user-attachments/assets/9a6b4127-9057-4dbf-a783-51e63103a515" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Post 5 - Tracing, debugging errors and warnings, adding 3d models, finalizing the PCB with silkscreen

Date - Fri Aug 9

Time used - 3.5 hours

I've spent the last day just tracing and fixing errors within the PCB. It took a really long time but it looks really clean and organized! Yesterday, I've spent the rest of the day just adding the 3d models for cadding later, adding silkscreen, and other small details to finalize the PCB. The process of making the PCB was alot of hell but eventually came with a very nice PCB. The hardest part of this post was tracing definitely, as I had to organize and push other traces around to fit into a microcontroller. Adding 3d models took a long time because the switches didn't have a default model, so I had to manually add that in aswell. With the 3d model, you can view everything. Diodes, Switches, Rotary Encoder Switch, 0.91 OLED, the Raspberry Pi Pico, and lastly the stablizers. Next post I hope to finish or go halfway through the CAD model. 

Here's a finalized PCB 
<img width="1724" height="758" alt="image" src="https://github.com/user-attachments/assets/8de24dd4-6602-4a51-90ae-79fae7111163" />

Here's a finalized 3d model of the PCB
<img width="1856" height="904" alt="image" src="https://github.com/user-attachments/assets/046cbf20-6dd2-4d8f-9d55-2aeca1486f5d" />
<img width="2006" height="882" alt="image" src="https://github.com/user-attachments/assets/aad09b62-97e1-4e08-8818-4bc54c075b15" />
<img width="2076" height="902" alt="image" src="https://github.com/user-attachments/assets/9df8c020-3966-4ded-a77c-7f4be25ae26c" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Post 6 - Just adding PCB files and adding BOM file

Date - Fri Aug 9

Time used - 2 hours

I've spent 2 hours just researching parts with consideriness with the price and quality. The PCB was extremely annoying for me as any PCB website would be extremely costly because of the size. At the end, I just chose JLCPCB as my regular with a coupon for ~$15. For the other parts, I just chose mainly Amazon, PiShop, and other Canadian shops. At the end of making my BOM, I realized that my keyboard would be extremely expensive, which I couldn't really solve. Afterwards, I went through the tutorial to figure out how to add gerber files to this repo and input it in JLCPCB to estimate my costs.

Here's some photos I took while working 
<img width="2940" height="1692" alt="image" src="https://github.com/user-attachments/assets/3a4a3f71-1fd7-4f33-8bbc-bcb89361bae6" />
<img width="2940" height="586" alt="image" src="https://github.com/user-attachments/assets/d0e1e4c1-e6ff-4dc4-bd9f-05003661d3be" />
<img width="2940" height="824" alt="image" src="https://github.com/user-attachments/assets/40258f02-5fcc-4782-a58e-6126294dc2c0" />
I'll have to cad the case for the keyboard next.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Post 7 - Starting with cad and fixing and updating bom list

Date - Mon Aug 10

Time used - 3

I spent the 2 hours just trying to https://kbplate.ai03.com/ to generate me a perfect cutout of the stabilizers, switches, and rotary encoder. Then I spent time on Fusion360 working on a new case, inspired by my previous macropad. I used the plate generator and put a base between the switch. Then I worked on some small aesthetics for the knob case, and OLED. I then grabbed some 3d models for the keycaps which took quite a while to find some decent models. I then realized I needed some more items for the bom.csv: the stablizers, keycaps, and case. The stablizers and keycaps were hard to find because they were both costly. The most stablizers needed to be lubed, but I decided to buy the cheapest and pre-lubed stablizers. The keycaps I found were hard to find because I had a custom keyboard where I needed extra keycaps. Lastly, the 3d print would be free because of Hack Club's #printing-legion. I realized after calculating some estimate of everything, It was extremely costly. I unfortunately probably need to go searching around for cheaper parts.

Here's a photo of https://kbplate.ai03.com/
<img width="1342" height="758" alt="image" src="https://github.com/user-attachments/assets/03f48fbc-87b7-41e0-84f5-96f7e23c8ef7" />
Here's a photo of the latest work on Fusion, where I added keycaps and a base. 
<img width="2494" height="1162" alt="image" src="https://github.com/user-attachments/assets/a2d458ee-1691-4d23-9817-beec638de589" />
Here's a update on the bom.cvs
<img width="2940" height="526" alt="image" src="https://github.com/user-attachments/assets/b2dfb299-50f6-4fdf-a904-5966662dcb35" />




















