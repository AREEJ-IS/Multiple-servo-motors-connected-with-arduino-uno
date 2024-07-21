# Multiple-servo-motors-connected-with-arduino-uno
# LED-matrix-Robot-mouth
## Requirements
- Arduino Board
- Servo Motors x6
- Breadboard
- Wires

## Write the code 
````
#include <Servo.h>
Servo servo1;
Servo servo2;
Servo servo3;
Servo servo4;
Servo servo5;
Servo servo6;

void setup()
{
  servo1.attach(1);
  servo2.attach(2);
  servo3.attach(4);
  servo4.attach(6);
  servo5.attach(9);
  servo6.attach(11);
}

void loop()
{
  for(int i = 0; i <= 180; i = i + 10)
  {
    servo1.write(i); delay(50);
    servo2.write(i); delay(50);
    servo3.write(i); delay(50);
    servo4.write(i); delay(50);
    servo5.write(i); delay(50);
    servo6.write(i); delay(50);
  }
  
  for(int i = 180; i >= 0; i = i - 10)
  {
    servo1.write(i); delay(50);
    servo2.write(i); delay(50);
    servo3.write(i); delay(50);
    servo4.write(i); delay(50);
    servo5.write(i); delay(50);
    servo6.write(i); delay(50);
  }
  
  /*
  for(int j = 0; j <= 180; j = j + 10)
  {
    servo2.write(j);
    delay(500);
  }
  */
  
  
  /*
  for(int j = 180; j >= 0; j = j - 10)
  {
    servo2.write(j);
    delay(500);
  }
  */
}

````
## Build the Circuit

<img width="1440" alt="Screen Shot 2024-07-21 at 11 27 27 PM" src="https://github.com/user-attachments/assets/39ae879e-4509-4fa9-9381-ecf471498121">

<img width="1440" alt="Screen Shot 2024-07-21 at 11 28 14 PM" src="https://github.com/user-attachments/assets/85e35c53-279e-42d1-9041-4005f209e95a">


- Note program that help you design

- Tinkercad :https://www.tinkercad.com/dashboard
 
