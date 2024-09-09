#define BLYNK_PRINT Serial
#include <Wire.h>
#include <Adafruit_PWMServoDriver.h>
#include <WiFiClient.h>
#include <BlynkSimpleEsp32.h>
Adafruit_PWMServoDriver srituhobby = Adafruit_PWMServoDriver(0x40);
#define servoMIN 150
#define servoMAX 600
// Enter your Auth token
char auth[] = "*************";
//Enter your WIFI SSID and password
char ssid[] = "***********";
char pass[] = "*************";	
BLYNK_WRITE(V0) 
{
  int value = param.asInt();
  value = map(value, 0, 180, servoMIN, servoMAX);
  srituhobby.setPWM(0, 0, value);
  delay(1);
}
BLYNK_WRITE(V1) 
{
  int value = param.asInt();
  value = map(value, 0, 180, servoMIN, servoMAX);
  srituhobby.setPWM(1, 0, value);
  delay(1);
}
BLYNK_WRITE(V2) 
{
  int value = param.asInt();
  value = map(value, 0, 180, servoMIN, servoMAX);
  srituhobby.setPWM(2, 0, value);
  delay(1);
}
BLYNK_WRITE(V3) 
{
  int value = param.asInt();
  value = map(value, 0, 180, servoMIN, servoMAX);
  srituhobby.setPWM(3, 0, value);
  delay(1);
}
void loop() 
{
  Blynk.run();
}
