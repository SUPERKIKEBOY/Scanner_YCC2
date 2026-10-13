# Etiqueta Scanner V2 (Android NYX)

## Funciones
- CameraX + ML Kit para códigos de barras y OCR.
- Captura HU, NP, Dado, Máquina, Cantidad, Fecha.
- Nueva HU reinicia campos; seis campos completos insertan en SQLite con HU UNIQUE.
- Etiquetas de Ensamble y Moldeo, incluyendo NP con S, máquinas E/F/G, dado junto o debajo del título.
- Orientación horizontal y exportación de todos los registros CSV mediante selector de archivos de Android.
- SQLite conserva nombre de archivo y esquema de V1 (`etiquetas_v1.db`).

## GitHub
Crear repositorio nuevo preferiblemente privado y subir el **contenido** descomprimido de este ZIP a la raíz, incluidas las carpetas `.github` y `app`. Actions -> Build Etiqueta Scanner V2 APK -> Run workflow; descargar artifact Etiqueta-Scanner-V2.

## Atención a los datos
El identificador de app sigue siendo `com.er.etiquetascanner`, pero GitHub Actions puede firmar cada APK debug con una clave diferente. Si Android no permite actualizar, **no desinstalar V1 sin respaldar primero sus datos**: desinstalar elimina SQLite. Probar V2 en otro equipo o disponer de un método de respaldo y firma estable.

## Validación pendiente
Proyecto preparado, no compilado ni probado físicamente en este entorno. Verificar con etiquetas reales los seis campos y el CSV. El OCR es heurístico y puede fallar ante sellos o texto borroso.
