# LS-RP SA:MP Launcher

LS-RP SA:MP Launcher es un ejecutable para Windows que funciona como acceso directo al servidor de San Andreas Multiplayer "Los Santos - Juego de Rol". Incorpora un proceso extra para mantener una conexión con Discord.

## Características
- Inicia SA:MP y conecta a LS-RP directamente al ejecutar el programa.
- Inicia un proceso extra que mantiene una conexión con Discord y se cierra automáticamente al abandonar el juego.
- Dispone de una instalación rápida que genera accesos directos en escritorio y en menú inicio. Al utilizar el instalador, la información se guarda en el registro de Windows para poder desinstalar el programa con facilidad.
- Genera un archivo (`lsrp-samp-launcher.log`) con información sobre funcionamiento del programa. Se reescribe en cada ejecución.

## Requisitos

Debe tener instalado Grand Theft Auto: San Andreas y San Andreas Multiplayer (en la misma carpeta).

## Instalación

Descargue y ejecute la [última versión del instalador](https://github.com/Autorojo/lsrp-samp-launcher/releases/latest).

Indique su carpeta de instalación de GTA San Andreas y San Andreas Multiplayer, luego instale el programa.

## Solución de problemas

Si tiene errores durante la instalación, pruebe iniciando el instalador como administrador (click derecho > Ejecutar como administrador).

Si tiene errores al ejecutar el programa, pruebe iniciando el programa como administrador. También puede configurar el programa para ejecutarse siempre como administrador (click derecho > Propiedades > Compatibilidad > Ejecutar este programa como administrador > Aceptar).

Si tiene errores de otro tipo, compruebe el archivo `lsrp-samp-launcher.log` e inicie un issue.

## Detalles técnicos

El instalador guarda información en el registro de Windows para facilitar la desinstalación.

La información es accesible desde las siguientes rutas:

- `HKEY_CURRENT_USER\Software\lsrp-samp-launcher`
- `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall\lsrp-samp-launcher`

El instalador descomprime y guarda los siguientes archivos en el directorio del juego:

- `lsrp-samp-launcher.exe`
- `lsrp-samp-launcher.ico`
- `lsrp-samp-launcher-uninstall.exe`

También se crean accesos directos en menú inicio y escritorio.

- `%APPDATA%\Microsoft\Windows\Start Menu\Programs\Los Santos - Juego de Rol`
- `%USERPROFILE%\Desktop`

Un archivo de texto es creado al ejecutar el programa. Se reescribe en cada ejecución.

- `lsrp-samp-launcher.log`
