 This folder contains the bulding instructions and the codes needed to construct a fully working car that is controlled via bluetooth !

 The diference between the SimpleCar and CarWithSpeeds is that.... the second one can move at differend speeds and the fact that it uses two more lines ,
one for the left side motors and one for the right side motors.

 If you are using my code exacly how it is written above , you can simply open the Arduino Bluetooth Controller/Remote app , scan for a new device , select your device 
and tap on the Car Controller button. Here you will have to tap the middle button with the Bluetooth sign on it , once connected the background of that button will 
be a bighter blue . After you connected you are good to go ! Enjoy your Arduino car :)

 If you want to change some of the commands that are giving to the Arduino car you have to do two steps :
1.In the code you need to modify the commands , such as , in my code there is case '1' (for going forward) , if you want other character than 1 to be sent to your device you need 
to change it to let's say case 'x'
NOTE : Remeber that the application only works with characters such as 'a' or 'b' , it will not work if you put your code such as "abcd" , it works just for a single item.
2.Open the app and choose your Arduino car, after that head up to the Car controller. Here tap on the middle Bluetooth sign button , after you connected to your device , 
that button will be a brighter blue . Now , since you modified some of the commands that are given to the car , tap the Setting button and look there for the command you changed . 
For example you changed the command for forward like this : case 'a' : ( go forward ) , well in this case in the Settings menu you need to find the forward button and 
in the right side of it you need to add the character a . That's it :) !
 
