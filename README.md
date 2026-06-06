# ![Espanime](https://img.shields.io/badge/Espanime-v1.1.0-blueviolet?style=for-the-badge) ![Kodi](https://img.shields.io/badge/Kodi-addon-00a8ff?style=for-the-badge) ![Estado](https://img.shields.io/badge/Estado-Activo-brightgreen?style=for-the-badge)

Fuente: https://tremordev.github.io/espanime/

<p align="center">
  <img src="espanime.png">
</p>


## Funciones de reproducción

### Reproducir (automático)
Prueba los servidores en orden de prioridad y reproduce el primero que funcione sin intervención del usuario. Si uno falla, pasa al siguiente de forma silenciosa. Esta opción solo se muestra cuando hay más de un servidor disponible.

### Dejar solo los que responden
Comprueba el estado de todos los servidores en paralelo (mostrando barra de progreso) y filtra la lista para dejar únicamente los que están disponibles en ese momento. Permite elegir servidor manualmente evitando los enlaces caídos.

### Ordenación dinámica de servidores
Se activa en `Configuración > Ordenación dinámica de servidores`.
El addon baja la prioridad de los servidores que fallan automáticamente. Requiere al menos 5 intentos registrados para ese servidor y un fallo en los últimos 7 días para aplicar la penalización.

### Descarga de streams
Si un servidor falla en streaming, se puede mantener pulsado y seleccionar "Descargar este servidor". Algunos enlaces que fallan por buffering o velocidad de conexión funcionan correctamente una vez descargados localmente.

## Dependencias

El funcionamiento del addon requiere o se complementa con los siguientes módulos:

* **script.module.resolveurl** (Importante)
  * Instalar el repositorio desde el ZIP: `https://raw.githubusercontent.com/Gujal00/smrzips/master/zips/repository.resolveurl/repository.resolveurl-1.0.0.zip` e instalar el módulo desde dicho repositorio en Kodi.
* **script.module.yt-dlp** (Opcional)
  * Descargar ZIP desde: `https://github.com/lekma/script.module.yt-dlp/releases` e instalar desde Kodi.
* **script.module.youtube.dl** (Opcional)
  * Se instala automáticamente al instalar el addon oficial de YouTube en Kodi.
* **service.upnext** (Opcional)
  * Módulo para reproducción automática del siguiente episodio.

### Instalación de dependencias desde Kodi
Si faltan módulos o hay fallos de reproducción:
1. Ir a `Ajustes > Add-ons > Mis add-ons > Add-ons de vídeo > Espanime`.
2. Seleccionar el botón `Dependencias`.
3. Pulsar sobre la dependencia requerida y hacer clic en `Instalar`.
4. Una vez completado, reiniciar el addon.
