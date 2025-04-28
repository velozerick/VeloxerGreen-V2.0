##  Arquitectura General del Sistema**

### Descripción General

El sistema **VeloxerGreen** ha sido diseñado bajo una **arquitectura por capas (multicapa)** para asegurar una estructura modular, escalable y fácil de mantener. Esta separación de responsabilidades permite que cada componente del sistema (hardware, lógica de control, comunicación y visualización) pueda ser desarrollado, probado y mejorado de forma independiente, facilitando futuras expansiones hacia funcionalidades IoT y control remoto.

La arquitectura asegura que el sistema pueda operar de forma autónoma en ausencia de conectividad, y además estar preparado para sincronizarse con una aplicación móvil en futuras versiones.

---

### Objetivos de la Arquitectura

- Separar responsabilidades para evitar acoplamientos innecesarios.
- Permitir mantenimiento y actualizaciones independientes por capa.
- Facilitar la futura integración con servicios en la nube y plataformas móviles.
- Soportar una operación autónoma 24/7 incluso sin conectividad.
- Permitir control local y remoto, monitoreo y almacenamiento histórico de datos.

---

### Modelo de Arquitectura por Capas

Cada capa cumple una función específica dentro del sistema. A continuación se describen las capas que componen VeloxerGreen:

| **Capa** | **Responsabilidad** | **Componentes / Ejemplos** |
| --- | --- | --- |
| **1. Capa de Percepción** | Recoge información del entorno físico y actúa sobre él | Sensores de humedad, temperatura, luz; bomba de agua; relé; RTC |
| **2. Capa de Comunicación** | Transfiere datos entre el hardware (ESP32) y la aplicación móvil | Wi-Fi integrado, ESP32-CAM, HTTP / MQTT, sockets |
| **3. Capa de Procesamiento** | Contiene la lógica del sistema embebido, control de riego, validación de horarios | Código en C++/Arduino, lógica de activación del riego, RTC |
| **4. Capa de Aplicación** | Interacción con el usuario a través de una interfaz móvil | Aplicación Android Studio (Java/Kotlin), control remoto |
| **5. Capa de Almacenamiento** | Guarda configuración, horarios, métricas y registros históricos | EEPROM del ESP32, posible Firebase, archivos locales |

---

### Justificación del Modelo

Esta estructura permite desarrollar una solución modular y sólida, con ventajas como:

- **Escalabilidad**: se pueden añadir nuevos cultivos, sensores o funciones sin modificar el sistema base.
- **Resistencia a fallos**: el sistema puede seguir operando aunque la app no esté disponible.
- **Reutilización**: módulos y lógica pueden usarse en distintos entornos.
- **Preparación para la nube**: es compatible con servicios de backend en fases posteriores.

---

### Aplicación de la Arquitectura

El modelo permite que:

- Cada cultivo pueda tener sensores dedicados y una bomba independiente si es necesario.
- Se gestione información de múltiples cultivos con distintos horarios.
- La app móvil solo consuma datos de forma opcional, ya que el sistema es autónomo.
- A futuro se integre una base de datos o backend centralizado para expandir funcionalidades.
