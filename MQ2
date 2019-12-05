// Input Analog Pins
int smokeA5 = A5;

// Smoke Threshold
int SmokeParameter = 0;

void setup() {
  pinMode(smokeA5, INPUT);
  Serial.begin(9600);
  delay(1500);
}

void loop() {
  int analogSmokeSensor = analogRead(smokeA5);

  Serial.print("Smoke Reading: ");
  Serial.println(analogSmokeSensor);
  Serial.print("--------------------------------------------\n"); 

  // Checks if it has reached the threshold value
  while (analogSmokeSensor >= SmokeParameter)
  { 
    Serial.print("Smoke Reading: ");
    Serial.println(analogSmokeSensor);
    Serial.print("============================================\n");
    delay(1000);
  }
  if (analogSmokeSensor < SmokeParameter)
  {
    Serial.begin(9600);
    Serial.print("\nUnder Threshold. \n");
  }
  
  delay(1000);
}

// FILE PROGRAM END
