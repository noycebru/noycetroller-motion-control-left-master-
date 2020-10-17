# noycetroller-motion-control-left-master-

******
This is the motion control version of the noyctroller. I added the I2c dev and MPU6050 as local files because I couldn't get them to install as a library in arduino, so all the files i've included are necessary unless you install the i2cdev and mpu6050 libraries.

This code will be split into two side, left and right, left being the primary (master) i2c and right being secondary. The MPU6050s are also connected via i2c.

The secondary code will be uploaded seperately to limit confusion
***

These work on the Xinput library. If you want to learn how to install the board packages required, please watch my tutorial: https://youtu.be/61U-S7_XTDw or you can read the specifics here: https://github.com/dmadison/ArduinoXInput

This code is a modification of this example: https://github.com/dmadison/ArduinoXInput/tree/master/examples/GamepadPins

3d print files https://www.thingiverse.com/thing:4406183

This controller is based around using two Arduino Pro Micros that communicate with eather other via I2C. The reason for this is pro micros do not have enough pins to cover all of the buttons on an Xbox gamepad. If you use a Teensy board 3.1 it has enough pins to cover all the buttons.

This project is unique because it's an xbox controller split in two, making I2C a great option to limit the number of wires between controllers.

The I2C section of this code was written by: https://www.twitch.tv/gilbertsgadgets

If you make this controller I hope to see a photo of it!
