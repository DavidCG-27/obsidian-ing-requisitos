# Tema 1. Fundamentos de la Ingeniería de Requisitos
La ingeniería de requisitos se usa en otras profesiones.
- Donde más se utiliza y donde más está desarrollada es en la ingeniería del software.
## 1. Introducción

>[!question] Requisitos
>Un requisito es una circunstancia o condición necesaria para algo.
>No es lo mismo requisito que requerimiento. Es muy común este error en la traducción.
>Un requisito hace referencia a un sistema o software concreto.
>Los requisitos de un software concreto serán las necesidades, en sentido amplio, que debe satisfacer ese software y en qué condiciones específicas debe hacerlo

![[Pasted image 20251019233019.png]]
La ingeniería de requisitos es lo primero que se hace y lo último que estudiamos.

---
## 2. Desarrollo de la Ingeniería de Requisitos.

### 1. Pasar de cliente a *stakeholder*
**Stakeholder**: *Parte interesada (persona u organización) que tiene algo que decir sobre el software a construir y sus requisitos.*
Identificar a todos los stakeholders es una tarea complicada, ya que no son solo los clientes, son los usuarios finales, administradores, operadores, organismos, ... 
### 2. Principio del incremento creciente de coste
Cuanto más tiempo pasa entre que se detecta el error y se corrige, más cuesta corregirlo. 
Crece exponencialmente.
Con los requisitos es fácil cometer un error y no darse cuenta.
El análisis de requisitos dice al equipo de desarrollo lo que tienen que hacer, pero ellos no conocen a los stakeholders, por lo que no saben detectar cuando hay un error en los requisitos.

Estos errores es muy común que los detecte el cliente en el estado final de producto.

Consecuencias de errores en requisitos:
- Abandono total del proyecto.
- Sobrecostes.
- Retrasos en la implantación.
- ...

### 3. Afrontar mantenimiento de los requisitos
Cuello de botella en el mundo TIC -> MANTENIMIENTO
Gran parte del software actual requiere únicamente mantenimiento. 
Existe software en mantenimiento creado hace casi 20 años.

### 4. Formalizar y sistematizar todas las actividades y documentos asociados a los requisitos.
Existen herramientas para facilitar esto.

### 5. Adaptación a las metodologías ágiles
Adaptarse a entornos donde usen Scrum (por ejemplo), aunque es bastante complicado.

### 6. Uso de las IAs generativas
Auge herramientas 0-code: Utilizando IA generativa, permite crear el paradigma del *desarrollador ciudadano* (crear el producto software comunicándose mediante el lenguaje natural con la IA).

---
## 3. Definiciones formales 

>[!NOTE] Definiciones formales
• **Ingeniería de Requisitos:** *«Función interdisciplinar que media entre los dominios del adquirente (comprador) y el proveedor para establecer y mantener los requisitos que un sistema/software determinado debe satisfacer»*
>
• **Stakeholder**: *«Individuo u organización que tiene un derecho, participación, reclamación o interés en un sistema/software o en que este posea ciertas características que satisfagan sus necesidades y expectativas»* 
>
• **Requisito**: *«Afirmación que traduce o expresa una necesidad y sus restricciones y condiciones asociadas»*
>
• **Restricción** (constraint): *«Limitación impuesta externamente al software, su diseño o implementación, o al proceso utilizado para desarrollar o modificar un software»*
>
• **Condición**: *«Atributo cualitativo o cuantitativo medible que se estipula para un requisito y que indica una circunstancia o evento bajo el cual se aplica dicho requisito»*

> *Apuntes y comentarios varios*

El ingeniero de requisitos es un mediador entre dos mundos: el mundo de los *stakeholders* y el mundo de los desarrolladores.

¿Por qué los patrocinadores son *stakeholders*?
- Su interés es salir en el producto final.

Muchas veces hay que traducir lo que dice el stakeholder a algo que tenga sentido.
Debemos ser precisos y no decir cosas que se puedan interpretar de varias maneras.
Los requisitos no entran en como hacer las cosas, sino en que deben de hacer.

* Proceso cooperativo: Trabajo con *stakeholder*, equipo de desarrollo, ...
* Proceso Iterativo: Hay que hacer iterativas aproximaciones para acercarse mejor al objetivo

---
## 4. Tipología de los requisitos

Cosas que parecen requisitos y que **no lo son**:
- *Decisiones de diseño, arquitectura o implementación*: Los requisitos no dicen como hacer las cosas, sino dicen que deben de hacer. **Solo se deben incluir estas cosas cuando los *stakeholder* lo imponen.**
- *Decisiones de proyecto*: Ejemplo: Esto no debe de costar 1000 euros; tenéis que utilizar esta metodología; ... 
- *Necesidades que el software no puede cubrir*: Necesidades que el *stakeholder* quiere cubrir y que el software no puede hacer o asegurar.

Debido a la diversidad de requisitos, realizaremos dos clasificaciones distintas. Vamos a clasificar los requisitos en función de: 
* Su objeto:
	* Requisitos funcionales
	* Requisitos no funcionales
* Su perspectiva y nivel de detalle y abstracción:
	* Requisitos de usuario o *stakeholder*
	* Requisitos de software
### Requisitos funcionales
Describe lo que hace el sistema desde un punto de vista externo. 
Nos dicen como debe de responder el software, que debe de hacer, sin entrar en como lo hace internamente.
Para facilitar la gestión de los mismos, se suelen agrupar cuando hay muchos (por funcionalidades relacionadas, por tipo de usuario, ...).
A veces se les denominan «capacidades»
### Requisitos no funcionales
*Todos los demás :)*
Los funcionales expresan servicios que hace el software, y los no funcionales expresan restricciones.
Pueden condicionar el diseño y la arquitectura.

> **Ej**: *Necesito un tiempo de respuesta menor a 30 ms*

Depende del dominio, un requisito puede ser funcional o no funcional.

Existen diferentes maneras de clasificarlos, dependiendo del proyecto. Algunas de estas son:
* IEEE 830: Más antigua y tradicional.
* MEGEPA/GADEPA: Utilizada por el Principado de Asturias. 

## Requisitos de usuario
Lo correcto sería ***"Requisitos de stakeholder"***
Lo que el *stakeholder* expresa que necesita. 
Muchas veces lo hace con su lenguaje.
No son precisos, el *stakeholder* expresará sus necesidades de manera imprecisa y habrá que depurarlos y obtener la información importante.
### Requisitos de Software
Son requisitos de *stakeholder* pero más desarrollados y orientados a un lenguaje más familiar al lenguaje del equipo de desarrollo.
Debemos de refinar y desarrollar los requisitos del stakeholder.
Son mucho más detallados y concretos.

*Como gestionar ambos tipos de requisitos*
- **Opción 1**: Comienzo con los requisitos de *stakeholder*, y lo voy desarrollando y refinando hasta convertirlo en requisito de software.
- **Opción 2**: Documentarlos por separado.
- **Opción 3**: Mantener ambos en el mismo documentos, dejando los RSt (Requisitos de Stakeholder) como alto nivel (más genérico) y explotándolos en uno o varios RS (Requisitos de software).
	![[Pasted image 20251020001138.png]]

---
## 5. Especificación de requisitos del software (SRS)
Este es el **producto final.**
Documento que sirve de base para continuar con el proyecto.

El responsable de su creación es el ingeniero de requisitos o analista, junto a los *stakeholders*.
Ingeniero de requisitos se comunica con los stakeholders y pasa especificación al equipo de desarrollo.
	Ellos no tienen contacto con la empresa ni con los clientes, por eso tiene que ser clara y sin ambigüedades.

Esta especificación tiene que ser aprobada por los stakeholders designados
	Normalmente el que paga, aunque a veces delegan en gente más técnica y preparada.

>[!DANGER] Importante
Si el cliente final dice que el producto no se corresponde a lo que quería, siempre se revisará el documento firmado y aprobado por los *stakeholders* designados.

La especificación es fundamental para el desarrollo del proyecto. 
	Con ella se determinará la arquitectura, el diseño, la codificación, las pruebas, ...
	Los presupuestos, normalmente, se hacen a partir de la especificación.

Lo más normal es escribir la especificación en lenguaje natural.
	Algo que pueda entender cualquier stakeholder.

> [!NOTE] Características de un buen SRS (tomado de IEEE 830): 
> * **Correcto**: *«…cada requisito que se indica en él es uno que el software debe cumplir» *
> * **No ambiguo**: *«…cada requisito indicado en él tiene una única interpretación» *
> * **Completo**: si incluye todos los requisitos y es completo formalmente 
> * **Consistente**: *«…ningún subconjunto de requisitos individuales descritos en él entra en conflicto» *
> * **Clasificado por importancia y/o estabilidad**: esenciales, deseables u opcionales, si se esperan cambios… 
> * **Verificable**: se puede comprobar de forma objetiva si el software satisface cada requerimiento
>* **Modificable**: si puede evolucionar de manera sencilla 
>* **Trazable**: documentar el origen de cada requisito y mantener un id único para los siguientes documentos

---
## 6. Rol del ingeniero de requisitos
Ingeniero de requisitos no es un puesto normalmente, sino más bien un rol.
	*Analista senior, Director de proyectos, ...*
Está enfocado a perfiles senior, con más experiencia.

> [!note] Características de un buen ingeniero de requisitos
	> - **Buena capacidad de análisis y síntesis**
	> - **Detección de incoherencias**: darte cuenta de lo que falta o lo que está mal
	> - **Empatía**: implica mucho trato sso.
	> - **Buena expresión escrita**: Hay que escribir especificaciones.
	> - **Capacidad de diálogo y negociación**: El ingeniero de requisitos es el intermediario entre los stakeholders y el equipo de desarrollo, debe tratar con ambos constantemente.

---

> [!success] Resumen
> 1. La Ingeniería de Requisitos es la primera etapa del ciclo de vida del software 
> 	* Aunque, habrá que gestionar cambios en los requisitos en cualquier momento del ciclo de vida del software 
> 2. Su finalidad es crear una especificación de requisitos (SRS) que exprese las necesidades que debe satisfacer el software 
> 	* Para ello, tiene que mediar entre los *stakeholders* y el equipo de desarrollo 
> 	* Es un proceso: se comienza con la perspectiva del *stakeholder* y se termina con la del software 
> 3. Un buen trabajo de Ingeniería de Requisitos es fundamental para el éxito de un proyecto de software 
> 4. Hay requisitos funcionales y no funcionales, de «usuario» y de software 
> 5. Los requisitos y el SRS como tal deben de cumplir con ciertas características 
> 6. El rol de ingeniero de requisitos, junto con el de director/jefe de proyectos, es de los que tienen mayor proyección y recorrido profesional