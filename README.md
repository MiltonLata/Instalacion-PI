# Instalacion-PI

DEscargar el sofware desde la pagina oficial de raspberry pi (https://www.raspberrypi.org/downloads/raspbian/) despues descargamos el Raspbian Buster with desktop mediante Utorrent.
Pasos para iniciar la raspberry pi 3:
  1.- Formatear la tarjeta de memoria (8GB) mediante el programa SD Card Formatter abrimos el programa y ya aparecerá registrado la             tarjeta microSD, pero por si algún caso no aparece, solo hay que darle a “Refresh” para que se solucione. Nos dirigiremos al botón         de “Options” donde configuraremos un par de cosas. En la opción “Format Type” seleccionaremos “Full (Overwrite)”, y en “Format Size       Adjustement” elegiremos “ON”. Le damos a “OK” y luego a “Format”.
  2.- Despues lo montamos en la tarjeta (8Gb) el programa Raspbian Buster with desktop mediante el programa win32 Disk Image 4.0.
  3.- entramos en la tarjeta de memoria para editar archivo config.txt para cambiar la resolucion de la pantalla de la raspberry pi 3 el          cual debemos habilitr las opciones: a)disable_overscan=1    b)framebuffer_width=1280 y framebuffer_height=720.
  4.- Insertamos la tarjeta de memoria en la raspberry pi 3 y lo alimentamos con 5V DC.
  5.- Configurar lo siguiente: a)Pais(Ecuador), Lenguaje (Espanol), zona horaria (Guayaquil) y el tipo de idioma que se usara para el teclado.
  6.- cambiamos la contrasena (balanza)
  7.- conectamos a la red wifi
  8.- Activar el Vnc (para una conexion con la Pc)
  9.- Entrar al comando: sudo raspi-config (cambiar las opciones: expand file system)
Pasos para configurar la pantalla tactil del pasberry pi (https://www.altaruru.com/raspberry-pi-como-instalar-una-pantalla-lcd-de-3-5/)
  1.- sudo apt-get update
  2.- sudo apt-get upgrade
  3.- sudo rm -rf LCD-show  (para borrar restos de una instalacion anterior del alguna pantalla tactil)
  4.- Clonamos repo git en local: git clone https://github.com/goodtft/LCD-show.git
  5.- Damos permisos de ejecución: sudo chmod -R 755 LCD-show
  6.- Entramos en el directorio: cd LCD-show/
  7.- Selecionamos: 5.0″ HDMI Display(Resistance touch)(MPI5008) -> sudo ./LCD5-show
  8.- Reiniciar la raspberry pi 3: sudo reboot

  
