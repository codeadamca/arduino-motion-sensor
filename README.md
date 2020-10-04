# arduino-motion-sensor
A basic script to detect motion using an Arduino and a motion sensor.

```csharp
/*

*/

int motionPin = 2;

void setup(){
  
  Serial.begin(9600);
  pinMode(motionPin, INPUT);
  
  pinMode(LED_BUILTIN, OUTPUT);
  
}

void loop (){
  
  delay(1000);
  
  int motionResult = digitalRead(motionPin);
  
  Serial.println(motionResult);
  
  if (motionResult == HIGH) {
    digitalWrite(LED_BUILTIN, HIGH);
  } else {
    digitalWrite(LED_BUILTIN, LOW);
  }
  
}
```
