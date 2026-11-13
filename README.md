# Gestión de Boxes — instaladores

Instaladores para Windows de la app de escritorio **Gestión de Boxes**. Este repositorio solo
distribuye los instaladores; no contiene el código fuente.

## Descargar la última versión

| Instalador | Cuándo usarlo | Enlace |
|---|---|---|
| **MSI** | Caso normal, en un PC con internet | [GestionBoxes.msi](https://github.com/Demiannnnnn/Cesfam-Boxs-releases/releases/latest/download/GestionBoxes.msi) |
| **Sin internet** | PC sin conexión o sin WebView2 (incluye todo lo necesario) | [GestionBoxes-sin-internet.exe](https://github.com/Demiannnnnn/Cesfam-Boxs-releases/releases/latest/download/GestionBoxes-sin-internet.exe) |
| **Setup liviano** | Alternativa al MSI | [GestionBoxes-setup.exe](https://github.com/Demiannnnnn/Cesfam-Boxs-releases/releases/latest/download/GestionBoxes-setup.exe) |

Todas las versiones, incluidas las de prueba, están en
[Releases](https://github.com/Demiannnnnn/Cesfam-Boxs-releases/releases).

## Al instalar

- El instalador no está firmado. Si Windows muestra **«Windows protegió su PC»**, pulsa
  **Más información** y luego **Ejecutar de todas formas**.
- Para actualizar, desinstala primero la versión anterior desde **Configuración → Aplicaciones**.
  Los datos del servidor se conservan.
- Instalar el modo servidor pide permisos de administrador.

## Quitar el servidor de un equipo

Desinstalar la app desde Windows **no** quita el servidor: el servicio sigue funcionando y el
equipo recuerda su modo. Para quitarlo, descarga
[desinstalar.bat](https://github.com/Demiannnnnn/Cesfam-Boxs-releases/releases/latest/download/desinstalar.bat),
haz clic derecho sobre el archivo y elige **Ejecutar como administrador**.

- Detiene y elimina el servicio del servidor y sus reglas de firewall.
- Borra el modo guardado: al abrir la app de nuevo vuelve a preguntar cómo usar el equipo.
- **Conserva** la base de datos, los respaldos y los registros en `C:\ProgramData\GestionBox`.

Atención: si ese equipo es el servidor en uso, los demás equipos se quedan sin servicio.
