## Requerimientos del Sistema

### 4.1 Requerimientos Funcionales

- **RF01 - Registro y autenticación de usuarios:**
    - El sistema debe permitir a los usuarios crear una cuenta, iniciar sesión y acceder a su espacio personal de gestión de cultivos.
- **RF02 - Gestión de cultivos a partir de lista predefinida:**
    - Los usuarios deben poder agregar un cultivo seleccionándolo de una lista predefinida de cultivos (ejemplo: cilantro, jitomate cherry, menta, etc.).
    - Al seleccionar un cultivo, se deben cargar automáticamente parámetros de riego predeterminados (frecuencia, duración, horario sugerido).
    - El usuario podrá editar los datos precargados si lo desea.
- **RF03 - Configuración personalizada de riego:**
    - Cada cultivo podrá mantener su configuración de riego predefinida o ser personalizada por el usuario.
    - El usuario podrá ajustar la frecuencia de riego, los horarios de activación y la duración de cada sesión de riego para cada cultivo.
- **RF04 - Activación automática del sistema de riego:**
    - El sistema debe ejecutar el riego de forma automática en los horarios configurados, sin necesidad de intervención manual.
- **RF05 - Control manual del riego desde la aplicación móvil:**
    - El usuario podrá activar o desactivar el riego de cualquier cultivo desde la aplicación en cualquier momento.
- **RF06 - Visualización de variables ambientales:**
    - El sistema debe mostrar lecturas en tiempo real de sensores ambientales asociados a cada cultivo (humedad del suelo, temperatura, y luz ambiental si aplica).
- **RF07 - Histórico y gráficas de datos ambientales:**
    - El sistema debe registrar las lecturas de los sensores y permitir la visualización de gráficas históricas por día, semana o mes, separadas por cultivo.
- **RF08 - Sistema de notificaciones inteligentes:**
    - El usuario será notificado por la aplicación en los siguientes casos:
        - Nivel de agua bajo.
        - Falla en la activación del riego.
        - Valores de humedad fuera de los rangos ideales para el cultivo.
        - Finalización exitosa de un evento de riego.
- **RF09 - Gestión de múltiples cultivos:**
    - El usuario podrá gestionar múltiples cultivos de forma simultánea, cada uno con su propia configuración de sensores, horarios de riego y datos históricos.

---

### 4.2 Requerimientos No Funcionales

1. **RNF01 - Portabilidad:**
    - La aplicación debe ser compatible con dispositivos Android, versión mínima 8.0, y en el futuro adaptarse a iOS.
2. **RNF02 - Disponibilidad:**
    - El sistema debe funcionar las 24 horas del día, de manera autónoma, incluso sin conexión a Internet para tareas críticas (como el riego).
3. **RNF03 - Fiabilidad del reloj:**
    - El módulo RTC debe mantener una hora precisa para asegurar la ejecución correcta del riego.
4. **RNF04 - Seguridad de los datos:**
    - El acceso a la información y control del sistema debe estar restringido mediante autenticación y protocolos seguros.
5. **RNF05 - Escalabilidad:**

La arquitectura debe permitir agregar más cultivos y sensores sin afectar el rendimiento general del sistema.

1. **RNF06 - Interfaz intuitiva:**
    - La aplicación debe presentar una interfaz limpia y fácil de usar, adaptable tanto a usuarios novatos como avanzados.
2. **RNF07 - Persistencia local y sincronización:**
    - El sistema debe guardar los registros críticos localmente en el ESP32 o dispositivo vinculado, y sincronizar con la app cuando haya conexión.
3. **RNF08 - Registro de eventos:**
    - Todo riego activado (manual o automático), lecturas de sensores y alertas deben quedar registrados con fecha y hora.
