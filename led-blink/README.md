# ESP32 LED Blink

This project is a basic ESP32 example to blink an LED using a GPIO pin.

## 📌 Description
The goal of this project is to get familiar with:
- ESP32 GPIO pins
- Digital output
- Basic Arduino setup

## 🔌 Wiring
The LED is connected to GPIO 2 through a resistor.

![ESP32 Wiring ](images/blink.jpg) 
![ESP32 Wiring ](images/noblink.jpg)

## 💻 Code

```cpp
#define LED_PIN 2

void setup() {
  pinMode(LED_PIN, OUTPUT);
}

void loop() {
  digitalWrite(LED_PIN, HIGH);
  delay(1000);
  digitalWrite(LED_PIN, LOW);
  delay(1000);
}

