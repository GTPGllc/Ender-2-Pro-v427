## Ender 2 Pro v4.2.7 Motherboard Conversion.. This firmware is designed to be used with a Stock Hot End at no more than 220c and the Stock Heated bed at no more than 65c. If you change the Hot End out for a Higher temp one, then it is suggested that you attach an external Meanwell Power supply rated at 350watts and 15amps. The OEM PSU is not rated for higher temps and can burn out. You have been warned.
Converting an Ender 2 Pro to use a Creality v4.2.7 Motherboard. This does require the purchase of a cable adapter set from TH3dStudio.com or an Ender 3 Pro Motor Cable Set, and a Creality v4.2.7 Motherboard with a STM32F103RET6 CPU. If the Creality v4.2.7 Motherboard comes with another CPU other than a STM32F103RET6, the firmware provided in this repository will NOT work. You have been warned! 
## Creality v4.2.7 Motherboard Link. (This is not a paid affiliate link)
### LINK: https://www.amazon.com/gp/product/B07TMX9WFW
## TH3DStudio Link for Adapter Cable Set. (This is not a paid affiliate link)
### LINK: https://www.th3dstudio.com/product/ender-2-pro-stepper-motor-adapter-cable-4-pack/
## Ender 3 Pro Motor Cables (This is not a paid affiliate link)
## LINK: https://www.amazon.com/gp/product/B07SYJQFKR
This adapter kit will make the motors run backwards only on a Creality v4.2.7 motherboard. I have compensated for this in the firmware already and no changes to firmware are necessary, and the motors now turn in the proper direction. 
## Specific Firmware Functionality:
 1. Cleaner Main Information Screen.
 2. Single Language Menu System.
 3. Cleaner and more detailed Menu System.
 4. Cleaner and better labled Menu System.
 5. No automatic timeout and return to main information screen. (Really anoying when you turn away for a second, and it is back on the Main Information Screen, and you have to start again.)
 6. You must manually scroll and click to return to previous menus and to the Main Information Screen.
 7. Power Loss Recovery. (Off by Default, but can be turned on in the Settings Menu.)
 8. Filament Run Out Sensor. (Off by Default, but can be turned on in the Settings Menu.)
 9. LCD Assisted Manual 4 Corner Bed Leveling. (Paper method at 4 corners over bed screws, leveling by raising and lowering with bed adjustment wheels)
 10. (9)Nine Point LCD Assisted Manual Mesh Bed Leveing. (No need for ABL Probe) Paper method, raising and lower the nozzle with the LCD knob at (9) nine points around the bed to create a mesh, just like an ABL Probe, but none of the waiting, wiring, setup, firmware recompiling, and in my opinion, a simpler way to level the bed.
 11. Long File Names Enabled.
 12. Scrolling of Longer File Names Enabled.
 13. Removal of ABS Preheat, since the Ender 2 Pro cannot print ABS.
 14. Single PLA Preheat. Temps are as follows: Hot-End 205c Bed Temp 65c.
 15. Thermal Runaway Protection Enabled.
 16. No ABL Probe Function is available, and there will not be at this time. 
 17.  Disregard Next Section if you buy the Ender 3 Pro motor cable set instead of using the motor cable adapter set
## If you decide to compile your own firmware, and use the motor adapters listed above, make sure you change the following settings in the firmware in Configuration.h 
1. ### Change #define INVERT_X_DIR false  to  #define INVERT_X_DIR true
2. ### Change #define INVERT_Y_DIR false  to  #define INVERT_Y_DIR true
3. ### Change #define INVERT_Z_DIR true   to  #define INVERT_Z_DIR false
4. ### Change #define INVERT_E0_DIR false  to  #define INVERT_E0_DIR true
# Machine Wiring Safety: (If you are not sure what you are doing, ask someone who does know what they are doing.)
## All screw terminal wiring connections should have the tinned ends snipped off and replaced with wire ferrules. You can purchase a wire ferrule and crimping tool kit at the links below. This is the kit I used, and the wire strippers. If you are not sure how to use the kit, see video link below.
### Disclaimer: The 300lb Gorilla does NOT get paid or receive products for links to the BV3D You-Tube Channel, or BV3D's affiliate links. However, if you wish to support me and my work here, use Cash App, Cashtag: $The300lbGorilla
### 1. Wire Ferrule Installation Video Link: https://www.youtube.com/watch?v=8F4zQVzDRww   BV3D Channel on You-Tube
### 2. Wire Ferrule Kit Link: https://amzn.to/3FpvCqI (This is an affiliate link that helps out the BV3D You-Tube Channel)
### 3. Wire Strippers (If you need a good one): https://amzn.to/3bF8vv6 (This is an affiliate link that helps out the BV3D You-Tube Channel) 
# Instructions: (Note: If you are able, use a static ground strap on your wrist while working on the motherboard removal/installation.)
### (If I have missed any steps in the removal/installation instructions, please feel free to start an issue and I will add it to the removal/installation instructions as soon as I get it.)
1. Raise X Axis gantry all the way to top of the Z Axis. (This will make it easier to access the bottom of the machine.)
2. Power off the machine and unplug the Ender 2 Pro, and remove power cable. Set it aside for now.
3. Tip the machine onto its right side, the side where the plug goes and where the power switch is, and with the X Gantry End holding up the other side of the machine. This makes it easier to work on. Use a filament box with filament in it under the machine end. This will help balance the machine and raise the machine end up so it makes it easier to get at the screws on the bottom cover and work inside the machine.
4. Remove the two front rubber feet. (There are two screws hidden under them)
5. Remove the 8 screws from the bottom cover and set them aside. (Have a bowl or magnetic dish handy to hold screws and loose parts)
6. When the cover comes loose, slowly pull it away, and disconnect the case fan wire coupler for the case fan. Set the cover aside.
7. Take a few pictures of the old wiring placements. You can use these as a reference for reassembly. You can also use the v4.2.7 Wiring Layout PDF file in this repository for reference when reattaching all of the connecters and plugs. The PDF file has a picture of the Creality

8. Unscrew the main power to motherboard leads. (See v4.2.7 Wiring Layout PDF)
9. Unscrew all other terminal screws and pull wiring from terminal blocks.
10. Carefully remove hot glue with small fine tipped pliers that is holding all plugs in their sockets. Do Not Pull On Wire To Remove Plugs. Use a fine tipped set of needle nose pliers to pull the plugs out. Pulling on the wires may damage the connections, and/or cause a short in that plug.
11. Unscrew the ground wires from the top of the brass post that is screwed into the motherboard, and gently remove the brass grounding post by unscrewing it.
12. Unscrew the 3 remaining screws on the motherboard, one near the left end of the motherboard, one near the center of the motherboard, and one next the (E) extruder motor cable port, and remove the ribbon cable for the LCD controller from its socket. (You again may have to remove hot glue holding it in place.)
13. Carefully remove the old OEM motherboard, and set it aside. After installing the new Creality v4.2.7 Motherboard, place the old OEM motherboard in the silver anti-static bad for storage.
14. Remove the new Creality v4.2.7 motherboard from the silver anti-static bag. (Use it to store the old OEM motherboard in the box the new one came in.)
15. Before installing the new Creality v4.2.7 motherboard, now would be a good time to put wire ferrules on all the screw terminal ends, remember to snip the tinned ends off and strip off enough insulation so that the wire goes almost all the way through the wire ferrule, and then crimp it with the crimping tool. If you are not entirely sure how to do this, watch the video at the link near the top of this page.
16. Take note that there are two sets of wires going into the terminal block to the far left (See PDF of wiring diagram), those are for the Hot-End Fan and the Case cooling Fan. Make sure you do not cross wire them, and make sure that each terminal has both wires in the ferrule for the Red(+) and Black(-). Otherwise your hot end fan or your case fan may not work.
17. Slide the new Creality v4.2.7 motherboard into the case and make sure the micro SD card holder and micro USB port go into the stock case holes for them. You will know when you have it placed correctly when all the screw holes in the motherboard line up with screw holes in the case.
18. Using the brass grounding post, screw that in the hole between the X and Y motor ports. This will hold the motherboard in place while you attach the three other screws back in the holes where they came out of. This is a direct drop in replacement, so the holes will line up correctly once you have lined up the SD card and USB port. DO NOT OVER TIGHTEN, YOU CAN DAMAGE THE MOTHERBOARD!
19. Plug in the 5 pin to 4 pin motor cable adapters in all 4 motor ports, and route them out and around the left end of the board, and then plug in the motor cables to the matching port with the adapter.
20. Attach the two cables with the crimped eyelets on them back onto the brass threaded post. This will help keep the wiring from moving around on you, Use zip ties where needed to help keep the motor cables in place, and additional if needed.
21.  Attach the two red cables from the hot end cables bundle to the far right two screw terminal block holes. (+) and (-) do not matter because in this one case, no polarity for the heater cartridge on the hot end.
22.  Take the Thermister plug from the hot end cable bundle, it should be marked with a "TH" tag, and plug it into the last plug on the bottom row, which is marked with a "TH". It is keyed, so it can only go in one way.
23.  Attach the Red(+) wire from the heated bed wire bundle and put it in the positive terminal marked on the v4.2.7 PDF wiring layout. Third hole from the left. Then put the Black(-) wire in the hole to the right of it, again see PDF of wiring layout if you have any doubts. The plug in the plug marked with a "TB" in the port next to the other Thermister wire, second plug from the right end. (That takes care of the hot end power and Thermister and the heated bed power and Thermister.)
25.  Take the plug with the red and black pigtails that the case fan was connected to, and pair the red to red and black to black from the hot end wire bundle. That is the hot end fan wires. Make sure you snipped and put wire ferrules on both the positive(Red) and the negative(Black), and put the Red(+)wires ferrule in the very first hole from the left. Then put the Black(-) in the only remaining hole next to the red one you just inserted. Make sure all screws are tight on the terminal blocks, but do not over tighten and strip them.
26. There are 3 sets of Limit switch plugs marked with a little rubber tag. Each is marked for the port it goes in. Each port is marked X Y Z. The plugs are keyed and can only go in one way. Along the bottom row, there should be only one open plug, and it has three pins. That is for a filament run out sensor. Only use the one from Creality for this. It is available in the settings, but the default setting is OFF.
27. Above the three pin plug on the bottom row is a pair of two pin plug ports. Those are the parts cooling fan plugs. Take the blue and yellow wired plug from the hot end cable bundle and plug it into the one closest to the three pin plug (Bottom One). Again, this is plug is keyed, so it can only go in one way.
28. Make sure all wiring is going around the outside perimeter of the motherboard, and zip tie loose wiring as needed.
29. Now for the main 24v power connection. It is coming out from the center of the case and it has some black shrink tubing on it to prevent chafing. Make sure you have snipped the tinned end off both wires and crimped wire ferrules on them. The screw terminal is directly below the removable plastic blade fuse on the left edge of the motherboard. The screw terminal is oriented top and bottom, unlike the bottom row which were side by side. Insert the Black(-) cable in the bottom terminal, see the PDF wiring layout if you need to. Tighten down the screw for the Black(-) wire. Now, insert the Red(+) wire in the top terminal and tighten it down.
30. Okay, now tidy up any wiring with zip ties so all of them are neatly bundled and out of the way.
31. Attach the plug from the bottom case cover to the female plug that is shared with the hot end fan, it is keyed, and can only go in one way.
32. Make sure none of the wires are pinched when you put the bottom case cover back in place. The two front rubber fee squares should be on the right. Two bottom case screws on the bottom row, three screws in the middle row, and three screws on the top row.
33. Look at the two rubber blocks you removed, there should be some adhesive on one side, that is the side that goes back on the machine in the squares on the bottom cover. Press firmly and they should stay in place. DO NOT SUPERGLUE THEM ON if they do not stay in place. Clean the glue residue off the rubber blacks and in the squares on the bottom cover. Use very thin clear double sided tape to adhere the rubber blocks back in place if need be.
34. Copy new firmware "firmware-v4.2.7-Ender-2-Pro-20221223-171348.bin" from folder "New Firmware Ender 2 Pro v4.2.7" to a Micro SD Card.
35. Insert Micro Sd Card into Sd card slot, and make sure it is locked in place.
36. Okay. Now the easy part. Plug the power cord into the printer, and then connect to power.
37. Turn the printer on. If there is no smoke, or fire, you did it right. (Kidding)
38. Once the printer boots, if there is a "EEPROM ERROR, Rotate the knob to "Ignore" or "Reset" and click the knob. You might hear a beep.
39. Push the knob and the main menu will appear, rotate down to select System Settings, then push the knob, and rotate down to select Advanced Settings, rotate the knob to Initilize or Reset EEPROM. This will do a memory clear from the previous firmware settings that were preinstalled on the v4.2.7 motherboard. Rotate back to the top, select the top option, and push the knob again, this should bring you to the settings menu, rotate the knob down to "save settings", and push the knob. You should hear a beep, and that confirms that the settings were cleared.
40. Power off the printer.
41. Copy new firmware "firmware-v4.2.7-Ender-2-Pro-20221223-171348.bin" from folder "New Firmware Ender 2 Pro v4.2.7" to a Micro SD Card.
42. Insert Micro Sd Card into Sd card slot, and make sure it is locked in place.
43. Power on printer, and wait for the firmware to update. Once the update finishes, the first boot screen should appear as: HELLO and below that, LOADING......
44. The Second Screen should say "Gorilla Tech" with the version and website github.com/GTPGllc , then the main information screen will appear.
45. If you do not get an EEPROM ERROR, then you are all set. If you do Get an EEPROM Error, then repeat steps 35, 36, 37, 38, 39, 40, 41. You will have to change the firmware file name to make it newer than the first install. The current firmware.bin file is called "firmware-v4.2.7-Ender-2-Pro-20221223-171348.bin", simpley make it newer by adding time to the end of the file name. Current firmware time stamp is 171348, meaning it was 5:13pm and 48 seconds. So we are just going to add 12 seconds to the time stamp in the file name. So the new firmware.bin file will look like this: "firmware-v4.2.7-Ender-2-Pro-20221223-171400.bin", and that will give it the ability to be reloaded as newer firmware. This should clear up the EEPROM ERROR. If you still have issues, please feel free to use the issue or discussion tabs.
46. Now, click knob to "Move, Homne, Level", click knob.
47. Select Home X Y Z
48. Wait for printer to home.
49. Go back to Main Menu.
50. Click on 4 Corner Bed Leveling.
51. Follow the on screen prompts. Use a piece of paper to slide back and forth adjusting the height with the Bed Adjustment wheels.
52. Once 4 corner leveling is done, move to Mesh Bed Leveling. The machine will auto home and go to the first point of nine.
53. Make sure that there is a piece of paper under the nozzle, and start by clicking the know. The head will move to the first position. Use the paper to slide back and forth as you rotate the knob to either up or down to catch the paper. Once you are satisfied with the drag on the paper, click next. Repeat this process with all 9 points. Once you finish with the 9th point, the screen will say "Leveling Complete".
54. Got to main menu, and select "save settings". Now it is time for a test print.
55. From this point on, your on your own. Should you need help, feel free to open either a discussion or an issue, and I will be happy to help.

## DISCLAIMER: The 300lb Gorilla takes no responsibility for monetary loss or damages, injury, or death in the process of doing this motherboard conversion. If you do this conversion, you do so at your own risk, and will not hold The 300lb Gorilla liable for monetary loss or damages, injuries, or death. Proceed at your own risk!
# Sponsorship for this repository: 
##  Cash App, using the cashtag: $The300lbGorilla
