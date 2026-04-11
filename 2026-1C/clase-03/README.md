# Clase 03

**Tema:** Argumentos del main (`argc`, `argv`) y variables de entorno (`getenv`)

## Ejemplos 

* **ejemplo01.c** — Imprime la cantidad y lista de argumentos recibidos.
  Probar: argumentos simples, con espacios (entre comillas), vacíos. Comparar comportamiento en Windows vs Unix (Git Bash).

* **ejemplo02.c** — Valida cantidad mínima de argumentos e implementa `--help` / `-h`.
  Probar: con `-h`, con `--help`, con menos de 2 argumentos, con más de 2.

* **ejemplo03.c** — Convierte un argumento a entero usando `atoi`.
  Probar: con un número válido (`42`), con texto (`hola`). Notar que `atoi` no reporta error.

* **ejemplo04.c** — Convierte un argumento a entero usando `strtol`, con validación.
  Probar: con `42`, con `hola`, con `42abc`. Comparar con ejemplo03.

* **ejemplo05.c** — Convierte un argumento a float usando `atof`.
  Probar: con `3.14`, con `hola`. Notar que `atof` no reporta error.

* **ejemplo06.c** — Convierte un argumento a float usando `strtof`, con validación.
  Probar: con `3.14`, con `hola`, con `3.14xyz`. Comparar con ejemplo05.

* **ejemplo07.c** — Lee la variable de entorno `VERBOSE` con `getenv`.
  Probar: `export VERBOSE=1` y ejecutar, luego `unset VERBOSE` y ejecutar. También probar con `USER` y `PATH`.

* **ejemplo08.c** — Suma dos argumentos, con logging condicional via `VERBOSE`.
  Probar: sin VERBOSE (`unset VERBOSE`), luego con VERBOSE (`export VERBOSE=1`). Ver cómo cambia la salida.

**Tema:** Streams
* **ejemplo09.c** — probar sin nada. Luego ver que falla con stdin (fflush. Luego poner el espacio antes de %c en scanf. Luego agregar el while. 
* **ejemplo10.c** — correr en terminal con ./ejemplo10 12.34 > ejemplo10.txt y ver como crea el archivo en lugar de imprimir en pantalla
* **ejemplo11.c** — Mostrar cuando se va por stout y cuando por stderr 