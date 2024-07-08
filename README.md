# project
## 1- Write an algorithm for operating servo motors to drive the robot :
### Circuit programming code:
![لقطة شاشة 2024-07-08 174559](https://github.com/Ohood-Saleh2003/project/assets/173670281/04868f83-9995-49cb-8ade-8b8b5bfd1da1)
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
## 2-Connect and program an electronic circuit containing 6 servo motors on the simulation program :
### Using the TinkerCAD program, we designed the following electrical circuits:
![لقطة شاشة 2024-07-03 122015](https://github.com/Ohood-Saleh2003/project/assets/173670281/03579cec-e356-4425-a65e-1efa3abdfcf3)
## Click to enter the tinkercar website:
https://www.tinkercad.com/things/0hqYTGotElo-daring-bombul/editel?tenant=circuits

