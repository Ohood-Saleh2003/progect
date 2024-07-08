## 1- Write an algorithm for operating servo motors to drive the robot :
* 1. Initialize the servo motors: Set up the servo motors and calibrate them to the desired starting positions.

* 2. Read input commands: Read input commands from a control interface or a program that specifies the desired movement direction for the robot.

* 3. Convert commands to servo motor positions: Map the input commands to specific positions for the servo motors. For example, turning left could correspond to a specific angle for one servo motor and turning right could correspond to a different angle for another servo motor.

* 4. Send signals to servo motors: Send signals to the servo motors based on the mapped positions to move the robot in the desired direction.

* 5. Update position: Continuously update the position of the servo motors based on the input commands to ensure smooth and accurate movement of the robot.

* 6. Stop the robot: Implement a mechanism to stop the robot when required, either by sending a stop command or by setting the servo motors to a neutral position.

* 7. Handle errors: Implement error handling mechanisms to deal with any unexpected situations, such as loss of connection or malfunctioning of the servo motors.

* 8. Repeat: Repeat steps 2-7 in a loop to continuously operate the servo motors and drive the robot according to the input commands.
     
## 2-Connect and program an electronic circuit containing 6 servo motors on the simulation program :

### Using the TinkerCAD program, we designed the following electrical circuits:
![لقطة شاشة 2024-07-03 122015](https://github.com/Ohood-Saleh2003/project/assets/173670281/03579cec-e356-4425-a65e-1efa3abdfcf3)
### Circuit programming code:
![لقطة شاشة 2024-07-08 174559](https://github.com/Ohood-Saleh2003/project/assets/173670281/5429885a-7ad7-485e-816d-210ec23880f6)

```
#include <Servo.h>

Servo myServo1, myServo2, myServo3, myServo4, myServo5, myServo6;

void setup() {
  myServo1.attach(12);
  myServo2.attach(11);
  myServo3.attach(10);
  myServo4.attach(9);
  myServo5.attach(8);
  myServo6.attach(7);
}

void loop() {
  // تحريك السيرفو 1 من 0 إلى 90 درجة
  for (int pos = 0; pos <= 90; pos += 1) {
    myServo1.write(pos);
    delay(15);
  }
  for (int pos = 180; pos >= 0; pos -= 1) {
    myServo1.write(pos);
    delay(15);
  }

  // تحريك السيرفو 2 من 0 إلى 90 درجة
  for (int pos = 0; pos <= 90; pos += 1) {
    myServo2.write(pos);
    delay(15);
  }
  for (int pos = 90; pos >= 0; pos -= 1) {
    myServo2.write(pos);
    delay(15);
  }

  // تحريك السيرفو 3 من 0 إلى 90 درجة
  for (int pos = 0; pos <= 90; pos += 1) {
    myServo3.write(pos);
    delay(15);
  }
  for (int pos = 90; pos >= 0; pos -= 1) {
    myServo3.write(pos);
    delay(15);
  }

  // تحريك السيرفو 4 من 0 إلى 90 درجة
  for (int pos = 0; pos <= 90; pos += 1) {
    myServo4.write(pos);
    delay(15);
  }
  for (int pos = 90; pos >= 0; pos -= 1) {
    myServo4.write(pos);
    delay(15);
  }

  // تحريك السيرفو 5 من 0 إلى 90 درجة
  for (int pos = 0; pos <= 90; pos += 1) {
    myServo5.write(pos);
    delay(15);
  }
  for (int pos = 90; pos >= 0; pos -= 1) {
    myServo5.write(pos);
    delay(15);
  }

  // تحريك السيرفو 6 من 0 إلى 90 درجة
  for (int pos = 0; pos <= 90; pos += 1) {
    myServo6.write(pos);
    delay(15);
  }
  for (int pos = 90; pos >= 0; pos -= 1) {
    myServo6.write(pos);
    delay(15);
  }

  delay(2000); // التأخير قبل التكرار
}
```
## Click to enter the tinkercar website:
https://www.tinkercad.com/things/0hqYTGotElo-daring-bombul/editel?tenant=circuits

