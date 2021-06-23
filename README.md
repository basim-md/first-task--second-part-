# first-task--second-part-
في هذا الجزء تم اضافة كود الاردوينو اللازم لتحريك المحركات بزاوية 90 درجة والعودة للوضع الطبيعي 
arduino code:
#include <Servo.h>
  
Servo servo1;
Servo servo2;
Servo servo3;
Servo servo4;
Servo servo5;
int b=0;


void setup() 
{
  servo1.attach(1);
  servo2.attach(2);
  servo3.attach(3);
  servo4.attach(10);
  servo5.attach(12);

}
  
void loop() {
  for (int b = 0; b < 90; b++) {
    servo1.write(b);             
    servo2.write(b);    
    servo3.write(b);
    servo4.write(b);  
    servo5.write(b);        

    delay(30);                     
  }
  for (b =90; b > 0; b--) {
    servo1.write(b);               
    servo2.write(b);    
    servo3.write(b);
    servo4.write(b);  
    servo5.write(b);         

    delay(30);                     
  }
}

رابط مباشر من التنكركاد للمهمة :
https://www.tinkercad.com/things/4dfMfeHzoc6-neat-juttuli/editel?sharecode=k5oidwBf-XHjF4clxne_cegw0giOxLSa4kqn7_51WSo
