# rclone-briar

Configuración personal de [rclone](https://rclone.org/) para respaldar archivos
propios en Google Drive, cifrados de extremo a extremo.

Es una aplicación de escritorio de uso personal. No es un servicio, no tiene
usuarios, no tiene servidor y no está pensada para que la use nadie más.

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

## Privacidad

Ver [PRIVACY.md](PRIVACY.md).
