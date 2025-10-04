# READ-GREN-LED

## 📘 نبذة

مشروع بسيط يهدف إلى قراءة حالة الـ **LED الأخضر** (Green LED) باستخدام متحكم دقيق مثل Arduino أو Raspberry Pi.

## ⚙️ المتطلبات

- لوحة تطوير (مثل Arduino Uno أو Raspberry Pi)
- مقاومة (220 أوم)
- LED أخضر
- أسلاك توصيل
- برنامج Arduino IDE أو Python (حسب نوع المتحكم)

## 🔌 التوصيل

1. قم بتوصيل السلك الموجب من الـ LED إلى أحد مخارج المتحكم (مثل Digital Pin 7).
2. السلك السالب يمر عبر مقاومة إلى GND.
3. تأكد من تثبيت كل شيء بإحكام.

## 💡 مثال على الكود (Arduino)

```cpp
int ledPin = 7;

void setup() {
  pinMode(ledPin, INPUT);
  Serial.begin(9600);
}

void loop() {
  int ledState = digitalRead(ledPin);
  Serial.println(ledState);
  delay(500);
}
