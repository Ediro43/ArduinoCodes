In this project we will be able to connect to an Arduino Board via Bluetooth and sending characters to it in order to display them on the LCD 1602.

For more info about the address scanner found at Point 2 , you can check out this site : https://playground.arduino.cc/Main/I2cScanner/ .

In order to be able to compile the code in Arduino IDE you must download and import the library <LiquidCrystal_I2C.h> .In order to do that you will download the latest <LiquidCrystal_I2C.h>  
version from here https://bitbucket.org/fmalpartida/new-liquidcrystal/downloads/ . This library will be already included in the code from Point 5.

NOTE : for this project we will be using the Terminal Activity from the application.



Steps for the project :

1.Build your Arduino projects using the intructions found at the picture called "I2C Display 1602 building instrcutions.jpg" , from this folder , these should be self explainatory.

2.Open "Code for adress scanner.txt" and copy the code.

3. Go to your Arduino IDE and create a new project and select your board. Paste all the code over there and upload it to your Arduino.

NOTE: You may get an error when trying to upload the code to your arduino device , if so , disconnect the TX and RX wires from your arduino board before uploading code , and after the code is uploaded simply reconnect them.

4. After uploading the code , keep your Arduino Board with the I2C+Display connected to your PC and in Arduino IDE go to : Tools > Serial Monitor 
and there you should see something like : "I2C device found at address 0x27 " . The number "0x27" might be differend for you. If the display is already connect your board and the in Serial Monitor you are seeing : "No I2C devices found" you
did something wrong , check your connections again .

5. Remeber the adress from  Point 4 , and now open  "Code for I2C Display 1602.txt" . 

NOTE: In case you found an address differend than 0x27 on your device , in the text opened at Point 5 , at line 4 "LiquidCrystal_I2C lcd (0x27,2 , 1 ,0 , 4 , 5 ,6 , 7 ,3 , POSITIVE);"
change the first parameter from the paranthesis from 0x27 to the address I told you to remember.

6. Upload the code from Point 5 with the modification you did ( if you did any).Disconnect the RX and TX wires before uploading if needed , and reconnect them once you are done uploading.

7. Open Arduino Bluetooth Controller app , connect to your device , and select Terminal Activity.

8. Click the Bluetooth sign from middle.

9. You are all done now ! Write any text in the text box below and it will be displayed over the LCD.
TIP : You can bind the commands to the buttons from the bottom if you want , for more info press the (i) button on the top right corner.






