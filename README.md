# Ardunio Bluetooth Controller with Vex for HCRHS
Note: instruction derived from this [adarfuit artical](https://learn.adafruit.com/introducing-the-adafruit-bluefruit-le-uart-friend/)

![Bluefruit](/assets/bluefruit.jpg)
## Wiring

 - Refer to the [wiring diagram][wiring] for how to wire the Bluefruit LE
 - Wire remaing motors 
 - Make sure the switch is flipped to the UART side

![UART](/assets/uart-switch.jpg)
[wiring]: https://learn.adafruit.com/introducing-the-adafruit-bluefruit-le-uart-friend/wiring

## Programing

 - [Download this repo](https://github.com/zethra/ardunio-bluetooth-controller/archive/master.zip)
 - Exctract the zip achieve
 - Copy the contents of the `libraries` directory to `C:\Users\hcadmin\Documents\Arduino\libraries`
 - Open `controller/controller.ino`
 - Added your own code in the designated sections

![Code](/assets/code.png)

 - Refer to the [examples](https://github.com/zethra/ardunio-bluetooth-controller/tree/master/examples/) for help

## Control
 - Install the Bluefruit LE app for [Andriod][andriod] or [IOS][ios]
 
[andriod]: https://play.google.com/store/apps/details?id=com.adafruit.bluefruit.le.connect&hl=en
[ios]: https://itunes.apple.com/us/app/adafruit-bluefruit-le-connect/id830125974?mt=8
