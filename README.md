# Line-Follower-Robot

## Components Used

- **Arduino Uno** – Main microcontroller that runs the program.
- **L298N Motor Driver Module** – Controls direction and speed of the motors.
- **3 x IR Sensors** – Used to detect the black line on a white surface (Left, Middle, Right).
- **2 x DC Motors** – Drive the robot's wheels.
- **Chassis** – The body/frame of the robot to hold all components.
- **Wheels (x2)** – Attached to the DC motors for movement.
- **Caster Wheel (x1)** – A free wheel to help balance and smooth motion.
- **Battery Pack (9V or 12V)** – Powers the motors and Arduino.
- **Jumper Wires** – Used for all electrical connections between components.
- **Breadboard (optional)** – For easier prototyping and wiring.

---

## Features

- **Autonomous Line Following**  
  Follows a black line on a white surface using logic based on IR sensor input.

- **3-Sensor Logic**  
  Uses left, middle, and right IR sensors to determine if the robot should go forward, turn left, or turn right.

- **PWM Speed Control**  
  Motor speed is controlled using PWM (Pulse Width Modulation) for smoother motion.

- **Accurate Turning**  
  The robot makes clean directional decisions and adjusts its path precisely when it veers off the line.

- **Fail-Safe Stop**  
  If the robot loses the line completely (all sensors see white), it stops to avoid going off track.

- **Simple Code & Logic**  
  Easy-to-understand code using `if-else` statements — beginner-friendly.

- **Upgradeable**  
  Can be expanded with Bluetooth control, obstacle avoidance, PID control, or more sensors later.

## Circuit Connections – Line Follower Robot

## L298N Motor Driver to Arduino

| L298N Pin | Arduino Pin | Description |
|-----------|-------------|-------------|
| ENA       | 10          | Enable/speed control for Left Motor (PWM) |
| IN1       | 9           | Direction control for Left Motor |
| IN2       | 8           | Direction control for Left Motor |
| IN3       | 7           | Direction control for Right Motor |
| IN4       | 6           | Direction control for Right Motor |
| ENB       | 5           | Enable/speed control for Right Motor (PWM) |
| VCC       | 12V Battery | Motor power supply |
| GND       | GND         | Common ground |
| 5V (if jumper is present) | 5V Arduino | Power logic circuit (optional) |

---

## Motors to L298N

| Motor        | L298N Pins |
|--------------|------------|
| Left Motor   | OUT1, OUT2 |
| Right Motor  | OUT3, OUT4 |

---

## IR Sensors to Arduino

| IR Sensor     | Arduino Pin | Description              |
|---------------|-------------|--------------------------|
| Left Sensor   | A0




