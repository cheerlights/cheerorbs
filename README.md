# CheerOrb

Here is the Arduino code and the 3D printer STL files to make your own CheerOrb.

## Hardware

ESP8266  
[Wemos D1 mini](https://www.wemos.cc/en/latest/d1/d1_mini.html)  
Neopixel  
I use the single LED shield  
[WS2812B RGB shield](https://www.aliexpress.com/item/32757360867.html)  

If you choose to use the 7-LED shield from LOLIN [RGB LED Shield](https://www.wemos.cc/en/latest/d1_mini_shield/rgb_led.html) change line `70` of the sketch from  
`Adafruit_NeoPixel pixel = Adafruit_NeoPixel(1, D2, ORDER); // 1 pixels on pin D2`  
to  
`Adafruit_NeoPixel pixel = Adafruit_NeoPixel(7, D4, ORDER); // 7 pixels on pin D4`

Solder the top and  bottom through-pin headers onto the Wemos board and attach the neopixel shield on top, making sure you get it the right way round (so all the pin labels align correctly).

Power with a Micro-USB cable.

## Software

Download the .ino file and build it in the Arduino IDE.  
You need a few extra libraries, installed through the library manager.


## 3D printed case
Print the base and top in translucent filament on “normal” setting (takes about 2 hours for the top and 30 mins for the base).

### Assembly
- Put a drop of superglue onto each of the 4 pin holders.  
- Push the wemos board down into the holders.   
- Wait for the glue to dry.  
- Put a drop of superglue in the middle of the 3 edges of the base that are not the USB socket edge.   
- Push the top firmly but carefully down onto the base, making sure the cut-out is next to the USB socket.  
- Wait for the glue to dry.  

## Configuring your CheerOrb
Connect your CheerOrb to your WiFi using the instructions here: [CheerOrb instructions](https://cheerlights.com/orb).


**Have fun :)**

