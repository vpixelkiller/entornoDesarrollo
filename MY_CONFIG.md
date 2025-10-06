# Mi entorno de desarrollo


| HARDWARE | VALOR | 
| :--- | :--- | 
| **Product** | Macbook Pro |
| **Chip** | Apple M2 Pro |
| **Memoria** | 16GB |
| **Almacenamiento** | 494.38 GB|
| **Tarjeta gráfica** | Apple M2 Pro - GPU |




| SOFTWARE | VALOR | 
| :--- | :--- | 
| **Product** | macOS |
| **ProductVersion** | 15.6.1 |
| **IDE's** | NVIM v0.11.3 |
| **Herramientas** | DBeaver, Postman, Docker (Orbstack)|
| **Lenguajes de programación** | node v20.12.1, Python 3.13.3 |
| **Bases de Datos** | DuckDb, Postgres|



## Reflexiones para examen

`¿Por qué es importante mantener el software actualizado?`
- La principal razón para actualizar el software es la seguridad.
    - Los desarrolladores descubren y corrigen contínuamente fallos de seguridad.
    - El malware utiliza a menudo el software desactualizado.
- Estabilidad y rendimiento
    - Corrigen bugs
    - Optimizan el rendimiento
    - Se realizan habitualmente actualizaciones para el perfecto funcionamiento con el nuevo hardware

Aunque la experiencia me dice que, por lo menos a la hora de actualizar el `OS` vale la pena esperar algún mes,
que esté bien testeado y hayan sacado algún parche.

`¿Cómo afecta el uso de versiones antiguas al rendimiento y seguridad?`
- El rendimiento se ve afectado porque las nuevas versiones llevan consigo una optimización del código que hacen que el software sea más rápido y consuma menos recursos.
- Las versiones más nuevas a menudo son más eficientes en el uso de la batería en portátiles y en el consumo general de energía, ya que no fuerzan tanto los componentes.
- Las versiones antiguas contienen fallos de seguridad que ya fueron descubiertos y publicados.
- Los desarrolladores dejan de ofrecer soporte técnico y, lo que es más importante, dejan de lanzar parches de seguridad para versiones antiguas. 

`¿Qué es el PATH y para qué se usa?`
El PATH es una variable de entorno que contiene en formato string la ruta a los directorios que necesitas que estén contemplados cada vez que ejecutas un comando.
Por ejemplo, yo escribo: `echo $PATH` en mi terminal y me devuelve:
```
/opt/homebrew/opt/libpq/bin:/Users/victorlatency/.nvm/versions/node/v20.12.1/bin:/opt/homebrew/bin:/opt/homebrew/sbin:/usr/local/bin:/System/Cryptexes/App/usr/bin:
/usr/bin:/bin:/usr/sbin:/sbin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/local/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/bin:
/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/appleinternal/bin:/opt/X11/bin:/Applications/iTerm.app/Contents/Resources/utilities:/Users/victorlatency/.orbstack/bin:
/Users/victorlatency/.local/bin:/Users/victorlatency/.nvm/versions/node/v22.2.0/bin
```

La idea de usar **PATH** es no tener que escribir la ruta completa para ejecutar un comando:
- Para ejecutar Orbstack (Docker) tendría que hacer:
    `/Users/victorlatency/.orbstack/bin docker compose up -d`
- Sin embargo, gracias a usar *PATH* hago:
    `docker compose up -d`

Y hace exáctamente lo mismo




