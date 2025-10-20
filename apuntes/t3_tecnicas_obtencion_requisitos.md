# Tema 3: Técnicas de obtención de requisitos.
## 1. Introducción
Obtener los requisitos tiene una serie de pasos lógicos, no ir a lo loco a tomar apuntes.
1. Identificar fuentes de información (la mayoría de las veces personas, aunque no siempre).
2. Escoger una técnica adecuada para cada fuente
3. Preparar y planificar las técnicas.
4. Ejecutar la técnica (entrevista, analizar documentación, ...)

---
## 2. Fuentes de requisitos
Existen tres categorías principales de fuentes de requisitos.
* ***Stakeholders***
* **Documentos**
* **Sistema/Software existente**

La educción no basta con hacerla una única vez.
La ingeniería de requisitos es un proceso iterativo, por lo que nos podemos ir encontrando diferentes fuentes de requisitos a lo largo de la vida del proyecto.
### 2.1. *Stakeholders*
Solemos agruparlos por grupos o selecciones, aunque al final siempre tratemos con personas, no con grupos abstractos.
Normalmente empezamos identificando grupos y luego personas concretas.
#### Identificación de los *stakeholders*
1. Empezamos con los *stakeholders* obvios (cliente, ...).
2. Luego, buscamos *stakeholders* más concretos (por ejemplo, podemos revisar el organigrama de la empresa/organización, ...)
Una vez los hemos identificado y seleccionado, los debemos de documentar en una lista

>[!DANGER] Importante
>Siempre debemos de realizar la trazabilidad. 
>Todos los stakeholders deben de tener un identificador.

Existe un tipo especial de stakeholders: **los usuarios finales.**

Es muy buena práctica identificar que *stakeholders* pueden **ser un estorbo**, para evitar que perjudiquen al proyecto 
	*Truco*: mandar encuesta con propuestas de mejoras del producto que se va a hacer. Dependiendo de las respuestas que den, se puede suponer que *stakeholder* es un lastre.

### 2.2 Documentos
Podemos encontrar muchos requisitos en documentación relacionada con el software que vamos a desarrollar.
* *Legislación, normativa interna o estándares de obligado cumplimiento:* Nos los puede aportar la propia empresa (documentación de software parecido, del software anterior al que estamos creando, ...).
* *Planes estratégicos de la empresa*: sus objetivos, importante para conocer bien la empresa.
* *Documentación del anteproyecto*: Antes de realizar cualquier tipo de proyecto serio, siempre se hace un anteproyecto que explica la idea que se quiere realizar. Sirve para que los mandatarios de la empresa comprendan de que va el proyecto y nos contraten a nosotros para su realización. Es **básico** para empezar a hacer los requisitos. Incluye los estudios de viabilidad y demás información útil. Es probable que contenga una primera versión de los requisitos.
* *Especificaciones de requisitos de sistemas previos*: Si lo que tenemos que hacer es construir software que sustituya a otra software, es muy útil consultar la documentación del software anterior.
* *Manuales de usuario de sistemas previos o de la competencia*: Muchas veces, la competencia tiene cosas que nosotros podemos necesitar, o que estaría bien imitar.
* *Documentación de interfaces con otros sistemas*: Hoy en día, muchos sistemas están interconectados. Es importante conocer los sistemas con los que tendrá relación y contacto nuestro software (otros software de la empresa, por ejemplo), así podemos analizar su comportamiento antes estas acciones.
* *Documentos generados en el proceso de negocio relacionado*: Todo proceso de negocio produce algún tipo de informe. Todos esos documentos hay que tenerlos en cuenta. Igual, nuestro nuevo software tiene que generar documentos parecidos, o con información similar. Muchas veces son facturas, abales, certificados, ...

Antes de realizar la reunión de proyecto, es **muy recomendable** leer alguno de estos documentos, para enterarnos de que va el negocio.

Al igual que tenemos una lista de *stakeholders*, debemos de tener una lista de documentos.
La forma de proceder es la misma.

Muchas veces los documentos están asociados a un *stakeholder* que no es persona física.
A veces las organizaciones, nos hablan a partir de documentos.
### 2.3. Sistemas o software existente
A veces podemos obtener información muy útil de sistemas existentes, tanto internos como externos a la empresa/organización.
* *Software con el que el nuevo va a relacionarse*.
* *Plataformas en los que debe de integrarse*: Sirve para identificar restricciones técnicas (integración, ...). También ayuda a identificar la usabilidad que esperan los usuarios (parecida a las plataformas que ya existe). Nos sirve también para aprovechar sus funcionalidades (menos trabajo).
* *Software que va a ser reemplazado*: Como mínimo, nuestro software hará lo mismo o más.
* *Software que se espera que influya en el futuro*: Nos sirve para prepararnos para posibles cambios o actualizaciones en el futuro.
* *Software de la competencia*: Cogemos ideas.
Como siempre, debemos de documentarlo todo adecuadamente. Puede ser que estos sistemas estén ligados a stakeholders o documentos previamente identificados.

---
## 3. Técnicas de análisis de documentos y software
### 3.1 Análisis de documentación para educir requisitos
El **error típico** es coger un documento importante que sabemos que tiene información y **empezar a leerlo**.

Una buena técnica es la **lectura basada en perspectiva**.
Consiste en que cuando vamos a leer un documento, lo primero que tenemos que hacer es identificar desde que perspectiva lo vamos a leer. Es decir, desde que rol lo vamos a leer (usuario, responsable de seguridad, desarrollador software, ...) Así, atendemos solamente a lo que tenga que ver con el rol. 

Cuando ya hemos decidido desde que perspectiva leemos el documento, lo empezamos a leer y solo tomamos apuntes de lo que le interesa a nuestro rol.

Un documento puede tener diferentes puntos de vista. Si en el equipo hay varias personas, cada una puede leer el documento desde una única perspectiva.
El resultado de esta lectura (o lecturas), será un documento de notas (o similar).

Debemos registrar toda esta información relevante para, posteriormente, analizarla. 
En muchos casos, debemos de acudir a la fuente original de los registros que apuntamos, por eso es importante tenerlo todo documentado.
### 3.2. Reutilización de requisitos
Es muy útil buscar la especificación de requisitos del sistema que vamos a reemplazar o, si no aplica, el de sistemas similares.

Todas las especificaciones de requisitos de softwares públicos son públicas. Esto nos puede servir si tenemos pensado hacer un software parecido a alguno público.

Es muy útil para obtener requisitos no funcionales.

Si optamos por la reutilización de requisitos, obtendremos unas listas de requisitos **potenciales**, que igual debemos de adaptarlos a nuestro contexto y que debemos de contrastar mediante otros medios.
### 3.3. Análisis de software existente
Se suele hacer con el software que queremos reemplazar.

Tenemos que tener claro que queremos buscar.
	Nuevas funcionalidades, nuevos roles de usuario, estilos de IU, preparar entrevistas a stakeholders, ...
	
Debemos analizar:
* **La documentación del software**: Manuales, especificaciones, ...
* **El software en un entorno de pruebas**: Mucho más controlado que en producción.
* **Código fuente**: Esto solo si lo anterior no nos proporciona suficiente información.
## 4. Técnicas para pedir información
* **Preguntas cerradas**: Preguntas que se responden con una lista determinada de respuestas. No son tan comunes ni útiles en ingeniería de requisitos.
	(Ej: elige la opción correcta entre varias, elige entre si o no, elige entre un rango de números...). 
* **Preguntas abiertas**: Preguntas con cualquier tipo de respuesta (libre). Requieren un análisis posterior. Se utilizan mucho más.
### 4.1 Entrevistas
Técnica más usada.
*Preparación antes de la entrevista:*
	**Identificar quien es el entrevistado**
		Tenemos una serie de *stakeholders*, escogemos uno.
	**Tener claro para que queremos la entrevista**
		Tenemos que saber que información queremos obtener y sus criterios de calidad (para saber si la entrevista salió bien o no).
	**Preparar una guía para la entrevista.**
		Lista de temas a tratar o preguntas que le vamos a hacer.
		Existe el concepto de árbol de decisión
	![[Pasted image 20251014161708.png]]
		**Organizar la entrevista**
			Lugar, hora, quien toma notas, quien pregunta, ...
			
*Resultados de la entrevista*
	La información obtenida será analizada posteriormente.
		Después, podremos construir requisitos, información adicional de los requisitos que ya teníamos, nuevas fuentes de información, ...

Ideal --> Entrevista de un único *stakeholder*.
	Juntar a varios puede llevar a problemas.
	
Nosotros somos lo que debemos de dirigir la entrevista.
	El *stakeholder* no debe de hablar de lo que le apetezca. 
	Debemos de controlar el tiempo.
	Debemos ser educados y claros, buscando la **empatía**.
	Debemos de verificar que hemos entendido la respuesta que nos ha dado el entrevistado.
		Puede haber confusiones.
		Técnica --> Devolverle la respuesta con nuestras palabras "*Ah, o sea, que lo que me quieres decir es ..."*. Así, nos aseguramos de que el nos confirme que es exactamente eso lo que nos quiso decir.
	No es importante únicamente que dice, si no también **cómo** lo dice.
	
La entrevista debe de durar como máximo 1 hora (ideal: entre 20 y 40 minutos).
	El lugar es muy importante. Presencialmente se genera más empatía.
	Debemos evitar las distracciones
	
Es muy recomendable informar al *stakeholder* de lo que le vamos a preguntar durante la entrevista
	Los temas que trataremos, una lista de preguntas, un guion, ...
	Así, ya va pensando en ello. Ya va preparado para contestarnos.
	
Es una práctica habitual dar una copia del acta o resumen de la entrevista al *stakeholder*.
	El entrevistado validará el contenido, corrigiendo posibles errores.

### 4.2 Cuestionarios
Lista de preguntas que deben de contestar los *stakeholders* seleccionados.
Se les enviará la lista de preguntas para que las contesten y nos devuelvan la información.

Pueden ser cuestionarios con preguntas abiertas (lo más común) o con preguntas cerradas (menos habitual).
- **Preguntas cerradas**: Útiles para verificar información que ya tenemos.
- **Preguntas abiertas**: Útiles para obtener información que no teníamos. Debemos de procesar dicha información después de obtenerla.
Es muy importante preparar bien las preguntas.
	Deben de ser claras y directas, siguiendo un orden lógico.

---
## 5 Técnicas de observación
Técnicas que se basan en observar a los *stakeholders* realizar su trabajo habitual, relacionado con el software a construir.
### 5.1 Trabajo/observación de campo
Observamos al *stakeholder* en su trabajo habitual, **sin interferir.**

>[!question] ¿Por qué no preguntar al stakeholder directamente?
	>A veces, hay información implícita que los stakeholders tratan de manera tan natural, que no se dan cuenta de contartelo. 
	>Nadie es consciente de que eso se está haciendo, lo dan por hecho.   
	>También nos sirve para ver como trabajan, costumbres, hábitos, ...
### 5.2 Inmersión como aprendiz
Ingeniero de requisitos **toma el rol de aprendiz.**

Hace como si fuera un nuevo empleado.
No nos limitamos a preguntar y observar, realizamos el trabajo.
Esto nos da un punto de vista diferente.
### 5.3 Indagación contextual
Mezcla entre la observación y la entrevista.

Nos presentamos y observamos como hace ciertas cosas. No le engañamos en nada.
Mientras observamos como realiza la tarea, le vamos preguntando.
No nos limitamos a observar, le realizamos ciertas preguntas sobre lo que está haciendo.

---
## 6 Técnicas de trabajo colaborativo
Poner a trabajar en conjunto a varios *stakeholders* para educir requisitos.
La técnica colaborativa más común es el **taller** (workshop).

Juntamos a varios expertos para que trabajen juntos para definir, crear o desarrollar un requisito.
El ingeniero de requisitos funciona como **facilitador**.
	*Preparación*: Debemos de preparar el taller 
	*Inicio*: Dar la bienvenida a los participantes (presentarlos entre sí), explicarles los objetivos (cual es nuestra finalidad, en que nos vamos a centrar...), marcar una serie de reglas (poner orden)
	*Dirección*: Animar a la participación, reorientar el trabajo si se dispersa, ...
	*Cierre*: Agradecer la participación, explicar lo que se va a hacer con los resultados que han obtenido (muy importante, si no, sentirán que han perdido el tiempo).

* **¿Cuándo es útil hacer un taller?**
	Cuando tenemos los requisitos generales pero debemos de tomar ciertas decisiones para refinarlos del todo.
	Estos expertos serán los que tomen dichas decisiones.
	Ahorra mucho tiempo al ingeniero del software (si no, deberíamos de entrevistarlos individualmente y llegar a conclusiones).
* **Dificultades**
	Lugar, tiempo, personas, dinero, ...
	
>[!NOTE] Otras técnicas
>- **Grupos focales**: Orientados a obtener opiniones de un producto o servicio.
>- **Uso de redes sociales y software *ad hoc*** para que un montón de gente aporte ideas sobre que tipo de funcionalidades tiene un software.

---
## 3.7 Pautas de uso
**Reunión de arranque del proyecto**
	Necesaria para conocer contexto general
	
**¿Qué hacer primero?**
	Leer la documentación existente
	Si hay software legacy --> Pedir acceso
	
**¿Cuándo recorrer a cuestionarios frente a entrevistas?**
	Si no podemos hacer una entrevista
	Para refinar requisitos potenciales.
	Para pedir información específica.
	Lo normal no es empezar con ellos, ya que necesitamos mucho conocimiento del tema
	
**¿Cuándo recurrir a técnicas de observación?**
	Vemos que nos falta información que nadie nos da.
	Vemos que tenemos incoherencias entre documentos y práctica real.
	Cuando no es posible sacar al *stakeholder* de su puesto de trabajo.
	
**¿Cuándo recurrir a técnicas colaborativas?**
	Cuando no está muy claro qué se necesita, porque es algo nuevo.
	Cuando las «necesidades» son subjetivas, para ayudar a alcanzar consensos.

---

>[!success] Resumen
> 1. Hay diferentes fuentes de requisitos, cada una con diferentes técnicas específicas de educción: 
> 	1. Stakeholders: 
> 		▪ Preguntar: Entrevistas y cuestionarios 
> 		▪ Observar: trabajo de campo, inmersión laboral e indagación contextual 
> 		▪ Trabajo colaborativo: Talleres y otros 
> 	2. Documentos 
> 		▪ Lectura basada en perspectiva 
> 		▪ Reutilización de requisitos 
> 	3. Software 
> 		▪ Análisis de software existente 
> 2. El análisis de documentación y las entrevistas son las técnicas más utilizadas 
> 	* Las otras las complementan y permiten ampliar la capacidad de educción de requisitos
> 	* Las técnicas se aplican dependiendo de su disponibilidad, de los objetivos concretos de la educción y de la situación de las fuentes y el contexto

