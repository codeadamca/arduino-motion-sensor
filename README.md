# arduino-motion-sensor
A basic script to detect motion using an Arduino and a motion sensor.

```csharp
int motion_1 = 2;

void setup(){
  
  Serial.begin(9600);
  pinMode (motion_1,INPUT);
  
}

void loop (){
  
  delay(1000); //this delay is to let the sensor settle down before taking a reading
  
  int sensor_1 = digitalRead(motion_1);
  
  Serial.println(sensor_1);
  
  if (sensor_1 == HIGH){
    

  }
}
```
