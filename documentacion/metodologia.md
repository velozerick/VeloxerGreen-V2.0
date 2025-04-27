## **Metodología de Desarrollo**

Para el desarrollo del sistema **VeloxerGreen**, se ha adoptado la **metodología de prototipado**, una estrategia de desarrollo iterativa que permite construir versiones funcionales preliminares del sistema, evaluarlas en escenarios reales y aplicar mejoras continuas antes de una implementación definitiva. Esta metodología es especialmente adecuada para proyectos que integran **hardware embebido**, **sistemas físicos** y **aplicaciones móviles**, ya que favorece la validación temprana de funcionalidades clave y el ajuste de requerimientos a lo largo del proceso.

---

### **Fundamentos del modelo de prototipado**

El enfoque de prototipado parte del desarrollo rápido de una versión funcional del sistema (prototipo), que puede ser probada directamente con los usuarios o por el equipo de desarrollo para obtener retroalimentación útil. Esta información permite realizar mejoras iterativas sobre el diseño, comportamiento y experiencia de uso. A diferencia de metodologías secuenciales como el modelo en cascada, el prototipado es **dinámico, adaptable y centrado en el aprendizaje a partir de la práctica**.

---

### **Etapas del proceso de desarrollo**

| **Etapa** | **Descripción** |
| --- | --- |
| **1. Recolección de requerimientos iniciales** | Se identifican las necesidades básicas del sistema, como el control del riego automatizado, el uso de sensores ambientales y la posibilidad de gestionar el sistema de forma remota. |
| **2. Diseño rápido del prototipo** | Se realiza una versión inicial del sistema, enfocada en cumplir con los requerimientos mínimos: activación automática de riego y medición de humedad, controlada por el ESP32 y sensores básicos. |
| **3. Desarrollo físico y digital** | Se integran los componentes físicos (relés, sensores, bombas, RTC) con el microcontrolador ESP32 y se desarrolla la lógica embebida necesaria para ejecutar las acciones del sistema. |
| **4. Evaluación funcional del prototipo** | Se llevan a cabo pruebas funcionales para validar la operación del sistema en condiciones reales, midiendo la respuesta de sensores, la ejecución de rutinas programadas y la estabilidad general. |
| **5. Iteración y expansión del prototipo** | Con base en los resultados, se realizan ajustes y mejoras. Se agregan nuevas funciones como control desde app móvil,  notificaciones inteligentes y módulos adicionales. |
| **6. Pruebas finales e integración completa** | El sistema se somete a pruebas de integración y validación global, evaluando su operación autónoma 24/7, la sincronización con la app y el registro de datos históricos. |
| **7. Documentación técnica y preparación para despliegue** | Se genera la documentación formal, incluyendo diagramas, manuales, plan de pruebas y estructura del sistema, preparando su posible implementación en ambientes reales o comercialización. |


---

### **Aplicación del Prototipado en Hardware y Software**

El modelo de prototipado será aplicado de manera integral en:

- **Hardware**: Validación y optimización de módulos físicos (ESP32, sensores, relés, bombas de agua, RTC).
- **Software**: Desarrollo iterativo de la aplicación móvil de gestión de cultivos, incluyendo interfaz de usuario, control remoto y notificaciones inteligentes.
- **Integración IoT**: Futuras expansiones hacia conectividad con plataformas en la nube y monitoreo remoto.

Este enfoque garantiza que tanto los componentes físicos como los digitales evolucionen de manera coordinada, asegurando la coherencia, funcionalidad y eficiencia del sistema completo.

---


### **Ventajas del modelo de prototipado para VeloxerGreen**

- **Validación temprana** de las funciones esenciales del sistema (riego automatizado, monitoreo, sensado).
- **Retroalimentación constante**, que permite ajustar y mejorar tanto el hardware como la interfaz de usuario.
- **Adaptabilidad** a diferentes entornos, cultivos y necesidades del usuario final.
- **Escalabilidad progresiva**, gracias a la posibilidad de integrar nuevos módulos sin rediseñar todo el sistema.
- **Reducción de riesgos**, al identificar errores de diseño y funcionamiento en etapas tempranas.
- **Desarrollo centrado en la funcionalidad real**, priorizando la utilidad práctica sobre la teoría.
