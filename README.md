# Pràctica 1 - BLINK



### Codi de la pràctica:


```cpp
#include <Arduino.h>
#include <stdio.h>


int pin_led = 1;

void setup() {
   pinMode(pin_led, OUTPUT);
   //Serial.begin(115200);
}

void loop() {
    digitalWrite(pin_led, HIGH);
    delay(500);
   // Serial.println("ON");
    digitalWrite(pin_led, LOW);
    delay(500);
   // Serial.println("OFF");
}
```




### Fotografia del muntatge:

![image](https://user-images.githubusercontent.com/125595278/228271323-8b68768b-2fe1-4682-969f-68d08eb3e5ee.png)





### Diagrama de flujo:

![image](https://github.com/paudresaire/p1/assets/125595278/a206767c-610b-44a0-bf76-85733d5773a0)




### Diagrama de tiempo:

![Imatge_diagrama_temps](https://github.com/paudresaire/p1/assets/125595278/ee96a546-ab25-443d-b450-9549cfdc752a)







### En el programa que se ha realizado cual es el tiempo libre que tiene el procesador?

El tiempo libre del procesador es de 500ms, que es el tiempo de delay entre encendido/apagado del led. Sin embargo, nuestro procesador no puede hacer ninguna otra funcion mientrastanto debido a que está ocupado esperando ese tiempo.

