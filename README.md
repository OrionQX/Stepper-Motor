#include <Stepper.h>

int motor_yonu = 2048;

#define IN1 4
#define IN2 5
#define IN3 6
#define IN4 7

Stepper myStepper(motor_yonu, IN1, IN2,IN3,IN4);

void setup() {

 myStepper.setSpeed(1)

}

void loop() {
  myStepper.step(-motor_yonu);
  delay(1);

  myStepper.step(motor_yonu);
  delay(1);

}
