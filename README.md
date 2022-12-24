# Ender 2 Pro v4.2.7 Motherboard Conversion.
Converting an Ender 2 Pro to use a Creality v4.2.7 Motherboard. This does require the purchase of a cable adapter set from TH3dStudio.com and a Creality v4.2.7 Motherboard. 
## Creality v4.2.7 Motherboard Link. (This is not a paid affiliate link)
### LINK: https://www.amazon.com/gp/product/B07TMX9WFW
## TH3DStudio Link for Adapter Cable Set. (This is not a paid affiliate link)
### LINK: https://www.th3dstudio.com/product/ender-2-pro-stepper-motor-adapter-cable-4-pack/
This adapter kit will make the motors run backwards only on a Creality v4.2.7 motherboard. I have compensated for this in the firmware already and no changes to firmware are necessary, and the motors now turn in the proper direction. 
## If you decide to compile your own firmware, make sure you change the following settings in the firmware in Configuration.h 
1. ### Change #define INVERT_X_DIR false  to  #define INVERT_X_DIR true
2. ### Change #define INVERT_Y_DIR false  to  #define INVERT_Y_DIR true
3. ### Change #define INVERT_Z_DIR true   to  #define INVERT_Z_DIR false
4. ### Change #define INVERT_E0_DIR false  to  #define INVERT_E0_DIR true
# Machine Wiring Safety: 
## All screw terminal wiring connections should have the tinned ends snipped off and replaced with wire ferrules. You can purchase a wire ferrule and cripping tool kit at the links below. This is the kit I used, and the wire strippers. If you are not sure how to use the kit, see video link below.
### Disclaimer: GTPGllc (Gorilla Tech Programming Group, LLC) does NOT get paid or receive products for links to the BV3D You-Tube Channel, or BV3D's affiliate links.
### 1. Wire Ferrule Installation Video Link: https://www.youtube.com/watch?v=8F4zQVzDRww   BV3D Channel on You-Tube
### 2. Wire Ferrule Kit Link: https://amzn.to/3FpvCqI (This is an affiliate link that helps out the BV3D You-Tube Channel)
### 3. Wire Strippers (If you need a god one): https://amzn.to/3bF8vv6 (This is an affiliate link that helps out the BV3D You-Tube Channel) 
# Instructions: (Note: If you are able, use a static ground strap on your wrist while woring on the motherboard removal/installation.)
### (If I have missed any steps in the instalation instructions, please feel free to start an issue and I will ad it to the instructions as soon as I get it.)
1. Raise X Axis gantry all the way to top of the Z Axis. (This will make it easier to access the bottom of the machine.)
2. Power off the machine and unplug the Ender 2 Pro, and remove power cable. Set it aside for now.
3. Tip the machine onto it's right side, the side where the plug goes and where the power switch is, and with the X Gantry End holding up the other side of the machine. This makes it easier to work on. Use a filament box with filament in it under the machine end. This will help balance the machine and raise the machine end up so it makes it easier to get at the screws.
4. Remove the two front rubber feet. (There are two screws hidden under them)
5. Remove the 8 screws from the bottom cover and set them aside. (Have a bowl or magnetic dish handy to hold screws and loose parts)
6. When the cover comes loose, slowly pull it away, and disconnect the case fan wire coupler for the case fan. Set the cover aside.
7. Take a picture of the old wiring placements. You can use this as a reference for reassembly. You can also use the v4.2.7 Wiring Layout PDF file on this repository for reference when reattaching all of the connecters and plugs. The PDF file has a picture of the Creality

8. Unscrew the main power to motherboard leads. (See v4.2.7 Wiring Layout PDF)
9. Unscrew all other terminal screws and pull wiring from terminal blocks.
10. Carefully remove hot glue with small fine tipped pliers that is holding all plugs in their sockets. Do Not Pull On Wire To Remove Plugs. Use a fine tipped set of needle nose pliers to pull the plugs out. Pulling on the wires may damage the connections, and/or cause a short in that plug.
11. Uncrew the ground wires from the top of the brass post that is screwed into the motherboard, and gently remove the brass grounding post by unscrewing it.
12. Unscrew the 3 remaining screws on the motherboard, one near the left end of the motherboard, one near the center of the motherboard, and one next the (E) extruder motor cable port, and remove the ribbon cable for the LCD controller from it's socket. (You again may have to remove hot glue holding it in place.)
13. Carefully remove the old OEM motherboard, and set it aside. After installing the new Creality v4.2.7 Motherboard, place the old OEM motherboard in the silver anti-static bad for storage.
14. Remove the new Creality v4.2.7 motherboard from the silver anti-static bag. (Use it to store the old OEM motherboard in the box the new one came in.)
15. Before installing the new creality v4.2.7 motherboard, now would be a good time to put wire ferrules on all the screw terminal ends, remember to snip the tinned ends off and strip off enough insulation so that the wire goes almost all the way through the wire ferrule, and then crimp it with the crimping tool. If you are not entirely sure how to do this, watch the video at the link near the top of this page.
16. Take note that there are two sets of wires going into the terminal block to the far left (See PDF of wirng diagram), those are for the Hot-End Fan and the Case cooling Fan. Make sure you do not cross wire them, and make sure that each terminal has both wires in the ferrule for the Red(+) and Black(-). Otherwise your hot end fan or your case fan may not work.
17. Slide the new Crality v4.2.7 motherboard into the case and make sure the micro SD card holder and micro USB port go into the stock case holes for them. You will know when you have it placed corectly when all the screw holes in the motherboard line up with screw holes in the case.
18. Using the brass grounding post, screw that in the hole between the X and Y motor ports. This will hold the motherboard inplace while you attach the 3 other screws back in the holes they came out of. This is a direct drop in replacement, so the holes will line up correctly once you have lined up the SD card and USB port. DO NOT OVER TIGHTEN, YOU CAN DAMAGE THE MOTHERBOARD!
19. 
