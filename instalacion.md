# Instalación de un Sistema Operativo en Raspberry

## Sistemas Operativos para la Raspberry

Para instalar un SO en la Raspberry, primero deberemos de elegir que SO queremos.

Estos son algunos SO más populares según su uso:

  1. **Raspbian**: Es el sistema operativo ofical de la Raspberry. Es una versión de Debian, que está adaptada y optimizada específicamente para la Raspberry.

  2. **NOOBS y NOOBS Lite**: Es una aplicación que se instala en la tarjeta de memoria en vez de instalar un SO. La versión Lite, es una versión más ligera que la anterior.

  3. **Retroarch**: Es un emulador en el que se podrá jugar cualquier juego de consolas clásicas hasta modernas.

  4. **OSMC**: Este SO está especialmente diseñado para ser utilizado como centro multimedia, además viene con una aplicación llamada KODI, que nos permite acceder a contenido multimedia, servidor SAMBA y servidor SSH.

  5. **Windows IoT Core**: Está diseñado para un control de las conexiones y de los dispositivos. Su entorno gráfico no es como el habitual, sino que trae uno específico para desarroladores.

  6. **Ubuntu**: Si buscas algo más funcional y estándar.

## Tarjeta de memoria

Los SO o aplicaciones se instalan en las tarjetas SD o MicroSD. Hay que tener en cuenta que necesitaremos un tarjeta con suficiente capacidad (Entre 8 y 16 GB), aparte de un formato correcto.

Aplicaciones para dar formato:
Para **Windows y Mac**:
- [SD Memory Card Formatter](https://www.sdcard.org/downloads/formatter/)
Para **Linux**:
- [GParted](https://gparted.org/download.php)

## Instalación en Windows

1. Descargar e instalar la aplicación para instalar el SO en la Raspberry. En este caso es BerryBoot; Permite añadir más de un SO en una tarjeta SD.
- [BerryBoot](https://www.berryterminal.com/doku.php/berryboot)
2. Ejecuta la app. Seleccione la unidad donde se instalará el SO.
3. Seleccion el SO a instalar.
Ya podríamos introducir la tarjeta en la Raspberry

## Instalación en Mac

1. Descargamos la app.
- [ApplePi-Backer](https://www.tweaking4all.com/hardware/raspberry-pi/applepi-baker-v2/)
También en muy usada está app para hacer copias de seguridad y restaurar cualquier cos	a que esté o no relacionada con la Raspberry.
2. Haremos los pasos 2 y 3 de Windows.
3. Puedes hacer una copia de seguridad de instalación actual, le damos a _Backup_ y si quieres instalar otro SO, le damos a _Restore_ y volvemos a seleccionar otra imagen.
Introducimos la tarjeta en la Raspberry.

## Instalación en Linux

La instalación se realizará através de comandos.

1. Instalaremos las dependencias necesarias.
	>sudo apt-get install -y pv curl python-pip unzip

	>sudo pip install awscli

2. Ejecutamos el siguiente comando, que nos mostrará la información del SO.

	>uname -s

2. Si el comando nos devuelve _Linux_

	>wget https://raw.githubusercontent.com/hypriot/flash/master/Linux/flash

3. Lo que nos devuelva el comando anterior los sustituiremos por Darwin en el siguiente comando.

	>wget https://raw.githubusercontent.com/hypriot/flash/master/Darwin/flash

	>chmod +x flash

	>sudo mv flash /usr/local/bin/flash

Ya sabríamos hacer la instalación en diferentes sistemas operativos.

	
