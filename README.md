# Arduino-ESP-Internet-Connection-Check
Check your Arduino/ESP Internet Connection when wifi is connected.



```
#include <WiFiClient.h>

const char* host = "www.google.com"; 


void loop(){

  WiFiClient client;
  if (client.connect(host, 80)) {

    Serial.println("Net connected..");
    client.stop();
    delay(100);

  } else {

    Serial.println("Net not available..");
    client.stop();
    delay(100);

  }

}

```


HappY Coding............ 
