sudo sh -c 'echo 255 > /sys/devices/pwm-fan/target_pwm' 

open fan

cd /etc

sudo touch rc.local

sudo chmod u+x rc.local

#!/bin/bash

sleep 10

sudo /usr/bin/jetson_clocks

sudo sh -c 'echo 255 > /sys/devices/pwm-fan/target_pwm'
can let fan open when Jetson naon open
