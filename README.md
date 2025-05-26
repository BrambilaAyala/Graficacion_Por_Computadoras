# Graficacion_Lineas_SDL2

## Graficar Rectas usando SDL2
Este proyecto permite graficar líneas utilizando la librería externa **SDL2**, implementando distintos algoritmos para determinar qué píxeles deben dibujarse en pantalla.

## Objetivo

Explorar y comparar diferentes algoritmos de trazado de líneas mediante gráficos generados con **SDL2** en C/C++.

## Herramientas Usadas
- **Code::Blocks**.
- **Libreria SDL2**.

## Requisitos
- Sistema Operativo Windows 10 o 11
- **Code::Blocks**
 - [Codeblocks-20.03mingw-setup](https://www.codeblocks.org/downloads/binaries/)
- Tipo de Sistema de 32 o 64 bits.
- Liberia SDL2:
 - [SDL2-devel-2.30.11-mingw.zip](https://github.com/libsdl-org/SDL/releases/tag/release-2.30.11)
 - [SDL2-devel-2.30.9-mingw.zip](https://github.com/libsdl-org/SDL/releases/tag/release-2.30.9)
- Se necesita desactivar el antivirus(opcional).
- Compilador necesario para **Code::Blocks**:
  - `GNU GCC Compiler`.
  
## Instalacion.
1. Descargar la libreria SDL2 (version 2.30.11 o version 2.30.9), para evitar conflictos con librerias predeterminadas.
2. Extraer el archivo `.zip`.
3. Copiar la carpeta correspondiente según la arquitectura de tu sistema:
   - **32 bits**: `i686-w64-mingw32`
   - **64 bits**: `x86_64-w64-mingw32`
4. Ubicarse en el disco local, luego buscar la Carpeta **Archivos de Programa** y buscar la carpeta **Codeblocks**: `C:\Program Files\CodeBlocks`
5. Pegar la carpeta correspondiente y cambiarle el nombre a **SDL2**.

## Configurar la libreria SDL2 en codeblocks.

1. Abrir Code::Blocks y buscar `Configuracion`.
2. Buscar la opcion `Compiler`.
3. Buscar y seleccionar `Search directories`.
4. Elegir de nuevo `Compiler`.
5. Pegar los siguientes directorios en el siguiente orden(cambiar de direccion acorde a tu dispositivo):
 - `C:\Program Files\CodeBlocks\SDL2\bin`
 - `C:\Program Files\CodeBlocks\SDL2\include`
 - `C:\Program Files\CodeBlocks\SDL2\lib`
5. Buscar y seleccionar `Linker settings`:
6. Pegar los siguientes archivos en el siguiente orden(cambiar de direccion acorde a tu dispositivo):
 - `C:\Program Files\CodeBlocks\SDL2\lib\libSDL2.a`
 - `C:\Program Files\CodeBlocks\SDL2\lib\libSDL2.dll.a`
 - `C:\Program Files\CodeBlocks\SDL2\lib\libSDL2_test.a`
 - `C:\Program Files\CodeBlocks\SDL2\lib\libSDL2.main.a`
 - `C:\Program Files\CodeBlocks\SDL2\lib\libSDL2.dll`

## Crear proyecto en codeblocks.
1. Buscar y seleccionar `Create new proyect`.
2. Buscar la opcion `SDL2 proyect`.
3. Ponerle un nombre y ubicacion al proyecto.
   - Para la **direccion**, dirigirse a la carpeta "SDL2", ubicada en la carpeta "Codeblocks" del disco local.
4. Elegir el compilador `GNU GCC Compiler`.
5. Dar clic en finalizar.
6. Se creara un nuevo proyecto, con un archivo llamado `main.cpp` o `main.c`.
7. Dirigirse en donde estan declaradas las librerias y buscar la siguiente libreria:
   - `#include <SDL.h>`
   - Cambiarlo por: `#include <SDL2/SDL.h>`
9. Buscar un boton de `rebuild` (boton azul) en la barra de herramientas y dar click.
10. Va a salir un error, pero no sera un problema, solo se necesita para que se creen las carpetas:
    - `bin\Debug`
    - `obj\Debug`
    
## Agregar archivos al proyecto.
1. Buscar los archivo `SDL2.dll` y `libSDL2.dll.a`, en la carpeta de codeblocks del SL2.
2. Copiar y pegar los archivos `SDL2.dll` y `libSDL2.dll.a`, en la carpeta `bin\debug` de tu proyecto.

## Compilar el proyecto.
1. Buscar un boton de `rebuild` (boton azul) en la barra de herramientas y dar click.
2. Buscar el boton de `run` o `Build and run`.
3. Va a salir una ventana de error, dar en cerrar ventana.
4. Ese error va a continuar saliendo cada vez que lo ejecutes.
