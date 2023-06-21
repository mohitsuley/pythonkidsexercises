# Python Exercises for Programming a Robot (Continued)

## Exercise 21: Reading the Optical Sensor
Write a program that reads the light intensity and color from the optical sensor and prints them on the screen.

**Input**: None

**Output**: The light intensity is 50.
The color is red.

## Exercise 22: Changing the LED Color
Write a program that asks the user to enter a color and then changes the LED color to that color.

**Input**: blue

**Output**: The LED state is now True.
The LED color is now blue.

## Exercise 23: Detecting an Object
Write a program that uses the distance sensor to detect if there is an object in front of the buggy. If there is an object, the program should print "Object detected" and turn on the LED with green color. If there is no object, the program should print "No object detected" and turn off the LED.

**Input**: None

**Output**: Object detected
The LED state is now True.
The LED color is now green.

## Exercise 24: Moving the Buggy
Write a program that asks the user to enter a direction and a speed and then moves the buggy in that direction and speed.

**Input**: left
5

**Output**: The wheel's speed is now 5.
The wheel's direction is now backward.
The wheel's speed is now 5.
The wheel's direction is now forward.
The wheel's direction is now forward.
The wheel's speed is now 5.
The wheel's direction is now backward.
The wheel's speed is now 5.
The buggy is moving left at 5 speed.

## Exercise 25: Lifting an Object
Write a program that uses the arm and the touch sensor to lift an object. The program should rotate the arm down until it touches the object, then rotate it up until it reaches 90 degrees, then rotate it down again until it reaches 0 degrees.

**Input**: None

**Output**: The servo's angle is now -90 degrees.
The touch state is False.
The servo's angle is now -89 degrees.
The touch state is False.
...
The servo's angle is now -1 degrees.
The touch state is True.
The servo's angle is now 0 degrees.
The touch state is True.
The servo's angle is now 1 degree.
The touch state is True.
...
The servo's angle is now 89 degrees.
The touch state is True.
The servo's angle is now 90 degrees.
The touch state is True.
The servo's angle is now 89 degrees.
The touch state is True.
...
The servo's angle is now -1 degree.
The touch state is True.
The servo's angle is now -2 degrees.
The touch state is False.
...
The servo's angle is now -90 degrees.
The touch state is False.

# Hints

## Exercise 21: Reading the Optical Sensor
You can use the get_light_intensity() and get_color() methods of the optical sensor object to get the light intensity and color values. For example, light_intensity = optical_sensor.get_light_intensity() will store the light intensity value in a variable called light_intensity. You can use print() function to display text on the screen. For example, print(f"The light intensity is {light_intensity}.") will print this message.

## Exercise 22: Changing the LED Color
You can use input() function to get input from the user. For example, color = input("Enter a color: ") will ask the user for a color and store it in a variable called color. You can use set_led() method of the led object to set the led state and color. For example, led.set_led(True, "red") will turn on the led with red color.

## Exercise 23: Detecting an Object
You can use get_distance_to_object() method of the distance sensor object to get the distance to object value. For example, distance_to_object = distance_sensor.get_distance_to_object() will store the distance to object value in a variable called distance_to_object. You can use an if-else statement to check a condition and execute different blocks of code based on it. For example, if distance_to_object < 10: will execute the code inside if the distance to object value is less than 10. You can use set_led() method of the led object to set the led state and color. For example, led.set_led(True, "green") will turn on the led with green color.

## Exercise 24: Moving the Buggy
You can use input() function to get input from the user. For example, direction = input("Enter a direction: ") will ask the user for a direction and store it in a variable called direction. You can use move() method of the buggy object to move the buggy in a given direction and speed. For example, buggy.move("forward", 10) will move the buggy forward at 10 speed.

## Exercise 25: Lifting an Object
You can use rotate() method of the arm object to rotate the arm by a given degree. For example, arm.rotate(-90) will rotate the arm down by 90 degrees. You can use get_touch_state() method of the touch sensor object to get the touch state value. For example, touch_state = touch_sensor.get_touch_state() will store the touch state value in a variable called touch_state. You can use a while loop to repeat a block of code until a condition is false. For example, while touch_state == False: will execute the code inside the loop until the touch state value is False. You can use a break statement to exit a loop prematurely. For example, break will stop the loop and move on to the next line of code outside the loop.

I hope these exercises and hints are helpful for you and your child. If you have any questions or feedback, please let me know. 😊