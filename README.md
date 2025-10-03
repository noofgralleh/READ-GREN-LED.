# READ-GREN-LED.
int redPin   = 9;   // الرجل الأحمر
int greenPin = 10;  // الرجل الأخضر
int bluePin  = 11;  // الرجل الأزرق

void setup() {
  pinMode(redPin, OUTPUT);
  pinMode(greenPin, OUTPUT);
  pinMode(bluePin, OUTPUT);
}

void loop() {
  // تشغيل اللون الأحمر
  setColor(255, 0, 0);  
  delay(1000);

  // تشغيل اللون الأخضر
  setColor(0, 255, 0);  
  delay(1000);

  // تشغيل اللون الأزرق
  setColor(0, 0, 255);  
