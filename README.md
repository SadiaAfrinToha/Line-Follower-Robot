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

  ## Circuit Connections – Bluetooth Controlled Car with Arduino

## L298N Motor Driver to Arduino

| L298N Pin | Arduino Pin | Description |
|----------|-------------|-------------|
| ENA      | 10          | Left motor speed (PWM) |
| IN1      | 9           | Left motor direction control |
| IN2      | 8           | Left motor direction control |
| IN3      | 7           | Right motor direction control |
| IN4      | 6           | Right motor direction control |
| ENB      | 5           | Right motor speed (PWM) |
| VCC      | 12V Battery | Motor power |
| GND      | GND         | Common ground |
| 5V       | 5V (Arduino) *(Optional)* |

---

## Motors to L298N

| Motor        | L298N Pins |
|--------------|------------|
| Left Motor   | OUT1, OUT2 |
| Right Motor  | OUT3, OUT4 |

---

## Bluetooth Module (HC-05/HC-06) to Arduino

| Bluetooth Pin | Arduino Pin | Note |
|---------------|-------------|------|
| VCC           | 5V          | Power supply |
| GND           | GND         | Ground |
| TX            | RX (Pin 0)  | Receives data from Bluetooth |
| RX            | TX (Pin 1)  | Sends data to Bluetooth *(Use voltage divider!)* |

---

## Headlight (LED) to Arduino

| LED Pin | Arduino Pin | Description |
|---------|-------------|-------------|
| +ve     | 1           | Turn ON/OFF via digitalWrite |
| -ve     | GND         | Ground |

---

## IR Sensors to Arduino (Optional for Line Following)

| IR Sensor | Arduino Pin |
|-----------|-------------|
| Left IR   | A0          |
| Right IR  | A1          |
| Middle IR | A4          |

---

## Power Supply Notes

- Use **9V or 12V battery** to power motors via **L298N VCC**.
- Never power motors directly from



