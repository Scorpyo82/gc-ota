gc-ota
======

gc-ota es un script creado por un conjunto de funciones con contról de argumentos que hace operaciones de descarga OTA en una rom (rooteada).


Se incluye un archivo build.prop a modo de ejemplo.
Explicación de los valores en build.prop:

gingercerecilla.version=0.8
Es el número de versión actual de la rom, en este caso la "0.8"

gingercerecilla.update=0
Es el número de actualización en curso, en este caso es la "0" (no ha recibido actualizaciones)

gingercerecilla.url.repo=http://www.pc-citos.es/gingercerecilla/repo/updates
Es la ruta completa hasta donde se encuentra el archivo de repositorio.



Se incluye un archivo "updates" a modo de ejemplo.
Explicación de los valores en el archivo updates:


Se compone de 5 columnas:

VERSION   -> Número de versión de la ROM a la que va destinado el update.zip (0.8, 1.5, etc)
Nº_UPDATE -> Número de actualización (1, 2, 3, etc)
MD5       -> Suma de verificación correspondiente al archivo update.zip
URL       -> Link de descarga del archivo update.zip
Cambios   -> Cambios realizados en el update (sin espacios) ejemplo: "Última_actualización_que_proporciona_soporte_OTA"


Nota: El archivo "updates" es el más importante de todos ya que contiene información importante y sensible para acceder a las actualizaciones, así que debe estar en un sitio seguro y controlado solo por el desarrollador de la ROM



Ayuda:
	gc-ota Version 1.0

    Modo de empleo: gc-ota [Opción]

    --app              Ejecuta los trabajos por defecto para usar la app "Ajustes Especiales GC".
    --check            Busca y muestra la información usando el último repo descargado
    --update           Actualiza el repositorio, muestra información, pero no actualiza el sistema
    --upgrade          Actualiza el sistema con la versión superior que esté disponible en el servidor
    --version          Muestra la versión de gc-settings
    --help             Muestra esta ayuda

    Desarrollado por <Miguel Ponce Torres> bajo GNU GPL <http://www.gnu.org/licenses/>
    MAIL: miguelponcetorres@gmail.com
