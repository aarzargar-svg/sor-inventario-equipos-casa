- **Alumno:** Aarón Zaragoza García
- **Bloque:** Practica_03_Casa_Inventario_Equipos
- **Fase / ejercicio:** Fase 0.2
- **Fecha de inicio:** 26/10/2026
- **Fecha de entrega:** 26/10/2026

---

## 🎯 Qué se pedía

Crear desde cero un inventario de equipos utilizando Git y GitHub, guardando tres versiones diferentes. También había que añadir documentación, una imagen y clips de vídeo locales, consultar la primera versión y regresar a `main`. Por último, había que completar y subir la bitácora en un cuarto commit.


## ⌨️ Comandos y pasos importantes

- `pwd`: comprobar la ubicación del repositorio.
    
- `git init`: inicializar Git en `01_Proyecto`.
    
- `git status`: consultar el estado de los archivos.
    
- `git add`: preparar los archivos que se incluirán en el siguiente commit.
    
- `git diff`: ver los cambios que todavía no están preparados.
    
- `git diff --cached`: revisar los cambios preparados.
    
- `git commit -m "mensaje"`: guardar una versión en el historial.
    
- `git push`: subir los commits a GitHub.
    
- `git check-ignore -v`: comprobar por qué se ignoran los clips.
    
- `git log --oneline`: consultar el historial.
    
- `git switch --detach`: visitar temporalmente el primer commit.
    
- `git switch main`: regresar a la versión actual.
## 🛠️ Qué he hecho

He creado una bóveda independiente llamada `Boveda_Inventario_Casa` y he colocado el repositorio únicamente en `01_Proyecto`. Después, he creado el CSV inicial, el README, la bitácora y el archivo `.gitignore`.

He guardado una primera versión con los archivos iniciales. En la segunda versión, he cambiado la ubicación de EQ01 y el estado de EQ02. En la tercera, he añadido EQ03, documentación sobre mantenimiento y estados, una imagen y enlaces desde el README.

También he preparado individualmente los archivos de la ampliación, he comprobado que los clips locales estaban ignorados y he visitado el primer commit para comparar las versiones. Finalmente, he regresado a `main` y he completado la bitácora.
## 🚩 Qué me ha fallado y cómo lo he resuelto

He tenido un problema al revisar que todo estuviera bien subido en github, pero lo he conseguido solucionar haciendo otro commit, en el video se como lo arreglo.

## 🤔 Respuestas a las preguntas
¿Por qué el repositorio está en 01_Proyecto y no en la raíz de la bóveda?

Porque así Git controla únicamente los archivos del proyecto. La configuración de Obsidian y las grabaciones quedan fuera del repositorio, evitando incluir archivos que no forman parte de la entrega.

¿Qué dos celdas de datos cambiaste en la segunda versión y cómo se ven en diff?

Cambié la ubicación de EQ01 de `Aula-1` a `Aula-3` y el estado de EQ02 de `disponible` a `mantenimiento`. En `git diff` aparecen las líneas antiguas con un signo `-` y las nuevas con un signo `+`.

¿Qué diferencia hay entre editar una fila y preparar ese cambio con add?

Editar una fila modifica el archivo guardado en el ordenador. Ejecutar `git add` prepara esa modificación en el índice para incluirla en el siguiente commit. Todavía no se guarda una nueva versión ni se sube a GitHub.

¿Por qué la ficha nueva aparece en status y no en el diff de equipos.csv?

Porque la ficha `inventario/mantenimiento/EQ02.md` es un archivo nuevo y sin seguimiento, mientras que `git diff -- inventario/equipos.csv README.md` solo muestra modificaciones de esos archivos ya conocidos. Para preparar la ficha hay que utilizar `git add` y después revisar el índice con `git diff --cached`.

¿Qué archivos preparaste individualmente en la ampliación y qué mostró diff --cached?

Preparé individualmente estos cinco archivos:

- `inventario/mantenimiento/EQ02.md`
    
- `inventario/criterios-estados.md`
    
- `inventario/imagenes/equipo.png`
    
- `inventario/equipos.csv`
    
- `README.md`
    

Con `git diff --cached --stat` pude ver un resumen de los archivos preparados. Con `git diff --cached` pude revisar su contenido, incluyendo las modificaciones del CSV y del README, los documentos nuevos y el resumen de la imagen, cuyo contenido binario no se muestra como líneas de texto.

¿Cómo demostraste que los clips existen y están ignorados sin subirlos?

Comprobé que los archivos `revision-01.mp4` y `revision-02.mp4` existían en la carpeta `inventario/videos/` y los reproduje para verificar que eran vídeos reales. Después utilicé `git check-ignore -v` para comprobar que la regla `*.mp4` de `.gitignore` los excluía. Así permanecieron en el ordenador sin incluirse en los commits ni en GitHub.

¿Qué ubicación y estado recuperaste al visitar el primer commit y qué ocurrió con EQ03?

Al visitar el primer commit, EQ01 volvió a estar en `Aula-1` y EQ02 volvió al estado `disponible`. EQ03 desapareció porque todavía no existía en esa primera versión. Al regresar a `main`, recuperé la versión actual, con EQ01 en `Aula-3`, EQ02 en `mantenimiento` y EQ03 en `Aula-1` con estado `disponible`.

¿Por qué este CSV necesita historial y qué limitaciones tiene frente a un inventario multiusuario real?

Necesita historial para conservar las versiones, consultar cambios anteriores y saber cómo ha evolucionado el inventario. Git permite comparar entregas y recuperar versiones antiguas. Sin embargo, un CSV con Git no ofrece por sí solo permisos específicos, validación de datos ni edición simultánea controlada. Tampoco garantiza que los datos sean correctos.

¿Cómo comprobaste la subida de la bitácora y por qué su cierre ocurre después del vídeo?

Comprobé la modificación con `git diff`, preparé únicamente la bitácora con `git add` y revisé la selección con `git diff --cached --stat`. Después realicé el cuarto commit, ejecuté `git push` y comprobé el estado y el historial con `git status` y `git log --oneline`. Finalmente, abrí la bitácora en GitHub y verifiqué los enlaces del vídeo y de la playlist.

El cierre ocurre después del vídeo porque la bitácora debe incluir el enlace real y las marcas de tiempo definitivas. Por eso se realiza un cuarto commit documental que no aparece en la grabación ya terminada.

## 🔗 Enlaces


- **Vídeo de esta fase:** https://youtu.be/J89gifD5Ybs?si=7pgN5QrdO59I4hp5
- **Playlist:** https://www.youtube.com/playlist?list=PLfmnpwoiP41c

## 💭 Dudas / a repasar



- [ ]  nada.