# Tema 2. Proceso de la Ingeniería de Requisitos
## 1. Introducción
Actividades principales que conforman la Ingeniería de Requisitos:
![[Pasted image 20251020002351.png]]

---

## 2. Definición de las actividades principales

### Educción u obtención de requisitos

> [!QUOTE] Definición formal
> *«La actividad de obtener de las fuentes apropiadas la información básica para identificar y documentar los requisitos de los stakeholders»*

Obtener de la fuentes apropiadas (*stakeholders* principalmente) la información básica para identificar y documentar los requisitos de los *stakeholders*.

Normalmente, es el proceso más complicado y el que más tiempo lleva.
Debemos de identificar a los *stakeholders* que debemos de preguntar y, formular las preguntas que les vamos a hacer.

Es difícil porque es la parte con la que interaccionamos con personas.
	Se puede dar cualquier tipo de situación.
	Muchas veces, son gente que no saben nada de informática.
	Puede ser que sean tantos que no sabes a quien preguntar o como afrontarlo.
	Muchas veces debemos de ganarnos al *stakeholder* para que vea que estamos de su lado.
	Existen técnicas para dominar esto (Ciencias sociales).

### Análisis de requisitos

>[!quote] Definición formal
> *«Análisis de los requisitos educidos (obtenidos) con el fin de entenderlos y documentarlos»*

Consiste en "trabajar" los requisitos obtenidos en la educción.
Vamos a destripar los requisitos para entenderlos mejor.
	Muchas veces más que los propios *stakeholders*.

Objetivos del análisis de requisitos:
* Detectar lagunas o conflictos entre requisitos… que habrá que resolver 
* Precisar mejor el alcance de los requisitos, completar información asociada a ellos, clasificarlos u organizarlos… 
* Ir moviendo el foco o perspectiva desde los *stakeholders* hacia el software

### Especificación de requisitos.

>[!quote] Definición formal
> *«Plasmar los resultados de la educción y el análisis en un documento de especificación de requisitos (SRS)»*

Terminar de refinar los requisitos y plasmarlos en un documento de especificación de requisitos.
Este documento debe ser formal, y los requisitos seguir una serie de características.

### Validación de requisitos

>[!quote] Definición formal
> *«El proceso de confirmar que los requisitos documentados coinciden con las necesidades de los stakeholders; en otras palabras, si se han especificado los requisitos correctos»*

Se trata de verificar que el trabajo que hemos hecho (la especificación) es lo que esperaban los stakeholders.
La especificación de requisitos debe ser validada por los stakeholder designados.

### Gestión de requisitos

>[!quote] Definición formal
> *«El proceso de gestionar los requisitos existentes y los productos de trabajo relacionados con los requisitos, incluyendo el almacenamiento, modificación y trazabilidad de los mismos»*

Consiste en afrontar cambios en los requisitos a lo largo de todo el ciclo de vida del software.
Esta etapa estará presente a lo largo de todas las demás, no solo al final.
Debemos de mantener la consistencia entre ellos.

---

## 3. Flujo real del proceso
Vamos a ir construyendo la especificación de requisitos del software poco a poco.
De manera iterativa e incremental.

![[Pasted image 20251020003603.png]]

En cada iteración, vamos refinando mucho más los requisitos.
La situación ideal:
	▪ *Iteración 1:* Requisitos de negocio o dominio (los de más alto nivel).
	▪ *Iteración 2*: Requisitos de *stakeholder* más concretos. 
	▪ *Iteración 3*: Requisitos de software.

En la vida real casi nunca podemos hacerlo así.
Pasan un montón de cosas que nos lo van a impedir:
* Los *stakeholders* no van a estar disponibles siempre que quieras.
* Muchas veces debemos de retroceder para negociar partes de la especificación.
* En algunas partes de la especificación estaremos más avanzados que en otras.
* Los stakeholders suelen cambiar de opinión.
* ...

---

## 4. Otras actividades
### Negociación de requisitos
Resolver conflictos entre requisitos.
Por ejemplo, que dos stakeholders digan cosas distintas sobre una misma funcionalidad.
Los conflictos pueden aparecer en cualquier momento.
### Verificación de requisitos
Verificar que los requisitos están bien construidos formalmente.
Que sigan las características vistas en el tema anterior.
No confundir con la verificación del software.

---

> [!success] Resumen
> 1. En la Ingeniería de Requisitos pueden identificarse varias actividades principales: 
> 	1. **Educción**: obtener los requisitos de los *stakeholders* 
> 	2. **Análisis**: completarlos, subsanar conflictos y desarrollarlos para llegar a requisitos de software 
> 	3. **Especificación**: plasmar lo anterior en un SRS 
> 	4. **Validación**: validar con los *stakeholders* que el SRS expresa correctamente todas sus necesidades 
> 2. Estas actividades se realizan de forma iterativa e incremental (modelo de espiral) 
> 3. Además, la **gestión de requisitos** se encarga de lidiar con los cambios o evolución de los requisitos, durante el proceso de desarrollo y en el mantenimiento del software 
> 4. Otras tareas, como la negociación y verificación de requisitos, ocurren como parte de las anteriores
