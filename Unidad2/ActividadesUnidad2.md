## **Trayecto de actividades**

### **Ejercicio 1: comunicación entre computador y controlador**

La idea de este ejercicio es comunicar a través del puerto serial un computador con un controlador. La aplicación del computador la construirás usando una plataforma de creación de contenido digital interactivo llamada Unity.

Estudia con detenimiento el código para el controlador y para el computador. Busca la definición de todas las funciones usadas en la documentación de Arduino y de Microsoft.

¿Quién debe comenzar primero la comunicación, el computador o el controlador? ¿Por qué?

Programa el controlador con este código:

```C++
void setup() {
  Serial.begin(115200);
}

void loop() {
if(Serial.available()){
if(Serial.read() == '1'){
      Serial.print("Hello from Raspberry Pi Pico");
    }
  }
}
```
