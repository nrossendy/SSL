Compilador seleccionado: gcc via MinGW-w64;

Compiler Vers: gcc (Rev3, Built by MSYS2 project) 13.2.0;

Versión C que compila; 

Soporta C11
>gcc -std=c11 -dM -E - < NUL | findstr __STDC_VERSION__
>
#define __STDC_VERSION__ 201112L

Soporta C18
>gcc -std=c18 -dM -E - < NUL | findstr __STDC_VERSION__
>
#define __STDC_VERSION__ 201710L

<.Probé el compilador con un programa hello.c que imprime Hello World en consola.

<.Ejecuté el programa y verifiqué que la salida es la esperada.

<.Ejecuté el programa con la salida redireccionada según la docu CharacterInputOutputRedirection a un archivo "output.txt" (.\hello.exe > output.txt) ya que ya estába compilado. El contenido del txt coincidía con el de stdout
