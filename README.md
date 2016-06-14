# Ardunio Bluetooth Controller with Vex for HCRHS
Note: instruction derived from this [adarfuit artical](https://learn.adafruit.com/introducing-the-adafruit-bluefruit-le-uart-friend/)

![Bluefruit](/assets/bluefruit.jpg)
## Wiring

 - Refer to the [wiring diagram][wiring] for how to wire the Bluefruit LE
 - Wire remaing motors 
 - ![Motor witing](/assets/motor-wiring.png)
 - Make sure the switch is flipped to the UART side

![UART](/assets/uart-switch.jpg)
[wiring]: https://learn.adafruit.com/introducing-the-adafruit-bluefruit-le-uart-friend/wiring

## Programing

 - Make sure the Ardunio IDE is upated to at least version 1.6
 - [Download this repo](https://github.com/zethra/ardunio-bluetooth-controller/archive/master.zip)
 - Exctract the zip achieve
 - Copy the contents of the `libraries` directory to `C:\Users\hcadmin\Documents\Arduino\libraries`
 - Open `controller/controller.ino`
 - Added your own code in the designated sections

![Code](/assets/code.png)

 - Refer to the [examples](https://github.com/zethra/ardunio-bluetooth-controller/tree/master/examples/) for help

## Naming Your Robot
 - Flip the previously metioned switch on the Bluefruit LE to the CMD side
 - Upload the `atcommand` sketch included in the zip to the ardunio
 - Open the serial console in the Arundio IDE
 - You should see something like this after a few seconds
 - ![Rename starting console](/assets/name1.png)
 - Type the command `AT+GAPDEVNAME=YOUR NAME HERE` into the input box and hit send (example command: `AT+GAPDEVNAME=HCRHS Test Bot #1`)
 - ![Rename typed command](/assets/name2.png)
 - ![Rename sent command](/assets/name3.png)

## Control
 - Flip the previously metioned switch on the Bluefruit LE to the UART side
 - Install the Bluefruit LE app for [Andriod][andriod] or [IOS][ios]
 - Connect the Arduino to the computer
 - Open the Arduino IDE and upload your code
 - Open the serial monitor and set the baud rate to 115200
 - You should see the following output
 - ![Bluetooth List](/assets/serial1.png)
 - Open the app and make sure bluetooth is turned on
 - Find the Your Robot in the list of devices and click connect
 - ![Bluetooth List](/assets/app1.png)
 - Click controller
 - ![Click controller](/assets/app2.png)
 - If you get the message "Waiting for device info..." for more than a few seconds click back and repeat steps 1 and 2
 - ![Click controller](/assets/app3.png)
 - Scroll down and select "Contol Pad"
 - ![Bluetooth List](/assets/app4.png)
 - The contol pad should come up
 - ![Bluetooth List](/assets/app5.png)
 - And you should see more output from the Arduino
 - ![Bluetooth List](/assets/serial2.png)
 - Push the buttons and the contol pad to operate the robot
 
[andriod]: https://play.google.com/store/apps/details?id=com.adafruit.bluefruit.le.connect&hl=en
[ios]: https://itunes.apple.com/us/app/adafruit-bluefruit-le-connect/id830125974?mt=8
