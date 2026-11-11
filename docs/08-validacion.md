# 08 · Validación

## 1. Métodos de testeo Lean UX

Comparamos cinco métodos de testeo para decidir cuál se ajusta mejor a nuestro prototipo: una base de datos para registrar y consultar los materiales que entran y salen del almacén de Multy Security S.A.S.

| Método | Qué valida | Cómo se aplica | Ventaja | Limitación | ¿Aplica a nuestro prototipo? |
|---|---|---|---|---|---|
| Prueba de usabilidad | Si el usuario logra completar tareas reales con el prototipo y qué dificultades encuentra | Pedimos al usuario realizar tareas concretas con el prototipo mientras lo observamos y registramos tiempos, errores y comentarios | Muestra el uso real y permite detectar problemas de comprensión de los formularios y las consultas | Requiere coordinar al usuario y un espacio de prueba; con pocos participantes los resultados son cualitativos | Sí. Nuestro prototipo ya tiene formularios y consultas que se pueden operar |
| Mago de Oz | Si la idea de solución es útil cuando la funcionalidad aún no existe | Una persona del equipo simula manualmente, detrás de escena, las respuestas del sistema mientras el usuario cree que es automático | Permite probar el valor de una función sin construirla | Exige esfuerzo manual del equipo y no valida el funcionamiento técnico real | No. La v0.1 ya registra y consulta información, por lo que no necesitamos simular |
| Test A/B | Cuál de dos versiones de una misma pantalla o flujo funciona mejor | Se presentan dos variantes a grupos de usuarios y se comparan métricas | Aporta datos comparativos objetivos | Necesita varias versiones y un volumen de usuarios que no tenemos; tenemos un solo usuario | No. Contamos con una sola versión y un único usuario de prueba |
| Prueba de 5 segundos | Si el usuario entiende el mensaje o propósito de una pantalla en muy poco tiempo | Mostramos una pantalla durante 5 segundos y preguntamos qué recuerda y qué entendió | Es rápida y barata; sirve para evaluar claridad visual | No evalúa el uso de formularios ni la ejecución de tareas | Parcialmente. Sirve para la primera impresión, pero no valida nuestra hipótesis |
| Puerta falsa | Si existe interés real en una función antes de construirla | Ofrecemos una función que aún no existe y medimos cuántas personas intentan usarla | Mide la demanda con poca inversión | Mide interés, no usabilidad; el usuario ya expresó su necesidad en la entrevista | No. La necesidad ya fue confirmada y el prototipo ya existe |

## 2. Método elegido

Elegimos la **prueba de usabilidad**, porque nuestro prototipo ya cuenta con formularios de entrada y salida, consulta de existencias e historial que Orlando Morales puede operar directamente.

Nos permite comprobar si registra y consulta los movimientos del almacén sin ayuda, en los computadores de la empresa y en su propio entorno de trabajo.

Los demás métodos evalúan interés, comparaciones o simulaciones que no aportan a nuestra hipótesis, mientras que esta mide directamente la facilidad de uso que el usuario pidió: una automatización fácil de comprender.

## 3. Plan de testeo

| Elemento | Detalle |
|---|---|
| Prototipo a validar | Base de datos para la gestión de inventario del almacén, versión 0.1 |
| Método | Prueba de usabilidad |
| Hipótesis | Creemos que Orlando Morales podrá mejorar el control del inventario de Multy Security S.A.S. si utiliza una base de datos donde se registren los materiales que entran y salen del almacén, se consulten las existencias y se identifiquen los movimientos por cada área de trabajo. Sabremos que es cierto si los movimientos de entrada y salida quedan registrados y se puede consultar la información del inventario sin depender exclusivamente del conteo manual y físico. |
| Participante | Orlando Morales, gerente general de Multy Security S.A.S., quien vive el proceso de inventario |
| Lugar | Instalaciones de Multy Security S.A.S., en los computadores de la empresa, donde se implementa el prototipo |
| Fecha | 7 de noviembre de 2026. Después de la sesión, el prototipo queda instalado para una semana de uso y seguimiento |
| Materiales | Computador de la empresa con el prototipo v0.1 instalado; lista de materiales y áreas de trabajo de ejemplo para registrar; guion de tareas impreso; hoja de observación para anotar tiempos, errores y comentarios; formato de satisfacción de 1 a 5; teléfono o cámara para grabar la sesión con autorización del participante |

### Tareas del participante

| N.º | Tarea | Qué observamos |
|---|---|---|
| 1 | Registrar la entrada de un material al almacén, indicando la cantidad y el área de trabajo | Si encuentra el formulario, completa los campos y guarda el registro sin ayuda |
| 2 | Registrar la salida de un material, indicando la cantidad y el área de trabajo que lo solicita | Si identifica el formulario de salidas y entiende que la cantidad descuenta de las existencias |
| 3 | Consultar las existencias de un material y revisar el historial de entradas y salidas | Si localiza la consulta y encuentra la información que necesita |

### Métrica de éxito

- Orlando completa las 3 tareas sin ayuda del equipo.
- Cada tarea se realiza en un máximo de 3 minutos.
- Los movimientos registrados aparecen correctamente en las existencias y en el historial.
- Califica la facilidad de uso con 4 o más sobre 5.

Consideramos validada la hipótesis si se cumplen estos cuatro criterios. Si no se cumplen, ajustamos el prototipo en una nueva versión.

### Responsables por rol

| Rol | Responsable | Función |
|---|---|---|
| Facilitador | Yoel Morales | Explica el objetivo, entrega las tareas y hace las preguntas sin sugerir respuestas |
| Observador y anotador | Jerónimo Triviño | Registra tiempos, errores, frases textuales y la calificación de satisfacción |
| Registro y soporte técnico | Javier Salamanca | Graba la sesión, deja el prototipo funcionando en los computadores y atiende fallas técnicas |

## 4. Resultados

### Qué observamos
GUION DEL VIDEO (duración aproximada: 2 min 30 s)

0:00 – 0:20 | Presentación
Nos presentamos como equipo Multy security: Yoel Morales, Jerónimo Triviño y Javier Salamanca. Explicamos que el problema es el inventario manual del almacén de Multy Security S.A.S., con conteo en papel, demoras y riesgo de perder información. Mostramos brevemente la pantalla del prototipo v0.1.

0:20 – 0:45 | Hipótesis y método
Explicamos la hipótesis: Orlando Morales podrá mejorar el control del inventario si registra entradas y salidas, consulta existencias e identifica los movimientos por área de trabajo. Indicamos que usamos una prueba de usabilidad porque el prototipo ya se puede operar.

0:45 – 1:05 | Preparación de la prueba
Mostramos el lugar y el computador de la empresa donde está instalado el prototipo. Indicamos la fecha, el 7 de noviembre, y los roles: facilitador, observador y registro técnico. Pedimos la autorización de Orlando para grabar.

1:05 – 1:45 | Las tres tareas
Mostramos a Orlando realizando cada tarea:
- Tarea 1: registrar una entrada de material con cantidad y área.
- Tarea 2: registrar una salida de material.
- Tarea 3: consultar existencias e historial de movimientos.
Se ve cómo el facilitador da las instrucciones sin ayudar y cómo el observador toma notas.

1:45 – 2:10 | Qué observamos y qué dijo el usuario
Resumimos qué tareas completó, cuánto tardó y dónde dudó. Incluimos una o dos frases textuales de Orlando sobre la facilidad de uso y la utilidad de la información.

2:10 – 2:30 | Qué vamos a cambiar y cierre
Explicamos los ajustes que haremos a la v0.1 según lo observado. Cerramos con el siguiente paso: la semana de uso en la empresa y el seguimiento de los resultados. Agradecemos a Orlando Morales y a Multy Security S.A.S.

### Qué dijo el usuario

### Qué vamos a cambiar

Video:(https://drive.google.com/file/d/1d2nPzlT5_9R5wEnl7isfoCdALmP-N3yk/view?usp=drive_link)
