# setup jetson nano fan
first lock fan on jetson nano  ventilated rib

* Like this

![](https://github.com/katakusan/image/blob/master/image/IMG_20230723_173857.jpg)

Use this code to open fan

 ```
   sudo sh -c 'echo 255 > /sys/devices/pwm-fan/target_pwm' 
 ```

and write this Lets when your Jetson nano open your fan will be open

```
cd /etc

sudo touch rc.local

sudo chmod u+x rc.local

sudo vim rc.local
```
open a vim file

```
#!/bin/bash

sleep 10

sudo /usr/bin/jetson_clocks

sudo sh -c 'echo 255 > /sys/devices/pwm-fan/target_pwm'
```
write this into your vim file 

press ESC and write :wp and press enter

the fan is open when your Jetson nano open 





























