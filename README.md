# Disclaimer
This product is not a medical device and is not intended to diagnose, treat, cure, or prevent any disease or medical condition. It should not be used as a substitute for professional medical advice, diagnosis, or treatment. Always consult with a qualified healthcare professional before making any decisions related to your health or using this product in conjunction with a medical treatment plan.

# Introduction
This is a repository for files associated with the PD Buzzboard.  It is open and free to copy.  Any questions can be sent to pdbuzzboard@gmail.com. I hope this content will bring relief to your PD partner as it has to mine.

The PD Buzzboard project has a few variations:
- The "PD Buzzboard" itself, which is a board which sits in your lap, and has vibrating motors on each finger. Users can put this in their lap, place their fingers on the motors, and get vibration on their fingers. This is easiest to build, but users must stay stationary while using.
- The "PD Buzzboard Gloves with One Controller". This variation has a central controllers running the vibration program, typically used in a fanny pack, and wires running from the fanny pack to the gloves. This is more mobile than the buzzboard, as users can walk and move around, but there are some central cables which can get caught on things.
- The "PD Buzzboard Gloves with Separate Controllers". This variation has separate controllers on each hand. This is the hardest to build, but has the most mobility.

# PD Buzzboard
This project will typically take a few hours to build the first time, if you have all the parts and supplies
![IMG_2205](https://user-images.githubusercontent.com/8185194/229241850-693c4389-845f-4d5b-a3c4-0547330350af.jpg)

## Parts & Equipment
### Equipment

This is equipment you must have:
- Soldering Iron - Any one should do, but getting one with clips will make it easier. Here is a random one that should work on Amazon: https://www.amazon.com/Soldering-Iron-Station-Kit-Temperature/dp/B09T3BTDWZ
- Heat Gun - Any heat gun should do, here is one that should work: https://www.amazon.com/SEEKONE-Handheld-Reflector-Embossing-Stripping/dp/B08VFY8THD
- Small phillips head screwdriver
- Computer to program it

### Parts

Working with parts like these, note that they will fail much more often than you would expect of normal consumer products. If you have the budget, I'd recommend getting extras of every part.

- Arduino Uno R3 -	https://www.amazon.com/dp/B008GRTSV6
- USB A-B cable - https://www.amazon.com/AmazonBasics-USB-Printer-Cable-Male/dp/B00NH13DV2
- HiLetgomotorshield – 4 motor	https://www.amazon.com/dp/B01DG61YRM?psc=1&ref=ppx_yo2ov_dt_b_product_details
- Vibrating Motors. We recommend the ones following the Stanford spec: 15,000 rpm -   (meet Stanford spec)	https://www.digikey.com/en/products/detail/vybronics-inc/VW0625AB001G/9974285 but you can use these as an alternative, although their rpm are 12,000 instead of 15,000.	https://www.amazon.com/dp/B0989GN2XY
- Arduino case	https://www.amazon.com/dp/B00UBT87XM OR https://www.amazon.com/gp/product/B0BSLR5LHB (this second one can contain both the motor shield and the Arduino together)
- 1/8”, ¼”, 3/8” heat shrink tubing	https://www.amazon.com/dp/B084GDLSCK
- 22GA wire red and black 	https://www.amazon.com/dp/B07JNRJW37
- USB on off power switch	https://www.amazon.com/dp/B07QQZFYYJ
- USB to power cable	https://www.amazon.com/dp/B0BLKMDM66
- USB power splitter cable	https://www.amazon.com/dp/B085BJRZN2
- Battery power pack (at least 2Amp USB A Output)	
- Command decorating tabs	- https://www.amazon.com/Command-White-Decorate-Damage-Free-17026-40ES/dp/B000M3YGHS
- Lap desk	https://www.amazon.com/dp/B09FTM5XZX
- Wrist rest	https://www.amazon.com/dp/B07D3QJ8WQ
- 2 sided self adhesive velcro	- https://www.amazon.com/Mounting-Double-Side-Reclosable-Fastener-Waterproof/dp/B07CBT5FVP
- Small Cable ties	- https://www.amazon.com/AmazonBasics-Multi-Purpose-Cable-Ties-200-Piece/dp/B087MKMSDY

## Instructions
For instructions on assembly, look here: https://www.youtube.com/watch?v=1PfsVjnPAuQ&t=1456s

### Prepare Central Board
- Take your Arduino Uno and attach the Motor Shield to the top of the Arduino. Line up the motor shield to the end of the board.
- Put your Arduino and Motor Shield into a case.
- Remove the jumper from the Motor Shield.
- Connect USB power source to Motor Shield.
- Connect USB power source to Arduino.
![image](https://user-images.githubusercontent.com/8185194/229240578-8c7c7e98-c4d3-4001-8e2a-2d7cb5a2a556.png height="400")


### Prepare Vibrating Motors
- Cut 16 wires total to length. 8 black wires and 8 red wires.
- Strip the ends of the wires.
- Solder the wires to the vibrating motors. Match the red wire from the motor to the red wire, and match the black wire from the motor to the black wire.

### Cover Vibrating Motors With Protective Covers
- Take 4 1/8 heat shrink tubes and cut them in half, so you have 8.
- Take 4 1/4 heat shrink tubes and cut them in half, so you have 8.
- Take 4 3/8 heat shrink tubes and cut them in half, so you have 8.
- Insert a 1/8 heat shink tubing over the black wire, push all the way to the end.
- Insert a 1/4" heat shrink tube and push it over the red and black wires, pushing it all the way to the end.
- Use the heat gun to shrink it.
- Slide 3/8 heat shrink tube over the 1/4" head shield and the motor.
- Use the head gun on this.
- Repeat for all fingers.

### Install Arduino Software
- Install Arduino IDE
- Plug in Arduino
- Install Adafruit Motor Shield Library
- Upload the sketch

### Attach Vibrating Motors to Arduino Motor Shield
- Attach 2 motors into each "slot" in the Arduino Motor Shield. This is because "Motor 1" slot in the motor shield is sending a pattern for "finger 1 on each hand". So 2 blacks and 2 reds in motor 1 and 2 blacks and 2 reds in motor 2, and same for motor 3 and motor 4.
- Tighten the motor shield screws to ensure the motors are held firmly in place.

### Assemble Lapboard
- Place laboard on table, and put wrist guard on end.
- Have the user place their fingers on the board, and mark each spot.
- Label the fingers as 1, 2, 3, 4, with 1 being the index finger and 4 being the pinky finger.
- Place decorating stickers on each spot. 
- Add the central controller (Arduino) to the top-center of the board, securing it with 2 sided velcro.
- Put the correct vibrating motor to each number. For example, the 2 motors coming from the M1 slot on the Arduino Motor Board go to the 1 finger slot. 
- Add cable tie to secure the motor in place.

### Final Power Assembly
- Put the motor shield and arduino power cables into a Y-splitter, so they have 1 usb powering both.
- Put that usb power into a switch.
- Plug the switch into your battery pack.

### Turn It On and Check It
- Turn it on, and check to see if the light inside is flashing.
- It should work in a pattern, with each finger vibrating. This video shows how it should work and sound: https://www.youtube.com/shorts/loSCJDZAPkg



# PD Buzzboard Gloves with One Controller

## Parts List
Buy all the parts for the PD Buzzboard except you will also need the following:
xxxx <coming soon>


## Instructions
Many of these instructions are similar to the PD Buzz Board itself, but the main difference is that you will be putting the main control board in a central fanny pack, and the user will have the vibrating motors in gloves on their hands. This is more comfortable for them. 

Here is a video of some parts of this build: https://www.youtube.com/watch?v=dvRL9_7ok0E

### Prepare Central Board
- Take your Arduino Uno and attach the Motor Shield to the top of the Arduino. Line up the motor shield to the end of the board.
- Put your Arduino and Motor Shield into a case.
- Remove the jumper from the Motor Shield.
- Connect USB power source to Motor Shield.
- Connect USB power source to Arduino.

### Prepare Vibrating Motors
These motors will connect to the wrist station.
- Cut 16 wires total to length. 8 black wires and 8 red wires.
- Strip the ends of the wires.
- Solder the wires to the vibrating motors. Match the red wire from the motor to the red wire, and match the black wire from the motor to the black wire.

### Cover Vibrating Motors With Protective Covers
- Take 4 1/8 heat shrink tubes and cut them in half, so you have 8.
- Take 4 1/4 heat shrink tubes and cut them in half, so you have 8.
- Take 4 3/8 heat shrink tubes and cut them in half, so you have 8.
- Insert a 1/8 heat shink tubing over the black wire, push all the way to the end.
- Insert a 1/4" heat shrink tube and push it over the red and black wires, pushing it all the way to the end.
- Use the heat gun to shrink it.
- Slide 3/8 heat shrink tube over the 1/4" head shield and the motor.
- Use the head gun on this.
- Repeat for all fingers.

### Build wrist station
The "wrist station" is basically where the individual motors connect from the ends of the fingers to a central part of the wrist. Then, they will connect with a larger cable to a fanny pack, where the central board is. 

- Strip both ends of a CAT 5 cable. There should be 4 pairs of wires. In mine, there was orange, green, blue, and brown. While you can set up the colors in any order you like, I set it up assuming 1 (orange), 2 (green), 3 (blue), 4(brown), with 1 (orange) being the index finger and 4 (brown) being the pinky finger. 
![image](https://user-images.githubusercontent.com/8185194/229240670-7ebd92fa-1f53-438e-b924-d6d152be92e4.png  height="400")
- Use the same colors to represent the same fingers on both sets of gloves.


Each 

### Install Arduino Software
- Install Arduino IDE
- Plug in Arduino
- Install Adafruit Motor Shield Library
- Upload the sketch

### Attach Vibrating Motors to Arduino Motor Shield
- Split your CAT5 cable into 8 separate wires, the 4 colors and the 4 grounds.
  <img  height="400" alt="image" src="https://user-images.githubusercontent.com/8185194/229241356-4b5390a3-4e59-4eab-824f-3efd4ad3e295.png">

- Attach 2 motors into each "slot" in the Arduino Motor Shield. The color corresponding with finger 1 (the index finger) should be in the "Motor 1" slot, and so on. Add the grounds next to the Motor as well.
- Tighten the motor shield screws to ensure the motors are held firmly in place.
![image](https://user-images.githubusercontent.com/8185194/229240696-64d1cc71-85aa-4391-86ac-bb09ea989621.png  height="400")


### Fanny Pack
- Add the central controller (Arduino) to the top-center of the board.
- Put the correct vibrating motor to each number. For example, the 2 motors coming from the M1 slot on the Arduino Motor Board go to the 1 finger slot. 
- Add cable tie to secure the motor in place.

### Final Power Assembly
- Put the motor shield and arduino power cables into a Y-splitter, so they have 1 usb powering both.
- Put that usb power into a switch.
- Plug the switch into your battery pack.

### Turn It On and Check It
- Turn it on, and check to see if the light inside is flashing.
- It should work in a pattern, with each finger vibrating. This video shows how it should work and sound: https://www.youtube.com/shorts/loSCJDZAPkg
For assembly of the gloves themselves, look here: http://www.youtube.com/watch?v=Otokrrb2WSU 

For assembly of the electrical compontents, look here: https://www.youtube.com/watch?v=dvRL9_7ok0E&t=57s

# PD Buzzboard Gloves with Separate Controllers

## Parts List
Coming soon...

## Instructions
More instructions coming soon...

# Vibration Sensor
To know if your PD Buzzboard is working correctly, you will need a vibration sensor.

## Parts List
- Ardiuno Nano - https://www.amazon.com/Arduino-Nano-Every-Single-Board/dp/B07VX7MX27
- Vibration Sensor - https://www.amazon.com/gp/product/B0829SZFBL (this was used successfully) OR https://www.amazon.com/gp/product/B07KS5NV4V/ (ordered but not yet tested)
- Cable to connect Arduino Nano to Vibration Sensor - https://www.amazon.com/Elegoo-EL-CP-004-Multicolored-Breadboard-arduino/dp/B01EV70C78/ref=pd_bxgy_img_sccl_2/142-9931700-3505438?pd_rd_w=HbXTB&content-id=amzn1.sym.6ab4eb52-6252-4ca2-a1b9-ad120350253c&pf_rd_p=6ab4eb52-6252-4ca2-a1b9-ad120350253c&pf_rd_r=YWE164W196MS21VGYW97&pd_rd_wg=14t4p&pd_rd_r=ab8c649b-56c1-4fdb-a338-421d0a2193e3&pd_rd_i=B01EV70C78&th=1

## Instructions
This video gives you the instructions to build it:
https://www.youtube.com/watch?v=qlr-2mkvalQ

- Assemble the sensor unit. Connect the black sensor wire to the GND (ground) and the red sensor wire to the INPUT and tighten. I have seen many of these not work, so you may have to solder them in.
<img width="442" alt="image" src="https://user-images.githubusercontent.com/8185194/229240900-59457e6a-2cb4-46f6-b1d5-1c00671c0e4d.png">

- Assemble the sensor unit. Connect the black sensor wire to the GND (ground) and the red sensor wire to the INPUT and tighten. I have seen many of these not work, so you may have to solder them in.
- Connect the arduino cable from the sensor to the board.
