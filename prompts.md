> Detalla en esta sección los prompts principales utilizados durante la creación del proyecto, que justifiquen el uso de asistentes de código en todas las fases del ciclo de vida del desarrollo. Esperamos un máximo de 3 por sección, principalmente los de creación inicial o  los de corrección o adición de funcionalidades que consideres más relevantes.
Puedes añadir adicionalmente la conversación completa como link o archivo adjunto si así lo consideras


## Índice

1. [Descripción general del producto](#1-descripción-general-del-producto)
2. [Arquitectura del sistema](#2-arquitectura-del-sistema)
3. [Modelo de datos](#3-modelo-de-datos)
4. [Especificación de la API](#4-especificación-de-la-api)
5. [Historias de usuario](#5-historias-de-usuario)
6. [Tickets de trabajo](#6-tickets-de-trabajo)
7. [Pull requests](#7-pull-requests)

---

## 1. Descripción general del producto

**Prompt 1:**
Eres un experto Producto owner y tienes que crear un PRD para el desarrollo de una aplicación que permita crear un tipo de sujeto por ejemplo: cliente, socio, proveedor, etc con su código único; además se pueden crear clasificaciones las mismas que pueden tener relaciones por ejemplo un socio puede tener n créditos, o m inversiones con un código único creado por el usuario, cada crédito o inversion posee una ramificación con una etiqueta para ser cargada con información en formato pdf como se aprecia en el ejemplo, la información puede ser modificada, eliminada por el personal autorizado

- socio 1
 	-Crédito 123
		- Documento de identificación
			cedula_123.pdf
		- Solicitudes de crédito
			solicitud_credito_123.pdf
		- Documentos firmados
			pagare_credito_123.pdf	
	-Crédito 124
		- Documento de identificación
			cedula_124.pdf
		- Solicitudes de crédito
			solicitud_credito_124.pdf
		- Documentos firmados
			pagare_credito_124.pdf	

	- inversion 101
		- Documentos legales
			poliza_101.pdf

el stack tecnológico es base de datos PostgreSQL, backend con spring boot y frontend con React, mejora esta descripción para se adapte al estándar de buenas practicas para el detalle de un PRD y consulta si requieres mas información con el fin de afinar a lo mas optimo

**Prompt 2:**

aclarando las preguntas
1) la jerarquía pueden tener n niveles y esta es definida por el administrador.
2) Las etiquetas documentales no se anidan.
3) la etiqueta admite solo uno con version.
4) el código de clasificación es único globalmente.
5) se separan por rol con un código de identificación
6) el atributo principal es un código para cada sujeto que adopte un rol, como socio, proveedor, etc
7) no consideremos migración masiva por el momento
8) no es necesario un flujo de aprobación, solo que los documentos muestren y validen las etiquetas de obligatorio o no.
9) solo pdf.
10) visibilidad únicamente por rol.
11) el despliegue es local con docker.
12) no existe proveedor de identidad corporativo.
13) usuarios concurrentes unos 30 y se esperan unos 200 documentos por mes.
14) el plazo legal por retención es 10 años, el borrado definitivo lo realiza únicamente el administrador.
15) si debe registrar la lectura y descarga del documento
16) se debe realizar todo con shadcn
17) no se requiere firma electronica o sellado en ningún documento.
18) la aplicación se puede utilizar desde la tableta y un pc normal

en caso de existir mas consultas de igual manera me las indicas con el fin de afinar el documento

**Prompt 3:**

---

## 2. Arquitectura del Sistema

### **2.1. Diagrama de arquitectura:**

**Prompt 1:**
Usa el formato que consideres más adecuado para representar los componentes principales de la aplicación y las tecnologías utilizadas. Explica si sigue algún patrón predefinido, justifica por qué se ha elegido esta arquitectura, y destaca los beneficios principales que aportan al proyecto y justifican su uso, así como sacrificios o déficits que implica

**Prompt 2:**

**Prompt 3:**

### **2.2. Descripción de componentes principales:**

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**

### **2.3. Descripción de alto nivel del proyecto y estructura de ficheros**

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**

### **2.4. Infraestructura y despliegue**

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**

### **2.5. Seguridad**

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**

### **2.6. Tests**

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**

---

### 3. Modelo de Datos

**Prompt 1:**
Realiza el Diagrama del modelo de datos usa mermaid para el modelo de datos, y utilizar todos los parámetros que permite la sintaxis para dar el máximo detalle, por ejemplo las claves primarias y foráneas.

**Prompt 2:**

**Prompt 3:**

---

### 4. Especificación de la API

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**

---

### 5. Historias de Usuario

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**

---

### 6. Tickets de Trabajo

**Prompt 1:**
Crea y documenta 3 de los tickets de trabajo principales del desarrollo, uno de backend, uno de frontend, y uno de bases de datos. Da todo el detalle requerido para desarrollar la tarea de inicio a fin teniendo en cuenta las buenas prácticas al respecto

**Prompt 2:**

**Prompt 3:**

---

### 7. Pull Requests

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**
