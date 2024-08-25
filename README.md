# Laboratorio 02- Patterns
*Nombres:*

*-Jaider Vargas.*

*-Laura Sofia Gil Chaves.*

## Preguntas
### -¿Cuál es su mayor utilidad?

La herramienta Maven nos ayuda a facilitar y optimizar procesos de desarrolo y hacerlos en el menor tiempo posible. Además, nos proporciona sistema de información de proyectos y contrucción de calidad para así lograr buenas prácticas. 

### -Fases de maven:

*Maven Validate*: Verifica la configuración y estructura de un proyecto sea correcta, validando que todas las dependecias esten disponibles. 

*Comando: mvn validate*

*Maven Compile:* Compila el código fuente del proyecto. Esto incluye la verificacioón de sintaxis y semántica. 

*Comando: mvn compile*

*Maven Test:* Ejecuta las pruebas unitarias, que son escenciales para garatizar el comportamiento esperado. 

*Comando: mvn test*

*Maven Package:* Encapsula el código compilado y los recuros asociados en un fromato de distribución. 

*Comando: mvn package*

*Maven Integrartion Test:*  Hace pruebas de integración
que verifican la interracion entre diferentes servicios dentro del proyecto.

*Comando: mvn integration-test*

*Maven Verify:* Válida el empaquetamiento del código, comprobando  que cumple los lineamientos de calidad.

*Comando: mvn verify*

*Maven Install: *  Instala el empaquetamiento del código del repositorio local de Maven, permitiendo que se reutilize como dependencia en otros proyectos. 

*Comando: mvn install*

*Maven Deploy:* Despliega el código aun repositorio remoto o a un entorno de producción para ser ejecutado.

*Comando: mvn deploy*

### -Ciclo de vida de la construcción:

Existen 3 ciclos de vida de contrucción principales:
*Default o build*: Este ciclo construye, prueba, empaqueta, e instalar un proyecto. 
*Clean:* Maneja la limpieza del proyecto, eliminando compilaciones previas. 
*Site:* Genera la documentación del proyecto.

### -¿Para qué sirven los plugins?
Los plugins amplia las funcionalidades a las aplicaciones web. 

### -¿Qué es y para qué sirve el repositorio central de maven?

Es un repositorio público que contiene colección de biblotecas para usar en los proyectos de Maven de manera centralizada y automatizasda. Nos sirve para gestión de versiones, plugins y acceso de dependencias.
