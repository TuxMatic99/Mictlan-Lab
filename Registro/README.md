# Registro Mictlán

Formulario de una observación con nombre y nota. Está escrito en `.mict` y usa las API públicas `ui`, `archivo`, `cadena` y `lista`. Funciona con el mismo anfitrión que VectorLab.

Abre una terminal en una carpeta privada para guardar tu observación. Usa una ruta absoluta al archivo si está en otra carpeta.

```bash
/ruta/a/mictlan-ui -- /ruta/a/Registro/principal.mict
```

Escribe un nombre y una nota. Tab y Mayús+Tab cambian el foco. Enter en un campo o el botón Guardar solicita el guardado. Recuperar vuelve a mostrar la última observación. Cerrar termina la ventana. El guardado reemplaza `registro-v1.txt` en la carpeta de trabajo de forma atómica.

El archivo tiene tres líneas UTF-8, terminadas por LF. La cabecera es `Registro-v1`, seguida por el nombre y la nota. Cada campo puede ocupar hasta 255 bytes y contiene una sola línea. El formulario exige dos puntos de código como mínimo para el nombre. Los nombres españoles con acentos se conservan.

Para probar el módulo de datos sin ventana, usa la consola desde una carpeta temporal vacía.

```bash
/ruta/a/mictlan -- /ruta/a/Registro/pruebas/datos.mict
```
