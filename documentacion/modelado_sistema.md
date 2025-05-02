
![CASOS_DE_USO](https://github.com/user-attachments/assets/22799a75-6a42-41e8-ba68-69c89268d443)

El siguiente diagrama representa los principales casos de uso del sistema **VeloxerGreen** desde la perspectiva del usuario. Está basado en los requerimientos funcionales identificados y muestra la interacción entre el actor principal (el usuario) y las funcionalidades del sistema.

La relación `<<include>>` indica que un caso de uso **necesita obligatoriamente** la ejecución de otro (por ejemplo, validar datos al registrarse o iniciar sesión).

La relación `<<extend>>` indica que un caso de uso **puede opcionalmente** extender su comportamiento hacia otro caso más específico (como monitorear en tiempo real y recibir notificaciones).

Este modelo permite visualizar de forma sencilla:

- Las funcionalidades principales del sistema desde el punto de vista del usuario.
- Las funcionalidades auxiliares que amplían o complementan las principales.
- La estructura modular y extensible de la aplicación.

Este diagrama se alinea directamente con los requerimientos funcionales definidos y guía la construcción de los módulos de interfaz y lógica del sistema.





![USER_FLOW](https://github.com/user-attachments/assets/fadeb97d-e8cb-42b6-9c0a-f9e805c97ec3)



El siguiente diagrama representa el flujo de navegación del usuario dentro de la aplicación

**VeloxerGreen**

. Muestra las distintas rutas que un usuario puede seguir desde su inicio en la aplicación, incluyendo el registro o autenticación, la gestión de cultivos mediante una selección desde lista predefinida, el monitoreo de condiciones ambientales a través de sensores, la configuración personalizada del riego y la visualización del historial de actividades.

El flujo destaca la estructura lógica del sistema para garantizar una experiencia intuitiva y organizada en la interacción con los cultivos.









![ERD](https://github.com/user-attachments/assets/bb0a5f6c-fb76-4089-93d3-30aed9e12faa)



El siguiente modelo entidad-relación (ERD) describe la estructura lógica de la base de datos del sistema

**VeloxerGreen**

. Representa las entidades principales: usuarios, cultivos registrados, cultivos predeterminados, riegos realizados, lecturas de sensores ambientales y alertas generadas.

El diagrama define cómo se relacionan entre sí estas entidades, asegurando la integridad de los datos, la trazabilidad de eventos históricos y la correcta vinculación de los cultivos a sus configuraciones de riego y monitoreo.












El siguiente diagrama de clases representa la estructura lógica de los objetos principales dentro del sistema VeloxerGreen, especialmente desde el punto de vista del desarrollo de la aplicación móvil. Este modelo permite visualizar cómo se organizan las clases, sus atributos, métodos y relaciones, facilitando así el diseño orientado a objetos y la implementación eficiente del sistema.

Cada clase define una entidad central en la gestión del riego inteligente, como usuarios, cultivos, sensores y sesiones de riego. Las relaciones entre clases (asociación, agregación o composición) reflejan la forma en que interactúan los componentes del sistema y cómo fluye la información.
