## Video #80 MAX7219-4-in-1  
Various files to support video #80 Scrolling LED Matrix here: https://www/youtube.com/c/RalphBacon

### 125kHz RFID links   
http://blog.deconinck.info/post/2015/04/22/RFID-reader-comparison-HZ-1050-vs-RDM6300

RDM630/6300 Data sheet  
http://store.iteadstudio.com/images/produce/RFID/125KReader_U/RDM630-Spec.pdf

RDM6300 125Khz RFID library (software serial so you can still upload code using the USB port)
https://github.com/Seeed-Studio/RFID_Library


### MAX7219 LED links     MAX7219 LED links  
Modified sketch & libraries (originally by Nick Gammon) to support Eclipse IDE plus extra functions

Hobby Components forum article on the MAX7219  
http://forum.hobbycomponents.com/viewtopic.php?f=58&t=1794

Hobby Components MAX7219 library (works with more than four 8x8 LED matrices)  
http://blog.hobbycomponents.com/?p=334

Notes from Nick Gammon on the MAX7219 LED multiplexer (well worth reading)  
http://www.gammon.com.au/forum/?id=11516

Nick Gammon's MAX7219 library (original) for the 4-in-1 LED unit  
https://github.com/nickgammon/MAX7219_Dot_Matrix

Nick Gammon's Bitbanging SPI library (required for Nick's MAX7219 library)  
https://github.com/nickgammon/bitBangedSPI

My amended version of Nick Gammon's MAX7219 library to work with Eclipse IDE AND have an extra function exposed  
https://github.com/RalphBacon/MAX7219-4-in-1 (zip)

My amended version of Nick Gammon's smooth scrolling sketch to include brightness/speed/switch off controls 
and how to concatenate the message string with special characters (like the 'degrees' symbol)  
https://github.com/RalphBacon/MAX7219-4-in-1 (zip)

IMPORTANT WIRING NOTE  
Note that where Nick mentions the LOAD pin he means the CS (Chip Select) pin on the MAX7219 displays (they have changed the name, I guess)

Arduino Uno/Nano  
Pin 13 - goes to MAX7219 4-in-1 display pin CLK (Clock)  
Pin 11 - goes to MAX7219 4-in-1 display pin DIN (Data in)  
Pin 10 - goes to MAX7219 4-in-1 display pin CS (Chip select)  
