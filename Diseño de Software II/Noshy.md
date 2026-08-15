
## Descripción general del negocio.

 **Noshy** es un ecosistema digital inteligente diseñado para cerrar la brecha entre los objetivos de salud personalizados y la ejecución culinaria diaria. Busca, por medio del despliegue de Agentes de Inteligencia Artificial Especializados (Chef Agents Personalizados), ofrecer un servicio de acompañamiento integral y dinámico en el proceso de nutrición. Estos agentes no planifican la alimentación basada en biometría y preferencias, sino por medio de un acercamiento al natural. Este acercamiento se realiza mediante un ciclo de aprendizaje continuo basado en el comportamiento del usuario, sirviendo, de esta forma, como apoyo al momento de realizar compras, entendiendo como se asocian componentes nutricionales, marcas y diferentes productos, con preparaciones a la medida de cada usuario de la plataforma.

Noshy también cuenta con una **comunidad**, donde usuarios puedan publicar y compartir preparaciones. Cada receta, a discreción del usuario, se asociará con el agente chef consultable, capaz de responder preguntas y ayudar a adaptar la preparación según las necesidades de cada persona.

Considerando la naturaleza del sistema como uno distribuido orientado a microservicios, divididos en 3 módulos fundamentales:
- **Motor de Personalización (IA):** Sistema de recomendación y generación de contenido (recetas y planes) basado en modelos de lenguaje.
- **De Datos (DB):** Sistema de persistencia y orquestación de la lógica de negocio (inventarios y perfiles)
- **Comunidad y Web:** Interfaz de acceso al sistema y gestión social.


---
## Justificación de la propuesta de valor.

Noshy no se plantea como una aplicación más de recetas, sino como una solución que ataca la distancia que existe entre tener una meta de alimentación y *llevarla a cabo*. La mayoría de las personas no fracasan por falta de información nutricional, sino por la dificultad de traducir esa información en decisiones repetibles. Noshy busca entonces asumir esa traducción.

#### 1. Resuelve la fatiga de decisión y la ejecución
Planificar qué comer, calcular las macros, armar el mercado y ajustarlo todo a gustos, metas, etc... es un proceso mentalmente costoso que la gente abandona con facilidad. Noshy desplaza esa carga del usuario hacia un agente: el usuario comunica su objetivo y sus restricciones una sola vez, y el sistema se encarga de proponer el plan, generar la compra y sugerir las preparaciones.

#### 2. Personalización
A diferencia de los planes genéricos ("dieta para bajar de peso"), Noshy se construye alrededor de la persona concreta: sus metas, su contexto de vida (si vive solo, presupuesto, tiempo para cocinar y demás). El agente no ofrece una respuesta estándar, sino un menú de planes entre los cuales el usuario elige. Y a medida que cocina y da retroalimentación, el agente aprende, de modo que la propuesta se vuelve cada vez más familiar a sus gustos reales.

#### 3. Conecta la intención con la logística
Tener la receta no sirve de nada si no se tienen los ingredientes, el tiempo o el conocimiento. Noshy busca acortar esa brecha al traducir el plan en una lista de mercado ejecutable y, con base en lo que el usuario realmente tiene, generar preparaciones posibles.

#### 4. El conocimiento accesible e interactivo
Al asociar cada preparación con un agente consultable, el usuario no solo lee una receta: puede preguntarle cómo adaptarla a sus necesidades (sustituciones, porciones, restricciones). Esto convierte el conocimiento culinario de chef  y usuarios de todo el mundo, en algo dinámico y aprovechable.

#### 5. Crea valor que crece con el uso
El ciclo de aprendizaje continuo implica que, mientras más cocina un usuario, mejor entiende el sistema sus preferencias, lo que genera una experiencia cada vez más afinada y difícil de replicar por un competidor sin ese historial. La propuesta de valor de Noshy, por tanto, no se agota en la primera sesión, sino que se fortalece con la constancia del usuario.

---

### Relación entre el modelo de negocio y los procesos clave.

El principal activo de Noshy es la relación que cada agente establece con su usuario, y esa relación se alimenta del proceso de retroalimentación continua. Sin este proceso, el agente se resumiría a un recetario. Por eso, el modelo de negocio se apoya en un proceso que captura cada interacción del usuario (qué elige, qué descarta, qué prepara y qué repite) y la devuelve como conocimiento para afinar la siguiente propuesta. Visto de otra forma, el proceso mismo es el que alimenta al modelo y el modelo le da sentido al proceso. Siendo asi, cuanto mejor sea el sistema entendiendo y anticipando las preferencias del usuario, mayor será el valor percibido y mayor la permanencia en la plataforma. La personalización no es un estado, es un proceso que mejora con cada interacción.

El sistema funciona de la siguiente forma:
1. **Captura del perfil:** el proceso de registrar metas, gustos y restricciones define la materia inicial sobre la que trabaja todo lo demás.
2. **Generación y selección del plan:** el proceso de ofrecer alternativas.
3. **Conversión del plan en lista de mercado:** el proceso logístico que traduce intenciones en compras concretas.
4. **Generación de recetas desde el inventario:** el proceso que usa lo que el usuario realmente tiene.

Cada uno de estos pasos es un proceso que sostiene el eslabón del valor.

El usuario como unidad de la comunidad, es entonces, valioso. El proceso de ir y publicar una receta permite que el contenido crezca de forma orgánica, mientras que el agente consultable de cada preparación agrega una capa de interacción que no existe en una comunidad tradicional. La comunidad no es un extra: es el proceso que sostiene el crecimiento del contenido y de los agentes.

Como equipo de Noshy, la promesa se asocia al proceso;
- Prometemos planes a la medida, entonces el proceso captura el perfil y aprende continuament.
- Prometemos ahorro de esfuerzo, entonces el Proceso es traducir el mercado a recetas posibles.
- Prometemos comunidad viva entoncs se dispone un medio de publicación de contenido,

---

### Rol de la tecnología y los sistemas de información en el modelo.

Los sistemas de información permiten convertir estas ideas en funciones reales dentro de la plataforma.

1. **Personalización:** el motor de IA procesa el perfil, gustos, restricciones y objetivos del usuario para generar planes, recetas y recomendaciones adaptadas.
   
2. **Gestión de datos:** la base de datos funciona como la memoria de Noshy, almacenando perfiles, recetas, inventarios e interacciones. Esto permite que el agente aprenda del comportamiento del usuario y mejore sus recomendaciones.
   
3. **Interacción y comunidad:** el módulo web permite al usuario comunicarse con su agente, consultar recetas, gestionar sus compras y compartir contenido con otros usuarios.
   
4. **Arquitectura del sistema:** separar la IA, los datos y la plataforma web permite que cada componente funcione de manera independiente, facilitando el crecimiento, mantenimiento y estabilidad del servicio.
   
---
