# Objetivo del Proyecto

**VeloxerGreen** es un sistema integral de riego inteligente diseñado para automatizar y optimizar el proceso de irrigación en espacios urbanos y residenciales, con el fin de mantener la salud de los cultivos y maximizar la eficiencia del recurso hídrico mediante tecnologías accesibles y conectividad remota. Este proyecto busca brindar una solución confiable, escalable y sostenible para usuarios que requieren mantener sus cultivos en condiciones óptimas sin necesidad de intervención constante o presencial.

VeloxerGreen se fundamenta en la necesidad de contar con un sistema que sea capaz de operar de forma autónoma, seguir rutinas personalizadas de riego y, en etapas posteriores, adaptarse a condiciones ambientales mediante el uso de sensores. Al mismo tiempo, se plantea como una plataforma abierta a futuras expansiones tanto a nivel de hardware como de software, permitiendo integraciones con aplicaciones móviles, monitoreo por cámara y control remoto a través de la nube.

### Objetivos Específicos

- **Automatizar el riego** a través de horarios programados, reduciendo la dependencia humana en tareas repetitivas.
- **Optimizar el uso del agua**, controlando con precisión la cantidad y frecuencia del riego.
- **Proteger cultivos** durante ausencias prolongadas del usuario, garantizando su supervivencia mediante la continuidad del servicio.
- **Permitir la gestión remota** mediante el desarrollo de una aplicación móvil en futuras versiones, ofreciendo notificaciones, control manual y monitoreo en tiempo real.
- **Establecer una arquitectura modular**, que permita escalar el sistema y adaptarlo a distintos espacios, necesidades y cantidades de cultivos.
- **Fomentar la sostenibilidad y la autonomía**, incentivando buenas prácticas agrícolas urbanas y el uso eficiente de la tecnología.
- **Construir un sistema confiable**, resistente a fallos comunes y capaz de continuar operando en contextos domésticos o semi-industriales.

## Justificación Técnica y Funcional

El desarrollo de **VeloxerGreen** nace de la necesidad de automatizar procesos de riego de forma inteligente y eficiente, apoyándose en tecnologías accesibles como el **ESP32**, sensores ambientales, relés de control y programación basada en microcontroladores. A través del uso de hardware de bajo consumo energético y fácil implementación, se establece una solución capaz de operar de manera autónoma sin depender de equipos complejos o costosos como servidores o estaciones centrales.

El **ESP32** ha sido elegido como el microcontrolador principal debido a su capacidad de procesamiento, su conectividad Wi-Fi/Bluetooth integrada y su compatibilidad con módulos complementarios.

El sistema contempla:

- Control eléctrico mediante **relés** para activar y desactivar la bomba de agua.
- **Programación con RTC (DS3231)** para garantizar que las tareas se ejecuten con puntualidad incluso sin conexión a internet.
- Un diseño físico resistente, adaptable y protegido, adecuado para ambientes interiores o semicerrados.
- La posibilidad de futura integración con **plataformas IoT** y protocolos de comunicación inalámbrica para análisis y control en tiempo real.

---

### Justificación Funcional

Desde el punto de vista funcional, **VeloxerGreen** ofrece una solución directa y real a un problema cotidiano: la imposibilidad de mantener el cuidado constante de los cultivos por ausencia, tiempo limitado o desconocimiento técnico.

Su función principal es garantizar el **riego regular de forma automatizada**, respetando las condiciones necesarias para el desarrollo saludable de las plantas. Al implementar este sistema, el usuario obtiene:

- **Tranquilidad y confianza** al saber que sus cultivos están siendo atendidos aunque él no se encuentre presente.
- **Ahorro de recursos**, al evitar el riego excesivo o deficiente.
- **Flexibilidad**, ya que puede ser adaptado a diferentes espacios, tamaños de cultivo y configuraciones de hardware.
- **Escalabilidad**, permitiendo la incorporación de nuevos módulos, sensores o funcionalidades sin necesidad de rehacer el sistema desde cero.
- Una experiencia real de **automatización doméstica y domótica**, como ejemplo de aprendizaje y aplicación de habilidades técnicas en un proyecto funcional.

---

## Público Objetivo

**VeloxerGreen** está dirigido a personas interesadas en el cultivo de plantas, el autocuidado de espacios verdes y la automatización doméstica. Se enfoca en usuarios que desean mantener sus cultivos o jardines en buen estado sin depender del riego manual constante, ya sea por falta de tiempo, ausencias prolongadas o simplemente por buscar una solución eficiente y automatizada.

- **Jardineros caseros y urbanos:** Personas que cultivan en patios, terrazas, invernaderos o huertos urbanos y buscan cuidar sus plantas sin complicaciones.
- **Estudiantes y desarrolladores** que desean aprender e implementar soluciones de automatización en el mundo real.
- **Personas que viajan frecuentemente** y requieren una forma de asegurar el cuidado de sus plantas durante su ausencia.
- **Adultos mayores o personas con movilidad limitada**, que prefieren minimizar el esfuerzo físico diario.
- **Amantes del "hazlo tú mismo" (DIY)** que buscan soluciones prácticas y personalizables, aplicando sus conocimientos de electrónica, programación o jardinería.
- **Familias con hijos pequeños**, para quienes un sistema automatizado puede ser una herramienta educativa y funcional para enseñar sobre el cuidado de la naturaleza y la tecnología.

- Conocimientos básicos de jardinería o interés por aprender.
- Curiosidad por la automatización o la tecnología.
- Valoración de la organización, el monitoreo y la mejora de procesos cotidianos.
- Interés por soluciones sostenibles, prácticas y personalizables.
