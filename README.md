# Laboratorio 02- Patterns
*Nombres:*

*-Jaider Vargas.*

*-Laura Sofia Gil Chaves.*

## Preguntas
### -¿Cuál es su mayor utilidad?

La herramienta Maven nos ayuda a facilitar y optimizar procesos de desarrolo y hacerlos en el menor tiempo posible. Además, nos proporciona sistema de información de proyectos y contrucción de calidad para así lograr buenas prácticas. 

### -Fases de maven:

![image](https://github.com/user-attachments/assets/d23f6ad4-13e9-4b32-957a-b52e2ad3f274)

*Maven Validate*: Verifica la configuración y estructura de un proyecto sea correcta, validando que todas las dependecias esten disponibles. (*Comando: mvn validate*)

*Maven Compile:* Compila el código fuente del proyecto. Esto incluye la verificacioón de sintaxis y semántica. (*Comando: mvn compile*)

*Maven Test:* Ejecuta las pruebas unitarias, que son escenciales para garatizar el comportamiento esperado. (*Comando: mvn test*)

*Maven Package:* Encapsula el código compilado y los recuros asociados en un fromato de distribución. (*Comando: mvn package*)

*Maven Integrartion Test:*  Hace pruebas de integración que verifican la interracion entre diferentes servicios dentro del proyecto. (*Comando: mvn integration-test*)

*Maven Verify:* Válida el empaquetamiento del código, comprobando  que cumple los lineamientos de calidad. (*Comando: mvn verify*)

*Maven Install: *  Instala el empaquetamiento del código del repositorio local de Maven, permitiendo que se reutilize como dependencia en otros proyectos. (*Comando: mvn install*)

*Maven Deploy:* Despliega el código aun repositorio remoto o a un entorno de producción para ser ejecutado. (*Comando: mvn deploy*)

### -Ciclo de vida de la construcción:

Existen 3 ciclos de vida de contrucción principales:

*Default o build*: Este ciclo construye, prueba, empaqueta, e instalar un proyecto. 

*Clean:* Maneja la limpieza del proyecto, eliminando compilaciones previas. 

*Site:* Genera la documentación del proyecto.

### -¿Para qué sirven los plugins?
Los plugins amplia las funcionalidades a las aplicaciones web. 

### -¿Qué es y para qué sirve el repositorio central de maven?

Es un repositorio público que contiene colección de biblotecas para usar en los proyectos de Maven de manera centralizada y automatizasda. Nos sirve para gestión de versiones, plugins y acceso de dependencias.

# EJERCICIO DE LAS FIGURAS
## CREAR UNPROYECTO CON MAVEN

Realizamos la búsqueda de cómo se crea el proyecto maven con ayuda de arquetipos. Además, cómo ejecutar desde línea de comandos el objetivo "generate" del plugin "archetype",con los siguientes parámetros:
Grupo: edu.eci.cvds
Id del Artefacto: Patterns
Paquete: edu.eci.cvds.patterns
archetypeArtifactId: maven-archetype-quickstart
Para visualizar la estructura usamos el comando:
*cd Patterns
tree /f*
![image](https://github.com/user-attachments/assets/e1998679-5bcb-4c01-8987-318dd792ebc7)

## AJUSTAR ALGUNAS CONFIGURACIONES EN EL PROYECTO

Hay que cambiar la version del compilador de Java a la versión 8, para ello, agregue la sección properties antes de la sección de dependencias:
![image](https://github.com/user-attachments/assets/70ebdfd6-f22c-438a-9d1b-86beb440fdfc)

## COMPILAR Y EJECUTAR
Para compilar el proyecto de maven se usa el comando:
*mvn package*
Buscamos cómo ejecutar desde línea de comandos un proyecto maven:
*mvn exec:java -Dexec.mainClass="edu.eci.cvds.patterns.App"*
![image](https://github.com/user-attachments/assets/6a10e2a5-0b87-465c-a96d-1e1594d53bc9)
Realizamos el cambio en la clase App.java para crear un saludo personalizado, basado en los parámetros de entrada a la aplicación.
![image](https://github.com/user-attachments/assets/a12ec8fa-1aa9-41af-872b-e19b820c0bb0)

Buscamos cómo enviar parámetros al plugin "exec".
![image](https://github.com/user-attachments/assets/b1b822e5-2776-44e9-a091-66cc12237133)

Ejecutar la clase con su nombre y apellido como parámetro. ¿Qué sucedió?
Lo que sucecedio fue que solo imprimio el primer nombre, el primer elemento del arreglo, debido a esto, tocó utilizar un  join
para que resultara el nombre y apellido.

## HACER EL ESQUELETO DE LA APLICACIÓN




