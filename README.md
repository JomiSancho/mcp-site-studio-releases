# MCP Site Studio

Canal público de paquetes estables de **MCP Site Studio**, plugin de WordPress para gestionar contenido y preparar cambios de diseño mediante MCP. Requiere WordPress 6.9 o posterior y PHP 8.2 o posterior. Conserva el slug `qls-mcp-content` para actualizar instalaciones existentes.

## Descarga e instalación

1. Abre [la última release estable](https://github.com/JomiSancho/mcp-site-studio-releases/releases/latest).
2. Descarga `qls-mcp-content-VERSION.zip` y su archivo `.zip.sha256` de esa misma release. Los archivos de código fuente que genera GitHub corresponden a la documentación de este canal; el plugin instalable es el ZIP adjunto con ese nombre.
3. Comprueba el SHA-256 del ZIP frente al checksum. En Linux/macOS: `sha256sum --check qls-mcp-content-VERSION.zip.sha256`. En PowerShell: `Get-FileHash ./qls-mcp-content-VERSION.zip -Algorithm SHA256` y compara el resultado.
4. En WordPress, utiliza **Plugins → Añadir plugin → Subir plugin**, instala el ZIP y actívalo. Para actualizar, conserva una copia recuperable y reemplaza el plugin con el mismo slug.
5. Abre **Herramientas → MCP Site Studio → Preparación** para preparar el adaptador MCP oficial. La autenticación conserva los permisos de WordPress y depende del cliente y del proveedor disponible.

El paquete incluye el código PHP editable, la guía de uso y el changelog de la versión. Desde 0.5.0, WordPress consulta y descarga este canal sin una cuenta GitHub ni credenciales. Las instalaciones 0.4.0 o anteriores necesitan un primer reemplazo manual con el ZIP oficial. Las actualizaciones automáticas son opcionales en Plugins y requieren WP-Cron y permisos de escritura del hosting. Publicar una release no instala el plugin en ninguna web.

## Licencias y código fuente

El código propio se distribuye bajo [AGPL-3.0-only](LICENSE). La unidad de bloques adaptada conserva GPLv3 y sus avisos; se incluyen [GPLv3](LICENSE-GPL-3.0.txt) y [los avisos de procedencia](THIRD_PARTY_NOTICES.md). Los archivos PHP del ZIP son el código fuente distribuido. La administración y `qls-wordpress/get-plugin-license` ofrecen además una descarga autenticada del código instalado.

Este repositorio conserva documentación pública y paquetes aprobados. Su historial documental es independiente del desarrollo. No contiene configuración de instalaciones, credenciales ni dependencias de herramientas de desarrollo.
