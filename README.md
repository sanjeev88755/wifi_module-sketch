#include <ESP8266WiFi.h>
#define WIFI_SSID "user ID"//enter hotspot ID
#define WIFI_PASSWORD "password"//enter hotspot password
void setup() {
Serial.begin(115200);
WiFi.begin(WIFI_SSID, WIFI_PASSWORD);
Serial.print("Connecting to Wi-Fi");
Serial.print(WIFI_SSID);
while (WiFi.status() != WL_CONNECTED)
{
Serial.print(".");
delay(300);
}
Serial.println();
Serial.print("Connected with IP: ");
Serial.println(WiFi.localIP());
Serial.println();
}

void loop() {
  

}
