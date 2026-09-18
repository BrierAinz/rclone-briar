# rclone-briar

Configuración personal de [rclone](https://rclone.org/) para respaldar archivos
propios en Google Drive, cifrados de extremo a extremo.

Es una configuración de escritorio de uso personal. No es un servicio, no tiene
usuarios, no tiene servidor y no está pensada para que la use nadie más.

## Límite de este repositorio

Este repositorio público contiene únicamente documentación de propósito y privacidad.
**No se publican** archivos `rclone.conf`, OAuth client secrets, refresh tokens,
credenciales, nombres de remotes privados, listados de archivos ni rutas personales.
La configuración operativa permanece fuera de GitHub.

## Qué hace

- Copia archivos desde un equipo local a una carpeta de Google Drive del propio
  dueño de la cuenta.
- Cifra el contenido y los nombres de archivo antes de que salgan del equipo,
  usando `rclone crypt`.
- Verifica cada copia por hash.

## Qué no hace

- No comparte archivos con nadie.
- No accede a cuentas ajenas.
- No envía datos a ningún servidor de terceros distinto de Google Drive.

## Seguridad y privacidad

- Los secretos se mantienen fuera del repositorio y del historial de Git.
- La copia usa `rclone crypt` antes de subir contenido al almacenamiento remoto.
- El acceso está limitado a la cuenta del propietario y no se ofrece como servicio a terceros.

Ver [PRIVACY.md](PRIVACY.md) para el detalle de tratamiento de datos.
