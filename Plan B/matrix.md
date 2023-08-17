# Matrix(back up plan)

## Why Have Backup plan

Because learning image recognition on Jetson Nano proved to be challenging and progress was slow, we collectively devised a backup plan.

## Aim

The project goal is to achieve a full score using Pixy and Matrix Mini, as only with a full score, there is a possibility to advance to the world competition.

## Project Development and Challenges

* Overall Program Structure:

The main objective of the program is to control the vehicle's movement while maintaining a certain distance from the walls using the laser distance sensors on each side. The color sensor beneath the vehicle is utilized to determine the direction of rotation (clockwise or counterclockwise) and when to turn. The Pixy sensor at the front of the vehicle is responsible for detecting obstacles' distance and color.

* Issue 1: Laser sensor readings exhibit unreasonable fluctuations

* Solution: Extend the sensing range of the laser sensor and apply a clamping filter to eliminate unreasonable readings.

* Issue 2: The color sensor fails to detect the blue and orange lines while the vehicle is in motion.

* Solution: Since the vehicle transitions from white to the color of the line when passing over it, the color sensor readings are set within a specific range.

* Issue 3: The ultrasonic sensor exhibits a delay when measuring over long distances.

* Solution: After continuous testing, we found that the laser sensor provides higher accuracy than the ultrasonic sensor for long-distance measurements. As a result, we replaced the ultrasonic sensor with the laser sensor.

* Issue 4: Car's speed was too fast. The color sensor can't recognize color on the field.

* Solution: Using only laser sensors to observe the road and make turns.
















