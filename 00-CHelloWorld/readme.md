# Trabajo #0
**Número de equipo:** ##

**Nombre del equipo (opcional):** -

**Autores de la resolución:** Rossendy Nicolás

**Usuario github:** nrossendy

**Legajo:** 177.380-0

**Apellido:** Rossendy

**Nombre:** Nicolás Nahuel

**Número y título del trabajo:** - [Trabajo #0 (Individual): §3. “Hello, World” en C]

**Transcripción del enunciado:** 

Adquirir y preparar los recursos necesarios para resolver los trabajos del curso.
1. Cuenta en GitHub
2. Repositorio para público para la materia
3. Instalar Compilador C11/C18
4. Publicación - Publique el trabajo en el repositorio personal SSL la carpeta 00- CHelloWorld con readme.md, hello.c, y output.txt.
5. Armado de Equipo.

## Hipótesis de trabajo que surgen luego de leer el enunciado: 
Podré aplicar conocimientos aprendidos en AyED para poder llevar a cabo el código, teniendo en cuenta las diferencias entre C++ y C.
Buscar el compilador a priori parece ser una actividad de investigación integrada, por lo que puede que sea la más demandante de tiempo.
Al finalizarlo debería quedar más familiarizado con las herramientas y formato de entrega necesarios para abordar la resolución de los trabajos posteriores.

## Resolución: 
**Compilador seleccionado:** gcc *(via MinGW-w64)*
**Compiler Vers:** 13.2.0
**Versión C que compila:** 
- Soporta C11
>gcc -std=c11 -dM -E - < NUL | findstr __STDC_VERSION__
#define __STDC_VERSION__ 201112L
- Soporta C18
>gcc -std=c18 -dM -E - < NUL | findstr __STDC_VERSION__
define __STDC_VERSION__ 201710L

Probé el compilador con un programa hello.c que imprime Hello World en consola.
Luego ejecuté el programa y verifiqué que la salida es la esperada.
Finalmente ejecuté el programa con la salida redireccionada según la docu **CharacterInputOutputRedirection** a un archivo "*output.txt*" (.\hello.exe > output.txt) ya que ya estába compilado. El contenido del txt coincidía con el de stdout
