# Graficacion_Lineas_SDL2

## Graficar Rectas usando SDL2
- Se utilizo la libreria externa SDL2, para graficar rectas, usando varios algoritmos, para saber que pixel dibujar.

## Herramientas Usadas
- CodeBlocks.
- Libreria SDL2

## Requisitos
- Sistema Operativo Windows 10 o 11
- Codebloscks:
- [Codeblocks-20.03mingw-setup](https://www.codeblocks.org/downloads/binaries/)
- Tipo de Sistema de 32 o 64 bits.
- Liberia SDL2:
- - [SDL2-devel-2.30.11-mingw.zip](https://github.com/libsdl-org/SDL/releases/tag/release-2.30.11)
- - [SDL2-devel-2.30.9-mingw.zip](https://github.com/libsdl-org/SDL/releases/tag/release-2.30.9)
- Se necesita desactivar el antivirus(opcional).
- Compilador necesario para codeblocks:
- - GNU GCC Compiler.
  
## Instalacion.
- Descargar la libreria SDL2 (version 2.30.11 o version 2.30.9), para evitar conflictos con librerias predeterminadas.
- Descomprimir el archivo descargado.
- Si la computadora es de 32 bit, copiar la siguiente carpeta: i686-w64-mingw32
- Si la computadora es de 64 bits, copiar la siguiente carpeta: x86_64-w64-mingw32
- Ubicarse en el disco local, luego buscar la Carpeta "Archivos de Programa" y buscar la carpeta "Codeblocks".
- Pegar la carepeta correspondiente y cambiarle el nombre a "SDL2".

## Configurar la libreria SDL2 en codeblocks.
- Abrir codeblocks y buscar "Configuracion".
- Buscar la opcion "Compiler".
- Buscar y seleccionar "Search directories".
- Elegir de nuevo "Compiler".
- Pegar los siguientes directorios en el siguiente orden(cambiar de direccion acorde a tu dispositivo):
- - C:\Program Files\CodeBlocks\SDL2\bin
- - C:\Program Files\CodeBlocks\SDL2\include
- - C:\Program Files\CodeBlocks\SDL2\lib
- Buscar y seleccionar "Linker settings":
- Pegar los siguientes archivos en el siguiente orden(cambiar de direccion acorde a tu dispositivo):
- - C:\Program Files\CodeBlocks\SDL2\lib\libSDL2.a
- - C:\Program Files\CodeBlocks\SDL2\lib\libSDL2.dll.a
- - C:\Program Files\CodeBlocks\SDL2\lib\libSDL2_test.a
- - C:\Program Files\CodeBlocks\SDL2\lib\libSDL2.main.a
- - C:\Program Files\CodeBlocks\SDL2\lib\libSDL2.dll

## Crear proyecto en codeblocks.
- Buscar y seleccionar "Create new proyect".
- Buscar la opcion "SDL2 proyect".
- Ponerle un nombre y ubicacion al proyecto.
- Dirigirse a la carpeta "SDL2", ubicada en la carpeta "Codeblocks" del disco local.
- Elegir el compilador "GNU GCC Compiler".
- Dar clic en finalizar.
- Se creara un nuevo proyecto, con un archivo llamado 'main.cpp' o 'main.c'.
- Dirigirse en donde estan declaradas las librerias y buscar la siguiente libreria: "#include <SDL.h>"
- - Cambiarlo por: "#include <SDL2/SDL.h>"
- Buscar un boton de 'rebuild' (boton azul) en la barra de herramientas y dar click.
- Va a salir un error, pero no sera un problema, solo se necesita para que se creen las carpetas:
- - bin\Debug
  - obj\Debug
    
## Agregar archivos al proyecto.
- Buscar los archivo "SDL2.dll" y "libSDL2.dll.a", en la carpeta de codeblocks del SL2.
- Copiar y pegar los archivos "SDL2.dll" y "libSDL2.dll.a", en la carpeta "bin\debug" de tu proyecto.
- Buscar un boton de 'rebuild' (boton azul) en la barra de herramientas y dar click.
- Buscar el boton de 'run' o 'Build and run'.
- Va a salir una ventana de error, dar en cerrar ventana.
- Ese error va a continuar saliendo cada vez que lo ejecutes.

