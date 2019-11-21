// PROGRAM START

// Detector Custim Libs Import
#include <dht.h>

// Input Analog Pins
#define dht_apin A1 // Analog Pin sensor is connected to

// Define dht Library as DHT
dht DHT;

void setup() {
  Serial.begin(9600);
  delay(1500);
}

void loop() {
  DHT.read11(dht_apin);

  Serial.print("Temperature Reading (Celsius): ");
  Serial.println(DHT.temperature);
  Serial.print("--------------------------------------------\n"); 

  delay(1000);
}

// FILE PROGRAM END
